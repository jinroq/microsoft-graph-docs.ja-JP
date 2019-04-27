---
title: workbookChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e12cc2f9a700ef66ec47a72aa88a2c30f2c2c3f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348907"
---
# <a name="workbookchartpoint-resource-type"></a>workbookChartPoint リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフの系列のポイントを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookChartPoint を取得する](../api/chartpoint-get.md) | [workbookChartPoint](workbookchartpoint.md) |chartPoint オブジェクトのプロパティと関係を読み取ります。|
|[List](../api/chartpoint-list.md) | [workbookChartPoint](workbookchartpoint.md)コレクション |chartPoint オブジェクトのコレクションを取得します。 |
|[ItemAt](../api/chartpointscollection-itemat.md)|[workbookChartPoint](workbookchartpoint.md)|データ系列内の位置に基づくポイントを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|value|Json|グラフのポイントの値を返します。 読み取り専用です。|
|id|string|一意識別子|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[workbookChartPointFormat](workbookchartpointformat.md)|グラフのポイントの書式設定プロパティをカプセル化します。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "format"
    ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartPointFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
