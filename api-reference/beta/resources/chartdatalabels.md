# <a name="chartdatalabels-resource-type"></a>ChartDataLabels リソースの種類

グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartDataLabels](../api/chartdatalabels_get.md) | [ChartDataLabels](chartdatalabels.md) |chartDataLabels オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartdatalabels_update.md) | [ChartDataLabels](chartdatalabels.md)    |ChartDataLabels オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|position|string|データ ラベルの位置を表す DataLabelPosition 値。可能な値は、`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout` です。|
|separator|string|グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。|
|showBubbleSize|boolean|データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。|
|showCategoryName|boolean|データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。|
|showLegendKey|boolean|データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。|
|showPercentage|boolean|データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。|
|showSeriesName|boolean|データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。|
|showValue|boolean|データ ラベルの値を表示するか非表示にするかを表すブール型の値。|

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|format|[ChartDataLabelFormat](chartdatalabelformat.md)|グラフのデータ ラベルの書式 (塗りつぶしとフォントの書式設定を含む) を表します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->