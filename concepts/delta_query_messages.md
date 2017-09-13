# <a name="get-incremental-changes-to-messages-in-a-folder"></a><span data-ttu-id="fccf6-101">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="fccf6-101">Get incremental changes to messages in a folder</span></span> 

<span data-ttu-id="fccf6-p101">デルタ クエリでは、一連の[デルタ](../api-reference/v1.0/api/message_delta.md)関数呼び出しを使用して、フォルダー内のメッセージへの追加、削除、または更新に対してクエリを実行できます。デルタ データを使用すると、毎回サーバーからユーザーのメッセージのセット全体をフェッチせずに、ユーザーのメッセージのローカル ストアの保守と同期が行えます。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p101">Delta query lets you query for additions, deletions, or updates to messages in a folder, by way of a series of [delta](../api-reference/v1.0/api/message_delta.md) function calls. Delta data enables you to maintain and synchronize a local store of a user's messages, without having to fetch the entire set of the user's messages from the server every time.</span></span>

<span data-ttu-id="fccf6-p102">デルタ クエリでは、フォルダー内 (ユーザーの受信トレイなど) のすべてのメッセージを取得する完全な同期と、最後の同期以降、そのフォルダー内で変更されたすべてのメッセージを取得する増分同期の両方がサポートされています。通常は、フォルダー内のすべてのメッセージの最初の完全同期を実行して、その後、そのフォルダーの増分の変更を定期的に取得します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p102">Delta query supports both full synchronization that retrieves all of the messages in a folder (for example, the user's Inbox), and incremental synchronization that retrieves all of the messages that have changed in that folder since the last synchronization. Typically, you would do an initial full synchronization of all the messages in a folder, and subsequently, get incremental changes to that folder periodically.</span></span> 

## <a name="track-message-changes-in-a-folder"></a><span data-ttu-id="fccf6-106">フォルダー内のメッセージの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="fccf6-106">Track message changes in a folder</span></span>

<span data-ttu-id="fccf6-p103">デルタ クエリはフォルダー単位の操作です。フォルダー階層内のメッセージの変更を追跡するには、各フォルダーを個別に追跡する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p103">Delta query is a per-folder operation. To track the changes of the messages in a folder hierarchy, you need to track each folder individually.</span></span> 

<span data-ttu-id="fccf6-p104">通常、メール フォルダー内のメッセージ変更の追跡は、**デルタ**関数を使用した、1 つ以上の GET 要求のラウンドです。最初の GET 要求は、**デルタ**関数を含めることを除いて、[メッセージの取得](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages)方法とほぼ同じです。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p104">Tracking message changes in a mail folder typically is a round of one or more GET requests with the **delta** function. The initial GET request is very much like the way you [get messages](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), except that you include the **delta** function:</span></span>

```
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

<span data-ttu-id="fccf6-111">**デルタ**関数を使用した GET 要求は、次のいずれかを返します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-111">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="fccf6-112">`nextLink` (**デルタ**関数の呼び出しと _skipToken_ を使用した URL を含む)、または</span><span class="sxs-lookup"><span data-stu-id="fccf6-112">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="fccf6-113">`deltaLink` (**デルタ**関数の呼び出しと _deltaToken_ を使用した URL を含む)。</span><span class="sxs-lookup"><span data-stu-id="fccf6-113">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="fccf6-p105">これらのトークンは、クライアントに対して完全に不透明な[状態トークン](delta_query_overview.md#state-tokens)です。変更追跡のラウンドを続行する手順は、最後の GET 要求から返された URL を、同じフォルダーの次の**デルタ**関数呼び出しにコピーして適用するだけです。応答で返される `deltaLink` は、変更追跡の現在のラウンドが完了したことを示します。`deltaLink` URL を保存して、次のラウンドを開始する際に使用することができます。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p105">These tokens are [state tokens](delta_query_overview.md#state-tokens) that are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the URL returned from the last GET request to the next **delta** function call for the same folder. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="fccf6-118">`nextLink` と `deltaLink` の URL を使用する方法については、以下の[例](#example-to-synchronize-messages-in-a-folder)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fccf6-118">See the [example](#example-to-synchronize-messages-in-a-folder) below to learn how to use the `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a><span data-ttu-id="fccf6-119">メッセージのデルタ クエリでクエリ パラメーターを使用する</span><span class="sxs-lookup"><span data-stu-id="fccf6-119">Use query parameters in a delta query for messages</span></span>

