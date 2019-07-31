---
author: daspek
description: ItemAnalytics リソースは、アイテムに対して行われたアクティビティに分析を提供します。 このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d2be5c7665961248e989101a1a9bd21eb805e6e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967102"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="7e6cf-104">itemAnalytics リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e6cf-104">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e6cf-105">**Itemanalytics**リソースは、アイテムに対して行われたアクティビティに分析を提供します。</span><span class="sxs-lookup"><span data-stu-id="7e6cf-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="7e6cf-106">このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="7e6cf-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="7e6cf-107">[GetActivitiesByInterval][] API を使用して、カスタムの時間範囲または間隔で分析を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="7e6cf-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="7e6cf-108">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="7e6cf-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e6cf-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e6cf-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7e6cf-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e6cf-110">Properties</span></span>

| <span data-ttu-id="7e6cf-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e6cf-111">Property</span></span>      | <span data-ttu-id="7e6cf-112">型</span><span class="sxs-lookup"><span data-stu-id="7e6cf-112">Type</span></span>                 | <span data-ttu-id="7e6cf-113">説明</span><span class="sxs-lookup"><span data-stu-id="7e6cf-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="7e6cf-114">allTime</span><span class="sxs-lookup"><span data-stu-id="7e6cf-114">allTime</span></span>       | <span data-ttu-id="7e6cf-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="7e6cf-115">[itemActivityStat][]</span></span> | <span data-ttu-id="7e6cf-116">アイテムの寿命を超えた分析。</span><span class="sxs-lookup"><span data-stu-id="7e6cf-116">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="7e6cf-117">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="7e6cf-117">lastSevenDays</span></span> | <span data-ttu-id="7e6cf-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="7e6cf-118">[itemActivityStat][]</span></span> | <span data-ttu-id="7e6cf-119">過去7日間の分析。</span><span class="sxs-lookup"><span data-stu-id="7e6cf-119">Analytics for the last seven days.</span></span>

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
