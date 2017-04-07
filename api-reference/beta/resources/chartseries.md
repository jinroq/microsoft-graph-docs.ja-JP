# <a name="chartseries-resource-type"></a>ChartSeries リソースの種類

グラフのデータ系列を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries_get.md) | [ChartSeries](chartseries.md) |chartSeries オブジェクトのプロパティと関係を読み取ります。|
|[ChartPoints を作成する](../api/chartseries_post_points.md) |[ChartPoints](chartpoint.md)| ポイント コレクションに投稿して、新しい ChartPoints を作成します。|
|[ポイントを一覧表示する](../api/chartseries_list_points.md) |[ChartPoints](chartpoint.md) コレクション| ChartPoints オブジェクトのコレクションを取得します。|
|[Update](../api/chartseries_update.md) | [ChartSeries](chartseries.md)    |ChartSeries オブジェクトを更新します。 |
|[List](../api/chartseries_list.md) | [ChartSeries](chartseries.md) コレクション |chartSeries オブジェクトのコレクションを取得します。 |
|[Itemat](../api/chartseriescollection_itemat.md)|[ChartSeries](chartseries.md)|コレクション内の位置に基づいてデータ系列を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|name|string|グラフのデータ系列の名前を表します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|format|[ChartSeriesFormat](chartseriesformat.md)|グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。|
|points|[ChartPoints](chartpoint.md) コレクション|データ系列にあるすべてのポイントのコレクションを返します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->