- <span data-ttu-id="fccf6-p106">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="fccf6-122">デルタ クエリは、メッセージの `$select`、`$top`、および `$expand` をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fccf6-122">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="fccf6-123">`$filter` と `$orderby` に対するサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="fccf6-123">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="fccf6-124">サポートされている唯一の `$filter` 式は、`$filter=receivedDateTime+ge+{value}` または `$filter=receivedDateTime+gt+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="fccf6-124">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="fccf6-p107">サポートされている唯一の `$orderby` 式は、`$orderby=receivedDateTime+desc` です。`$orderby` 式を含めない場合、戻り値の順序は保証されません。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="fccf6-127">`$search` に対するサポートはありません。</span><span class="sxs-lookup"><span data-stu-id="fccf6-127">There is no support for `$search`.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="fccf6-128">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fccf6-128">Optional request header</span></span>

<span data-ttu-id="fccf6-p108">各デルタ クエリの GET 要求は、応答で 1 つ以上のメッセージのコレクションを返します。必要に応じて、要求ヘッダー _Prefer: odata.maxpagesize={x}_ を指定して、応答内の最大メッセージ数を設定できます。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p108">Each delta query GET request returns a collection of one or more messages in the response. You can optionally specify the request header, _Prefer: odata.maxpagesize={x}_, to set the maximum number of messages in a response.</span></span>

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

6. When you eventually receive a _detlaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This 
round of change tracking is complete. 

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request 
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated) 
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a><span data-ttu-id="fccf6-131">ファルダー内のメッセージを同期する例</span><span class="sxs-lookup"><span data-stu-id="fccf6-131">Example to synchronize messages in a folder</span></span>

<span data-ttu-id="fccf6-132">次の例では、5 通のメッセージが含まれる特定のフォルダーを同期するための一連の 3 つの要求を示します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-132">The following example shows a series of 3 requests to synchronize a specific folder which contains 5 messages:</span></span>

