# <a name="chartlineformat-resource-type"></a>ChartLineFormat リソースの種類

直線要素の書式設定オプションをカプセル化します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartLineFormat](../api/chartlineformat_get.md) | [ChartLineFormat](chartlineformat.md) |chartLineFormat オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartlineformat_update.md) | [ChartLineFormat](chartlineformat.md)    |ChartLineFormat オブジェクトを更新します。 |
|[Clear](../api/chartlineformat_clear.md)|なし|グラフ要素の線の書式をクリアします。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|color|string|グラフの線の色を表す HTML カラー コード。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
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
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->