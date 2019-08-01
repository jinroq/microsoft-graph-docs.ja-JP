---
title: ChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4ecdc4c6f249b6783b023d0a69832a9415fc8549
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032915"
---
# <a name="chartseries-resource-type"></a>ChartSeries リソースの種類

グラフのデータ系列を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [WorkbookChartSeries](chartseries.md) |chartSeries オブジェクトのプロパティと関係を読み取ります。|
|[ChartPoints を作成する](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| ポイント コレクションに投稿して、新しい ChartPoints を作成します。|
|[ポイントを一覧表示する](../api/chartseries-list-points.md) |[ChartPoints](chartpoint.md) コレクション| ChartPoints オブジェクトのコレクションを取得します。|
|[Update](../api/chartseries-update.md) | [WorkbookChartSeries](chartseries.md) |ChartSeries オブジェクトを更新します。 |
|[List](../api/chartseries-list.md) | [WorkbookChartSeries](chartseries.md)コレクション |chartSeries オブジェクトのコレクションを取得します。 |
|[ItemAt](../api/chartseriescollection-itemat.md)|[WorkbookChartSeries](chartseries.md)|コレクション内の位置に基づいてデータ系列を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|name|string|グラフのデータ系列の名前を表します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[WorkbookChartSeriesFormat](chartseriesformat.md)|グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。|
|points|[WorkbookChartPoint](chartpoint.md)コレクション|データ系列にあるすべてのポイントのコレクションを返します。 読み取り専用です。|

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
