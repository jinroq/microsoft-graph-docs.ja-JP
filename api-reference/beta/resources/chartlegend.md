# <a name="chartlegend-resource-type"></a>ChartLegend リソースの種類

グラフに凡例を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartLegend](../api/chartlegend_get.md) | [ChartLegend](chartlegend.md) |chartLegend オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartlegend_update.md) | [ChartLegend](chartlegend.md)    |ChartLegend オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|overlay|boolean|グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。|
|position|string|グラフの凡例の位置を表します。可能な値は、`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom` です。|
|visible|boolean|ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。|

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|format|[ChartLegendFormat](chartlegendformat.md)|グラフ の凡例の書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->