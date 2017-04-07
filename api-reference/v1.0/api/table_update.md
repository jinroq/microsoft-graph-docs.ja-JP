# <a name="update-table"></a>テーブルを更新する

table オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を実行するために必要な**スコープ**は、次のとおりです。 
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables(<id|name>)
PATCH /workbook/worksheets(<id|name>)/tables(<id|name>)
```
## <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | Bearer <code>|


## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|name|string|テーブルの名前。|
|showHeaders|boolean|ヘッダー行を表示するかどうかを示します。この値によって、ヘッダー行の表示または削除を設定できます。|
|showTotals|boolean|集計行を表示するかどうかを示します。この値によって、集計行の表示または削除を設定できます。|
|style|string|テーブル スタイルを表す定数値。使用可能な値は次のとおりです。TableStyleLight1 から TableStyleLight21、TableStyleMedium1 から TableStyleMedium28、TableStyleStyleDark1 から TableStyleStyleDark11。ブックに存在するカスタムのユーザー定義スタイルも指定できます。|

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [Table](../resources/table.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables(<id|name>)
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
