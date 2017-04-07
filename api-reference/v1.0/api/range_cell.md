# <a name="range-cell"></a>範囲:セル

行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。
## <a name="prerequisites"></a>前提条件
この API を実行するために必要な**スコープ**は、次のとおりです。 
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/Cell
POST /workbook/worksheets(<id|name>)/range(<address>)/Cell
POST /workbook/tables(<id|name>)/columns(<id|name>)/range/Cell

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer <code>|


## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター       | 型    |説明|
|:---------------|:--------|:----------|
|row|number|取得するセルの行番号。0 を起点とする番号になります。|
|column|number|取得セルの列番号。0 を起点とする番号になります。|

## <a name="response"></a>応答
成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->