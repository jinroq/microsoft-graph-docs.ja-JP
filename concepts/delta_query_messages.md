# <a name="get-incremental-changes-to-messages-in-a-folder"></a>フォルダー内のメッセージへの増分の変更を取得する

デルタ クエリでは、一連の[デルタ](../api-reference/v1.0/api/message_delta.md)関数呼び出しを使用して、フォルダー内のメッセージへの追加、削除、または更新に対してクエリを実行できます。デルタ データを使用すると、毎回サーバーからユーザーのメッセージのセット全体をフェッチせずに、ユーザーのメッセージのローカル ストアの保守と同期が行えます。

デルタ クエリでは、フォルダー内 (ユーザーの受信トレイなど) のすべてのメッセージを取得する完全な同期と、最後の同期以降、そのフォルダー内で変更されたすべてのメッセージを取得する増分同期の両方がサポートされています。通常は、フォルダー内のすべてのメッセージの最初の完全同期を実行して、その後、そのフォルダーの増分の変更を定期的に取得します。

## <a name="track-message-changes-in-a-folder"></a>フォルダー内のメッセージの変更を追跡する

デルタ クエリはフォルダー単位の操作です。フォルダー階層内のメッセージの変更を追跡するには、各フォルダーを個別に追跡する必要があります。

通常、メール フォルダー内のメッセージ変更の追跡は、**デルタ**関数を使用した、1 つ以上の GET 要求のラウンドです。最初の GET 要求は、**デルタ**関数を含めることを除いて、[メッセージの取得](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages)方法とほぼ同じです。

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

**デルタ**関数を使用した GET 要求は、次のいずれかを返します。

- `nextLink` (**デルタ**関数の呼び出しと _skipToken_ を使用した URL を含む)、または
- `deltaLink` (**デルタ**関数の呼び出しと _deltaToken_ を使用した URL を含む)。

