---
title: グラフ リソースの種類
description: ブック内のグラフ オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4f412894ffaef07908a41f8f7cc15ab3a52331af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873403"
---
# <a name="chart-resource-type"></a>グラフ リソースの種類

ブック内のグラフ オブジェクトを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get Chart](../api/chart-get.md) | [WorkbookChart](chart.md) |グラフ オブジェクトのプロパティと関係を読み取ります。|
|[ChartSeries を作成する](../api/chart-post-series.md) |[WorkbookChartSeries](chartseries.md)| データ系列のコレクションに投稿して、新しい ChartSeries を作成します。|
|[データ系列を一覧表示する](../api/chart-list-series.md) |[WorkbookChartSeries](chartseries.md)コレクション| ChartSeries オブジェクトのコレクションを取得します。|
|[Update](../api/chart-update.md) | [WorkbookChart](chart.md)   |グラフ オブジェクトを更新します。 |
|[Image](../api/chart-image.md)|Base64 でエンコードされた文字列の画像|指定したサイズに合わせてグラフを拡大・縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。|
|[Delete](../api/chart-delete.md)|なし|グラフ オブジェクトを削除します。|
|[Setdata](../api/chart-setdata.md)|なし|グラフの元データをリセットします。|
|[Setposition](../api/chart-setposition.md)|なし|ワークシート上のセルを基準にしてグラフを配置します。|
|[List](../api/chart-list.md) | [WorkbookChart](chart.md)コレクション |グラフ オブジェクトのコレクションを取得します。 |
|[Itemat](../api/chartcollection-itemat.md)|[WorkbookChart](chart.md)|コレクション内での位置を基にグラフを取得します。|
|[Add](../api/chartcollection-add.md)|[WorkbookChart](chart.md)|新しいグラフを作成します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|height|double|グラフ オブジェクトの高さをポイント単位で表します。|
|ID|文字列|コレクション内での位置を基にグラフを取得します。読み取り専用です。|
|left|double|グラフの左側からワークシートの原点までの距離 (ポイント単位)。|
|name|文字列| グラフ オブジェクトの名前を表します。|
|top|double|オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。|
|width|double|グラフ オブジェクトの幅をポイント単位で表します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|axes|[WorkbookChartAxes](chartaxes.md)|グラフの軸を表します。値の取得のみ可能です。|
|dataLabels|[WorkbookChartDataLabels](chartdatalabels.md)|グラフのデータラベルを表します。値の取得のみ可能です。|
|format|[WorkbookChartAreaFormat](chartareaformat.md)|グラフ領域の書式設定プロパティをカプセル化します。値の取得のみ可能です。|
|legend|[WorkbookChartLegend](chartlegend.md)|グラフの凡例を表します。値の取得のみ可能です。|
|series|[WorkbookChartSeries](chartseries.md)コレクション|グラフの 1 つのデータ系列またはデータ系列のコレクションを表します。値の取得のみ可能です。|
|役職|[WorkbookChartTitle](charttitle.md)|指定したグラフのタイトル (タイトルのテキスト、表示/非表示、位置、書式設定など) を表します。値の取得のみ可能です。|
|worksheet|[WorkbookWorksheet](worksheet.md)|現在のグラフを含んでいるワークシート。読み取り専用。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
