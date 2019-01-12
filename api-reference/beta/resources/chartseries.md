---
title: ChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5a299c7140c2032a57cd47fb0880ae34620a920b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915817"
---
# <a name="chartseries-resource-type"></a>ChartSeries リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

グラフのデータ系列を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [ChartSeries](chartseries.md) |chartSeries オブジェクトのプロパティと関係を読み取ります。|
|[ChartPoints を作成する](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| ポイント コレクションに投稿して、新しい ChartPoints を作成します。|
|[ポイントを一覧表示する](../api/chartseries-list-points.md) |[ChartPoints](chartpoint.md) コレクション| ChartPoints オブジェクトのコレクションを取得します。|
|[Update](../api/chartseries-update.md) | [ChartSeries](chartseries.md) |ChartSeries オブジェクトを更新します。 |
|[List](../api/chartseries-list.md) | [ChartSeries](chartseries.md) コレクション |chartSeries オブジェクトのコレクションを取得します。 |
|[Itemat](../api/chartseriescollection-itemat.md)|[ChartSeries](chartseries.md)|コレクション内の位置に基づいてデータ系列を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|name|文字列|グラフのデータ系列の名前を表します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
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
