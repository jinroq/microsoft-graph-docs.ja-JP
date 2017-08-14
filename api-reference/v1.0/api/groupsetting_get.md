# <a name="get-a-group-setting"></a>グループ設定の取得

特定のグループ設定オブジェクトのプロパティを取得します。

## <a name="prerequisites"></a>前提条件

この API を実行するには、以下のいずれかの**スコープ**が必要です。*Directory.Read.All* または *Directory.ReadWrite.All* または *Directory.AccessAsUser.All*

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->

特定のテナント全体またはグループ設定を取得します。

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。

> 注: $filter はサポートされていません。

## <a name="request-headers"></a>要求ヘッダー
| 名前 | 説明 |
|:----------|:----------|
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupSetting](../resources/groupsetting.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a>応答

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->