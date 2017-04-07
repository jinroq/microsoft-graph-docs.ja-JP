# <a name="get-group"></a>グループを取得する

グループ オブジェクトのプロパティとリレーションシップを取得します。

##### <a name="default-properties"></a>既定のプロパティ

以下は、グループを取得または一覧表示するときに返されるプロパティの既定のセットを表します。これらは、利用可能なすべてのプロパティのサブセットです。 

* description
* displayName
* groupTypes
* id
* mail
* mailEnabled
* mailNickname
* onPremisesLastSyncDateTime
* onPremisesSecurityIdentifier
* onPremisesSyncEnabled
* proxyAddresses
* securityEnabled
* visibility

次のグループ プロパティは既定では返されません。

* allowExternalSenders
* autoSubscribeNewMembers
* isSubscribedByMail
* unseenCount

これらのプロパティを取得するには、**$select** クエリ パラメーターを使用します。次に、例を示します。 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1,0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1,0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All* または *Group.ReadWrite.All*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
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
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```
##### <a name="response"></a>応答
以下は、応答の例です。

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しでは、上で示すように既定のプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
