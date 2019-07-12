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
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="34c50-103">itemAnalytics リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34c50-103">itemAnalytics resource type</span></span>

<span data-ttu-id="34c50-104">**Itemanalytics**リソースは、アイテムに対して行われたアクティビティに分析を提供します。</span><span class="sxs-lookup"><span data-stu-id="34c50-104">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="34c50-105">このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="34c50-105">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="34c50-106">[GetActivitiesByInterval][] API を使用して、カスタムの時間範囲または間隔で分析を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="34c50-106">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="34c50-107">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="34c50-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="34c50-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34c50-108">Properties</span></span>

| <span data-ttu-id="34c50-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34c50-109">Property</span></span>      | <span data-ttu-id="34c50-110">型</span><span class="sxs-lookup"><span data-stu-id="34c50-110">Type</span></span>                 | <span data-ttu-id="34c50-111">説明</span><span class="sxs-lookup"><span data-stu-id="34c50-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="34c50-112">allTime</span><span class="sxs-lookup"><span data-stu-id="34c50-112">allTime</span></span>       | <span data-ttu-id="34c50-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="34c50-113">[itemActivityStat][]</span></span> | <span data-ttu-id="34c50-114">アイテムの寿命を超えた分析。</span><span class="sxs-lookup"><span data-stu-id="34c50-114">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="34c50-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="34c50-115">lastSevenDays</span></span> | <span data-ttu-id="34c50-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="34c50-116">[itemActivityStat][]</span></span> | <span data-ttu-id="34c50-117">過去7日間の分析。</span><span class="sxs-lookup"><span data-stu-id="34c50-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="34c50-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34c50-120">JSON representation</span></span>

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
