---
author: daspek
ms.author: dspektor
title: itemAnalytics リソースの種類
description: ItemAnalytics オブジェクトは、アイテムに対して行われたアクティビティに関する分析を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5c716f8faaafffe6afd75987843e6b614f5d6552
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970755"
---
# <a name="itemanalytics-resource-type"></a>itemAnalytics リソースの種類

**Itemanalytics**リソースは、アイテムに対して行われたアクティビティに分析を提供します。 このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。

[GetActivitiesByInterval][] API を使用して、カスタムの時間範囲または間隔で分析を取得することもできます。

>**注:****Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。

## <a name="properties"></a>プロパティ

| プロパティ      | 型                 | 説明
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemactiv][] | アイテムの寿命を超えた分析。
| lastSevenDays | [itemactiv][] | 過去7日間の分析。

[itemactiv]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```
<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": []
}
-->
