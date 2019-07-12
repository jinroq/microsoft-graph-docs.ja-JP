---
author: daspek
ms.author: dspektor
title: itemAnalytics リソースの種類
description: ItemAnalytics オブジェクトは、アイテムに対して行われたアクティビティに関する分析を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a18d12bd2b431d147f2d23ea2c958cd75078c9a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620417"
---
# <a name="itemanalytics-resource-type"></a>itemAnalytics リソースの種類

**Itemanalytics**リソースは、アイテムに対して行われたアクティビティに分析を提供します。 このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。

[GetActivitiesByInterval][] API を使用して、カスタムの時間範囲または間隔で分析を取得することもできます。

>**注:****Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。

## <a name="properties"></a>プロパティ

| プロパティ      | 型                 | 説明
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | アイテムの寿命を超えた分析。
| lastSevenDays | [itemActivityStat][] | 過去7日間の分析。

[itemActivityStat]: itemactivitystat.md
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
