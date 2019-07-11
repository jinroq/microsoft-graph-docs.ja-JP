---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 862b0b14f1efeb3a83dd4b842c0eb995abeabb80
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620263"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="ba8f8-102">itemAnalytics リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba8f8-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba8f8-103">**Itemanalytics**リソースは、アイテムに対して行われたアクティビティに分析を提供します。</span><span class="sxs-lookup"><span data-stu-id="ba8f8-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="ba8f8-104">このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ba8f8-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="ba8f8-105">[GetActivitiesByInterval][] API を使用して、カスタムの時間範囲または間隔で分析を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="ba8f8-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="ba8f8-106">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="ba8f8-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba8f8-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba8f8-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ba8f8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba8f8-108">Properties</span></span>

| <span data-ttu-id="ba8f8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba8f8-109">Property</span></span>      | <span data-ttu-id="ba8f8-110">型</span><span class="sxs-lookup"><span data-stu-id="ba8f8-110">Type</span></span>                 | <span data-ttu-id="ba8f8-111">説明</span><span class="sxs-lookup"><span data-stu-id="ba8f8-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="ba8f8-112">allTime</span><span class="sxs-lookup"><span data-stu-id="ba8f8-112">allTime</span></span>       | <span data-ttu-id="ba8f8-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="ba8f8-113">[itemActivityStat][]</span></span> | <span data-ttu-id="ba8f8-114">アイテムの寿命を超えた分析。</span><span class="sxs-lookup"><span data-stu-id="ba8f8-114">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="ba8f8-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="ba8f8-115">lastSevenDays</span></span> | <span data-ttu-id="ba8f8-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="ba8f8-116">[itemActivityStat][]</span></span> | <span data-ttu-id="ba8f8-117">過去7日間の分析。</span><span class="sxs-lookup"><span data-stu-id="ba8f8-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


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
