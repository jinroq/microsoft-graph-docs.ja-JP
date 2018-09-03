# <a name="rangefill-resource-type"></a>RangeFill リソースの種類

範囲オブジェクトの背景を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[RangeFill を取得する](../api/rangefill_get.md) | [WorkbookRangeFill](rangefill.md) |rangeFill オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/rangefill_update.md) | [WorkbookRangeFill](rangefill.md)   |RangeFill オブジェクトを更新します。 |
|[クリア](../api/rangefill_clear.md)|なし|範囲の背景をリセットします。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|color|文字列|枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->