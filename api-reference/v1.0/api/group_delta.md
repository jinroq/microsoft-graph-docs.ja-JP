# <a name="group-delta"></a>グループ：デルタ
[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用すると、アプリケーションは、要求ごとにターゲット リソースをすべて読み取ることなく、新しく作成、更新、削除されたエンティティを検出できます。グループへの変更を検出するには、*デルタ*関数を使用して要求を実行します。詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.Read.All、Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.Read.All、Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

## <a name="query-parameters"></a>クエリ パラメーター
グループで変更の追跡を実行するときには、1 つまたは複数の **delta** 関数の呼び出しが必要になります。クエリ パラメーター (`$deltatoken` および `$skiptoken` 以外) を使用する場合は、そのパラメーターを最初の **delta** 要求に指定する必要があります。指定されたパラメーターは、Microsoft Graph を使って自動的にエンコードされ、応答の `nextLink` または `deltaLink` URL のトークン部分として指定されます。

必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。

その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。

| クエリ パラメーター      | 種類   |説明|
|:---------------|:--------|:----------|
| $deltatoken | 文字列 | 同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。|
| $skiptoken | 文字列 | 前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。 |

### <a name="odata-query-parameters"></a>OData クエリ パラメーター
このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。

- 任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。
- デルタ クエリは、グループの `$select`、`$top`、`$expand` をサポートします。
- と `$orderby` に対するサポートには制限があります。`$filter`
  * サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。 複数のオブジェクトをフィルター処理することができます。 たとえば、`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff` などです。 フィルター処理されるオブジェクトには 50 の数量制限があります。
- はサポートされていません。`$search`

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| 承認  | ベアラー&lt;トークン&gt;|
| コンテンツタイプ  | アプリケーション /json |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。応答には、状態トークン (nextLink URL や deltaLink URL) も含まれます。

- nextLink URL が返される場合は、セッションに取得するデータの追加ページがあります。deltaLink URL が応答で返されるまで、アプリケーションは nextLink URL を使用して要求を実行し続けます。

- deltaLink URL が返される場合、返されるリソースの既存の状態に関するデータはありません。以降の要求では、アプリケーションは deltaLink URL を使用して、リソースへの変更点を確認します。

参照先:</br>
- 詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください</br>
- [ グループに対する増分の変更を取得する](../../../concepts/delta_query_groups.md)</br>

## <a name="example"></a>例
#### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response"></a>応答
応答の例を次に示します。
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
>
> グループ内のメンバー オブジェクトの id が含まれている *members@delta* プロパティが存在することに注意してください。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="see-also"></a>関連項目
- 詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください
- [ グループに対する増分の変更を取得する](../../../concepts/delta_query_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
