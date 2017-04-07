# <a name="range-merge"></a>範囲: マージ

範囲内のセルをワークシートの 1 つの領域にマージします。
## <a name="prerequisites"></a>前提条件
この API を実行するために必要な**スコープ**は、次のとおりです。 
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets(<id|name>)/range(<address>)/merge
POST /workbook/tables(<id|name>)/columns(<id|name>)/range/merge

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer <code>|


## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター       | 型    |説明|
|:---------------|:--------|:----------|
|across|boolean|省略可能。指定した範囲のセルを行ごとに結合して、行ごとに別のセルを作成する場合は True に設定します。既定値は False です。|

## <a name="response"></a>応答
成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->