これらのトークンは、クライアントに対して完全に不透明な[状態トークン](delta_query_overview.md#state-tokens)です。変更追跡のラウンドを続行する手順は、最後の GET 要求から返された URL を、同じフォルダーの次の**デルタ**関数呼び出しにコピーして適用するだけです。応答で返される `deltaLink` は、変更追跡の現在のラウンドが完了したことを示します。`deltaLink` URL を保存して、次のラウンドを開始する際に使用することができます。

`nextLink` と `deltaLink` の URL を使用する方法については、以下の[例](#example-to-synchronize-messages-in-a-folder)を参照してください。

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a>メッセージのデルタ クエリでクエリ パラメーターを使用する

- 任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。`id` プロパティは常に返されます。
- デルタ クエリは、メッセージの `$select`、`$top`、および `$expand` をサポートします。
- `$filter` と `$orderby` に対するサポートには制限があります。
  - サポートされている唯一の `$filter` 式は、`$filter=receivedDateTime+ge+{value}` または `$filter=receivedDateTime+gt+{value}` です。
  - サポートされている唯一の `$orderby` 式は、`$orderby=receivedDateTime+desc` です。`$orderby` 式を含めない場合、戻り値の順序は保証されません。
- `$search` に対するサポートはありません。

### <a name="optional-request-header"></a>オプションの要求ヘッダー

各デルタ クエリの GET 要求は、応答で 1 つ以上のメッセージのコレクションを返します。 必要に応じて、要求ヘッダー `Prefer: odata.maxpagesize={x}` を指定して、応答内の最大メッセージ数を設定できます。

<!--
### Iterative process

A typical round to track message changes goes like this:

1. Make the initial GET request with the mandatory _Prefer: odata.track-changes_ header. If this is your very first delta query
for messages in that folder, don't provide any state token. If the messages support tracking changes, following the iterative
process (steps 2-6) described below will return the entire set of messages in that folder.

2. Check if the first response returns the _Preference-Applied: odata.track-changes_ header,
which confirms your resource supports tracking changes. Stop if you don't receive the response header.

3. If you receive a _skipToken_ (in an _@odata.nextLink_ response header) in the response, you should continue to track the
   additional messages that have changed (added, deleted, or updated). Make a second GET request, using the URL returned
   in _@odata.nextLink_, which includes a _skipToken_.

4. The second request will return additional messages that have changed, and either a _skipToken_ if there are more changed messages,
  or a _deltaToken_ if all the changed messages have been returned.

5. If you receive a _skipToken_ from the last GET request, continue getting the changes by sending a next GET call, similar to step 3.

6. When you eventually receive a _deltaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This
round of change tracking is complete.

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated)
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a>ファルダー内のメッセージを同期する例

次の例では、最初に 5 つのメッセージを含んでいる特定のフォルダーの同期の 2 つのラウンドを示します。

最初のラウンドには、フォルダー内の 5 つのメッセージをすべて同期するための一連の 3 つの要求が含まれます。

- [サンプルの最初の要求](#sample-initial-request)と[応答](#sample-initial-response)
- [サンプルの 2 番目の要求](#sample-second-request)と[応答](#sample-second-response)
- [サンプルの 3 番目の要求](#sample-third-request)と[最後の応答](#sample-third-and-final-response)

最初のラウンドの後、メッセージの 1 つが削除され、別の 1 つのメッセージが既読としてマークされます。 同期の[ 2 回目のラウンド](#synchronize-messages-in-the-same-folder-in-the-next-round)では、変更されていない他のメッセージは返さず、デルタ (削除と更新) のみを返します。

### <a name="sample-initial-request"></a>最初の要求のサンプル

この例では、指定されたフォルダーは初めて同期されるため、最初の同期要求には状態トークンは含まれません。このラウンドは、そのフォルダー内のすべてのメッセージを返します。

最初の要求では、次のものを指定しています。

- 応答の各メッセージの `subject` プロパティ、`sender` プロパティ、`isRead` プロパティを返す `$select` パラメーター。
- [オプションの要求ヘッダー](#optional-request-header)である _odata.maxpagesize_。一度に 2 通のメッセージを返すよう指定しています。

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_1"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$select=subject,sender,isRead HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-initial-response"></a>最初の応答のサンプル

応答には、2 つのメッセージと `@odata.nextLink` 応答ヘッダーが含まれています。`nextLink` URL は、取得するフォルダーにさらにメッセージがあることを示します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "false",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
      "subject": "Holiday promotion sale",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Samantha Booth",
          "address": "samanthab@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAVRMKAAAAA=="
    }
  ]
}
```

### <a name="sample-second-request"></a>2 番目の要求のサンプル

2 番目の要求では、前の応答で返された `nextLink` URL を指定します。最初の要求にあるような同じ `$select` パラメーターを指定する必要はなくなりましたのでご注意ください。これは、`nextLink` URL の `skipToken` によってこのパラメーターがエンコードされて含まれるためです。

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_2"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a>2 番目の応答のサンプル

2 番目の応答は、フォルダーから取得するメッセージがまだあることを示す、フォルダー内の次の 2 つのメッセージと別の `nextLink` を返します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlqfdAAAEfYB+\"",
      "subject": "Microsoft Virtual Academy at Contoso",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Elliot Hyde",
          "address": "elliot-hyde@tailspintoys.com"
        }
      },
      "id": "AQMkADNkNAAAgWkAAAA"
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "New or modified user account information",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Randi Welch",
          "address": "randiw@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAgWJAAAA"
    }
  ]
}
```

### <a name="sample-third-request"></a>3 番目の要求のサンプル

3 番目の要求は、最後の同期要求から返された最新の `nextLink` URL を引き続き使用します。

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailFolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a>3 番目と最後の応答のサンプル

3 番目の応答では、フォルダーに残っている 1 つだけのメッセージと、そのフォルダーの同期が当面の間完了していることを示す `deltaLink` URL が返されます。`deltaLink` URL を保存して、[次のラウンドで同じフォルダーを同期するために使用します](#synchronize-messages-in-the-same-folder-in-the-next-round)。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzFPjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "Fabric CDN now available",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Jodie Sharp",
          "address": "Jodie.Sharp@contoso.com"
        }
      },
      "id": "AAMkADk0MGFkODE3LWEAAA="
    }
  ]
}
```

### <a name="synchronize-messages-in-the-same-folder-in-the-next-round"></a>次のラウンドで同じフォルダー内のメッセージを同期する

最後のランドの[最後の応答](#sample-third-request)からの `deltaLink` を使用すると、それ以降にそのフォルダーで (追加、削除、または更新によって) 変更されたこれらのメッセージのみを取得できます。次のラウンドの最初の要求は、同じ最大ページ サイズを維持することを前提とすると、次のようになります。

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_next"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```

応答には `deltaLink` が含まれます。 これは、リモート メール フォルダー内のすべての変更が同期されていることを示します。 1 つのメッセージは削除され、その他のメッセージは変更されました。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS0Dh_6qB-pB2Sa2pUum19a6YAAKnLuxoAAA=",
      "@removed": {
        "reason": "deleted"
      }
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    }
  ]
}
```

## <a name="see-also"></a>関連項目

- [Microsoft Graph デルタ クエリ](delta_query_overview.md)
- [カレンダー ビューのイベントへの増分の変更を取得する](delta_query_events.md)
- [グループに対する増分の変更を取得する](delta_query_groups.md)
- [ユーザーへの増分の変更を取得する](delta_query_users.md)
