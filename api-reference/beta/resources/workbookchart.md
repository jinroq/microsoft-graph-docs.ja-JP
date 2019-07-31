---
title: workbookChart リソースの種類
description: ブック内のグラフ オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c180d6d2649f7c55868ffa04a5318c5c5f522ddd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007383"
---
# <a name="workbookchart-resource-type"></a>workbookChart リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ブック内のグラフ オブジェクトを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get Chart](../api/chart-get.md) | [workbookChart](workbookchart.md) |グラフ オブジェクトのプロパティと関係を読み取ります。|
|[ChartSeries を作成する](../api/chart-post-series.md) |[workbookChartSeries](workbookchartseries.md)| データ系列のコレクションに投稿して、新しい ChartSeries を作成します。|
|[データ系列を一覧表示する](../api/chart-list-series.md) |[workbookChartSeries](workbookchartseries.md)コレクション| ChartSeries オブジェクトのコレクションを取得します。|
|[Update](../api/chart-update.md) | [workbookChart](workbookchart.md)   |グラフ オブジェクトを更新します。 |
|[Image](../api/chart-image.md)|Base64 でエンコードされた文字列の画像|指定したサイズに合わせてグラフを拡大・縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。|
|[Delete](../api/chart-delete.md)|None|グラフ オブジェクトを削除します。|
|[Setdata](../api/chart-setdata.md)|None|グラフの元データをリセットします。|
|[Setposition](../api/chart-setposition.md)|なし|ワークシート上のセルを基準にしてグラフを配置します。|
|[List](../api/chart-list.md) | [workbookChart](workbookchart.md)コレクション |グラフ オブジェクトのコレクションを取得します。 |
|[Itemat](../api/chartcollection-itemat.md)|[workbookChart](workbookchart.md)|コレクション内での位置を基にグラフを取得します。|
|[Add](../api/chartcollection-add.md)|[workbookChart](workbookchart.md)|新しいグラフを作成します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|height|double|グラフ オブジェクトの高さをポイント単位で表します。|
|id|string|コレクション内での位置を基にグラフを取得します。読み取り専用です。|
|left|double|グラフの左側からワークシートの原点までの距離 (ポイント単位)。|
|name|string|グラフ オブジェクトの名前を表します。|
|top|double|オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。|
|width|double|グラフ オブジェクトの幅をポイント単位で表します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|axes|[workbookChartAxes](workbookchartaxes.md)|グラフの軸を表します。値の取得のみ可能です。|
|dataLabels|[workbookChartDataLabels](workbookchartdatalabels.md)|グラフのデータラベルを表します。値の取得のみ可能です。|
|format|[workbookChartAreaFormat](workbookchartareaformat.md)|グラフ領域の書式設定プロパティをカプセル化します。値の取得のみ可能です。|
|legend|[workbookChartLegend](workbookchartlegend.md)|グラフの凡例を表します。値の取得のみ可能です。|
|series|[workbookChartSeries](workbookchartseries.md)コレクション|グラフの 1 つのデータ系列またはデータ系列のコレクションを表します。値の取得のみ可能です。|
|title|[workbookChartTitle](workbookcharttitle.md)|指定したグラフのタイトル (タイトルのテキスト、表示/非表示、位置、書式設定など) を表します。値の取得のみ可能です。|
|worksheet|[workbookWorksheet](workbookworksheet.md)|現在のグラフを含んでいるワークシート。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
