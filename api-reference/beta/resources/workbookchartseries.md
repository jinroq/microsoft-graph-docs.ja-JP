---
title: workbookChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e9ff478a5f7e91c3d116ca2dbd78e20699077aab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348885"
---
# <a name="workbookchartseries-resource-type"></a>workbookChartSeries リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフのデータ系列を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [workbookChartSeries](workbookchartseries.md) |chartSeries オブジェクトのプロパティと関係を読み取ります。|
|[chartpoint を作成する](../api/chartseries-post-points.md) |[chartPoints](workbookchartpoint.md)| points コレクションへの投稿によって、新しい chartpoint を作成します。|
|[ポイントを一覧表示する](../api/chartseries-list-points.md) |[workbookChartPoints](workbookchartpoint.md)コレクション| chartpoints オブジェクトのコレクションを取得します。|
|[更新する](../api/chartseries-update.md) | [workbookChartSeries](workbookchartseries.md) |chartseries オブジェクトを更新します。 |
|[List](../api/chartseries-list.md) | [workbookChartSeries](workbookchartseries.md)コレクション |chartSeries オブジェクトのコレクションを取得します。 |
|[ItemAt](../api/chartseriescollection-itemat.md)|[workbookChartSeries](workbookchartseries.md)|コレクション内の位置に基づいてデータ系列を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|name|string|グラフのデータ系列の名前を表します。|

## <a name="relationships"></a>関係
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
