---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemanalytics
localization_priority: Normal
ms.openlocfilehash: 2869655b3b645fc8d30ceec3867c28ca81ac9d51
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345457"
---
# <a name="itemanalytics-resource-type"></a>itemanalytics リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**itemanalytics**リソースは、アイテムに対して行われたアクティビティに分析を提供します。 このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。

[getActivitiesByInterval][] API を使用して、カスタムの時間範囲または間隔で分析を取得することもできます。

>**注:****itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。

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

## <a name="properties"></a>プロパティ

| プロパティ      | 型                 | 説明
|:--------------|:---------------------|:--------------------------------------
| alltime       | [itemactiv][] | アイテムの寿命を超えた分析。
| lastSevenDays | [itemactiv][] | 過去7日間の分析。

[itemactiv]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

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
