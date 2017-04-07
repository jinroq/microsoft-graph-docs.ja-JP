# <a name="workbookrangeview-range"></a>workbookRangeView: range
rangeView リソースに関連付けられている範囲を返します。

### <a name="prerequisites"></a>前提条件
この API を実行するために必要な**スコープ**は、次のとおりです。_Files.Read、Files.ReadWrite_

### <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
### <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Workbook-Session-Id  | 変更を保持するかどうかを決定するブック セッション ID。省略可能。|

### <a name="request-body"></a>要求本文

### <a name="response"></a>応答
成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。

### <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/{ver}/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
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
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
