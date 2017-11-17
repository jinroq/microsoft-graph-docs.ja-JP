# <a name="chartaxis-resource-type"></a>ChartAxis リソースの種類

グラフの 1 つの軸を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartAxis](../api/chartaxis_get.md) | [ChartAxis](chartaxis.md) |chartAxis オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartaxis_update.md) | [ChartAxis](chartaxis.md)    |ChartAxis オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|majorUnit|オブジェクト|2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。|
|maximum|object|数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|
|minimum|object|数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|
|minorUnit|オブジェクト|2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|format|[ChartAxisFormat](chartaxisformat.md)|グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。|
|majorGridlines|[ChartGridlines](chartgridlines.md)|指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。|
|minorGridlines|[ChartGridlines](chartgridlines.md)|指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。|
|title|[ChartAxisTitle](chartaxistitle.md)|軸タイトルを表します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->