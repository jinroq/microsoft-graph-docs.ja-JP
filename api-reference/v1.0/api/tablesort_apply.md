# <a name="tablesort-apply"></a>TableSort: apply　

並べ替え操作を実行します。
## <a name="prerequisites"></a>前提条件
この API を実行するために必要な**スコープ**は、次のとおりです。 
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables(<id|name>)/sort/apply
POST /workbook/worksheets(<id|name>)/tables(<id|name>)/sort/apply

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer <code>|


## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター       | 型    |説明|
|:---------------|:--------|:----------|
|fields|SortField|並べ替えに使用する条件の一覧。|
|matchCase|boolean|省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。|
|method|string|省略可能。中国語文字に使用される順序付けの方法です。可能な値は、`PinYin`、`StrokeCount` です。|

## <a name="response"></a>応答
成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables(<id|name>)/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a>応答
以下は、応答の例です。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->