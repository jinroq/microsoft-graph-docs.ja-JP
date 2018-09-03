# <a name="rangeborder-resource-type"></a>RangeBorder リソースの種類

オブジェクトの輪郭を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get RangeBorder](../api/rangeborder_get.md) | [WorkbookRangeBorder](rangeborder.md) |rangeBorder オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/rangeborder_update.md) | [WorkbookRangeBorder](rangeborder.md) |RangeBorder オブジェクトを更新します。 |
|[List](../api/rangeborder_list.md) | [WorkbookRangeBorder](rangeborder.md) コレクション |rangeBorder オブジェクトのコレクションを取得します。 |
|[Itemat](../api/rangebordercollection_itemat.md)|[WorkbookRangeBorder](rangeborder.md)|オブジェクトのインデックスを使用して、罫線オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|color|文字列|枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。|
|id|string|罫線の識別子を表します。 指定できる値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。 読み取り専用。|
|sideIndex|string|罫線の特定の側面を示す定数値です。 指定できる値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。 読み取り専用。|
|style|string|罫線の線スタイルを指定する、線スタイルの定数の 1 つです。 指定できる値は、`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot` です。|
|weight|string|範囲周辺の罫線の太さを指定します。 指定できる値は、  `Hairline`、  `Thin`、  `Medium`、  `Thick` です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->