- <span data-ttu-id="fccf6-133">[サンプルの最初の要求](#sample-initial-request)と[応答](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="fccf6-133">[Sample initial request](#sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="fccf6-134">[サンプルの 2 番目の要求](#sample-second-request)と[応答](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="fccf6-134">[Sample second request](#sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="fccf6-135">[サンプルの 3 番目の要求](#sample-third-request)と[最後の応答](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="fccf6-135">[Sample third request](#sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="fccf6-136">[次のラウンド](#the-next-round)で行う操作も参照してください。</span><span class="sxs-lookup"><span data-stu-id="fccf6-136">See also what you'll do in the [next round](#the-next-round).</span></span>


### <a name="sample-initial-request"></a><span data-ttu-id="fccf6-137">最初の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="fccf6-137">Sample initial request</span></span>

<span data-ttu-id="fccf6-p109">この例では、指定されたフォルダーは初めて同期されるため、最初の同期要求には状態トークンは含まれません。このラウンドは、そのフォルダー内のすべてのメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p109">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the messages in that folder.</span></span>

<span data-ttu-id="fccf6-140">最初の要求では、次を指定します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-140">The first request specifies the following:</span></span>

- <span data-ttu-id="fccf6-141">応答の各メッセージの **Subject** プロパティと **Sender** プロパティを返す `$select` パラメーター。</span><span class="sxs-lookup"><span data-stu-id="fccf6-141">A `$select` parameter to return the **Subject** and **Sender** properties for each message in the response.</span></span>
- <span data-ttu-id="fccf6-142">[オプションの要求ヘッダー](#optional-request-header)である _odata.maxpagesize_ が一度に 2 通のメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-142">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 messages at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_1"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$select=Subject,Sender HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a><span data-ttu-id="fccf6-143">最初の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="fccf6-143">Sample initial response</span></span>

<span data-ttu-id="fccf6-p110">応答には、2 つのメッセージと `@odata.nextLink` 応答ヘッダーが含まれています。`nextLink` URL は、取得するフォルダーにさらにメッセージがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p110">The response includes two messages and an `@odata.nextLink` response header. The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
            "subject":"Holiday hours update",
            "sender":{
                "emailAddress":{
                    "name":"Dana Swope",
                    "address":"danas@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADNkNAAASq35xAAA="
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
            "subject":"Holiday promotion sale",
            "sender":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAVRMKAAAAA=="
        }
    ]
}
```

### <a name="sample-second-request"></a><span data-ttu-id="fccf6-146">2 番目の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="fccf6-146">Sample second request</span></span>

<span data-ttu-id="fccf6-p111">2 番目の要求では、前の応答で返された `nextLink` URL を指定します。最初の要求にあるような同じ `$select` パラメーターを指定する必要はなくなりましたのでご注意ください。これは、`nextLink` URL の `skipToken` によってこのパラメーターがエンコードされて含まれるためです。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same `$select` parameter as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_2"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="fccf6-149">2 番目の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="fccf6-149">Sample second response</span></span> 

<span data-ttu-id="fccf6-150">2 番目の応答は、フォルダーから取得するメッセージがまだあることを示す、フォルダー内の次の 2 つのメッセージと別の `nextLink` を返します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-150">The second response returns the next 2 messages in the folder and another `nextLink`, indicating there are more messages to get from the folder.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWJAAAA"
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB9\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWHAAAA"
        }
    ]
}
```


### <a name="sample-third-request"></a><span data-ttu-id="fccf6-151">3 番目の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="fccf6-151">Sample third request</span></span>

<span data-ttu-id="fccf6-152">3 番目の要求は、最後の同期要求から返された最新の `nextLink` URL を引き続き使用します。</span><span class="sxs-lookup"><span data-stu-id="fccf6-152">The third request continues to use the latest `nextLink` URL returned from the last sync request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="fccf6-153">3 番目と最後の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="fccf6-153">Sample third and final response</span></span>

<span data-ttu-id="fccf6-p112">3 番目の応答では、フォルダーに残っている 1 つだけのメッセージと、そのフォルダーの同期が当面の間完了していることを示す `deltaLink` URL が返されます。`deltaLink` URL を保存して、[次のラウンドで同じフォルダーを同期するために使用します](#the-next-round)。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p112">The third response returns the only remaining message in the folder, and a `deltaLink` URL which indicates synchronization is complete for the time being for this folder. Save and use the `deltaLink` URL to [synchronize the same folder in the next round](#the-next-round).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB8\"",
            "subject":"You've joined the Customer Manager group",
            "sender":{
                "emailAddress":{
                    "name":"Customer Managers team",
                    "address":"customer_managers@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWFAAAA"
        }
    ]
}
```


### <a name="the-next-round"></a><span data-ttu-id="fccf6-156">次のラウンド</span><span class="sxs-lookup"><span data-stu-id="fccf6-156">The next round</span></span>

<span data-ttu-id="fccf6-p113">最後のランドの[最後の応答](#sample-third-request)からの `deltaLink` を使用すると、それ以降にそのフォルダーで (追加、削除、または更新によって) 変更されたこれらのメッセージのみを取得できます。次のラウンドの最初の要求は、同じ最大ページ サイズを維持することを前提とすると、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="fccf6-p113">Using the `deltaLink` from the [last request](#sample-third-request) in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_next"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```



## <a name="see-also"></a><span data-ttu-id="fccf6-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="fccf6-159">See also</span></span>

- [<span data-ttu-id="fccf6-160">Microsoft Graph デルタ クエリ</span><span class="sxs-lookup"><span data-stu-id="fccf6-160">Microsoft Graph delta query</span></span>](../Concepts/delta_query_overview.md)
- [<span data-ttu-id="fccf6-161">カレンダー ビューのイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="fccf6-161">Get incremental changes to events in a calendar view</span></span>](../Concepts/delta_query_events.md)
- [<span data-ttu-id="fccf6-162">グループに対する増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="fccf6-162">Get incremental changes to groups</span></span>](../Concepts/delta_query_groups.md)
- [<span data-ttu-id="fccf6-163">ユーザーに対する増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="fccf6-163">Get incremental changes to users</span></span>](../Concepts/delta_query_users.md)
