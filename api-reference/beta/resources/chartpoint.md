# <a name="chartpoint-resource-type"></a>ChartPoint リソースの種類

グラフの系列のポイントを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartPoint](../api/chartpoint_get.md) | [ChartPoint](chartpoint.md) |chartPoint オブジェクトのプロパティと関係を読み取ります。|
|[List](../api/chartpoint_list.md) | [ChartPoint](chartpoint.md) コレクション |chartPoint オブジェクトのコレクションを取得します。 |
|[Itemat](../api/chartpointscollection_itemat.md)|[ChartPoint](chartpoint.md)|データ系列内の位置に基づくポイントを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|value|object|グラフのポイントの値を返します。値の取得のみ可能です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|format|[ChartPointFormat](chartpointformat.md)|グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->