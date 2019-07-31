---
title: workbookChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c7f7c8108ac17e6705b8bf5f69b0e87f0dc96b31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007250"
---
# <a name="workbookchartseries-resource-type"></a>workbookChartSeries リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフのデータ系列を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [workbookChartSeries](workbookchartseries.md) |chartSeries オブジェクトのプロパティと関係を読み取ります。|
|[ChartPoint を作成する](../api/chartseries-post-points.md) |[chartPoints](workbookchartpoint.md)| Points コレクションへの投稿によって、新しい chartPoint を作成します。|
|[ポイントを一覧表示する](../api/chartseries-list-points.md) |[workbookChartPoints](workbookchartpoint.md)コレクション| ChartPoints オブジェクトのコレクションを取得します。|
|[Update](../api/chartseries-update.md) | [workbookChartSeries](workbookchartseries.md) |ChartSeries オブジェクトを更新します。 |
|[List](../api/chartseries-list.md) | [workbookChartSeries](workbookchartseries.md)コレクション |chartSeries オブジェクトのコレクションを取得します。 |
|[ItemAt](../api/chartseriescollection-itemat.md)|[workbookChartSeries](workbookchartseries.md)|コレクション内の位置に基づいてデータ系列を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|name|string|グラフのデータ系列の名前を表します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[workbookChartSeriesFormat](workbookchartseriesformat.md)|グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。|
|points|[workbookChartPoint](workbookchartpoint.md)コレクション|データ系列にあるすべてのポイントのコレクションを返します。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
