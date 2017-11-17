# <a name="chartaxistitle-resource-type"></a>ChartAxisTitle リソースの種類

グラフ軸のタイトルを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartAxisTitle](../api/chartaxistitle_get.md) | [ChartAxisTitle](chartaxistitle.md) |chartAxisTitle オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartaxistitle_update.md) | [ChartAxisTitle](chartaxistitle.md)    |ChartAxisTitle オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|text|string|軸タイトルを表します。|
|visible|boolean|軸のタイトルの表示/非表示を指定するブール型の値です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|format|[ChartAxisTitleFormat](chartaxistitleformat.md)|グラフ軸のタイトルの書式設定を表します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->