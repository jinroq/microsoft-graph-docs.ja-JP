# <a name="list-groups"></a>グループを一覧表示する

Office 365 のグループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。各グループの[既定のプロパティ](../api/group_get.md#default-properties)が返されます。

Office 365 グループ (別名統合グループ) のみを一覧表示するには、**groupTypes** にフィルターを適用します。
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

OData クエリ オプション `$orderby` を使用して、以下の例のように、組織内のグループを **displayName** 値で並べ替えることができます。
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```


## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All* または *Group.ReadWrite.All*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。
## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```
##### <a name="response"></a>応答
以下は、応答の例です。

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しでは [既定のプロパティ](../api/group_get.md#default-properties)が返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
