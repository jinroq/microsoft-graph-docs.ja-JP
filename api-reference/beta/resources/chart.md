---
title: グラフ リソースの種類
description: ブック内のグラフ オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643235"
---
# <a name="chart-resource-type"></a>グラフ リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ブック内のグラフ オブジェクトを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get Chart](../api/chart-get.md) | [Chart](chart.md) |グラフ オブジェクトのプロパティと関係を読み取ります。|
|[ChartSeries を作成する](../api/chart-post-series.md) |[ChartSeries](chartseries.md)| データ系列のコレクションに投稿して、新しい ChartSeries を作成します。|
|[データ系列を一覧表示する](../api/chart-list-series.md) |[ChartSeries](chartseries.md) コレクション| ChartSeries オブジェクトのコレクションを取得します。|
|[更新する](../api/chart-update.md) | [Chart](chart.md)   |グラフ オブジェクトを更新します。 |
|[Image](../api/chart-image.md)|Base64 でエンコードされた文字列の画像|指定したサイズに合わせてグラフを拡大・縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。|
|[削除する](../api/chart-delete.md)|なし|グラフ オブジェクトを削除します。|
|[Setdata](../api/chart-setdata.md)|なし|グラフの元データをリセットします。|
|[Setposition](../api/chart-setposition.md)|なし|ワークシート上のセルを基準にしてグラフを配置します。|
|[List](../api/chart-list.md) | [Chart](chart.md) コレクション |グラフ オブジェクトのコレクションを取得します。 |
|[Itemat](../api/chartcollection-itemat.md)|[Chart](chart.md)|コレクション内の位置に基づいて、グラフを取得します。|
|[Add](../api/chartcollection-add.md)|[Chart](chart.md)|新しいグラフを作成します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|height|double|グラフ オブジェクトの高さをポイント単位で表します。|
|id|文字列|コレクション内での位置を基にグラフを取得します。読み取り専用です。|
|left|double|グラフの左側からワークシートの原点までの距離 (ポイント単位)。|
|name|文字列| グラフ オブジェクトの名前を表します。|
|top|double|オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。|
|width|double|グラフ オブジェクトの幅をポイント単位で表します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|axes|[ChartAxes](chartaxes.md)|グラフの軸を表します。値の取得のみ可能です。|
|dataLabels|[ChartDataLabels](chartdatalabels.md)|グラフのデータラベルを表します。値の取得のみ可能です。|
|format|[ChartAreaFormat](chartareaformat.md)|グラフ領域の書式設定プロパティをカプセル化します。値の取得のみ可能です。|
|legend|[ChartLegend](chartlegend.md)|グラフの凡例を表します。値の取得のみ可能です。|
|series|[ChartSeries](chartseries.md) コレクション|グラフの 1 つのデータ系列またはデータ系列のコレクションを表します。値の取得のみ可能です。|
|役職|[ChartTitle](charttitle.md)|指定したグラフのタイトル (タイトルのテキスト、表示/非表示、位置、書式設定など) を表します。値の取得のみ可能です。|
|worksheet|[Worksheet](worksheet.md)|現在のグラフを含んでいるワークシート。読み取り専用。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
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
<!--
{
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
