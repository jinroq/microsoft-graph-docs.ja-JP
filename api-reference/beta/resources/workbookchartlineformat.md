---
title: workbookChartLineFormat リソースの種類
description: 直線要素の書式設定オプションをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b40c72240771edd3517f2b29df269d83adeec8f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348886"
---
# <a name="workbookchartlineformat-resource-type"></a>workbookChartLineFormat リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

直線要素の書式設定オプションをカプセル化します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookChartLineFormat を取得する](../api/chartlineformat-get.md) | [workbookChartLineFormat](workbookchartlineformat.md) |chartLineFormat オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/chartlineformat-update.md) | [workbookChartLineFormat](workbookchartlineformat.md) |ChartLineFormat オブジェクトを更新します。 |
|[Clear](../api/chartlineformat-clear.md)|なし|グラフ要素の線の書式をクリアします。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|color|string|グラフの線の色を表す HTML カラー コード。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
