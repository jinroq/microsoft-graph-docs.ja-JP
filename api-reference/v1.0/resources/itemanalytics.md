---
author: daspek
ms.author: dspektor
title: itemAnalytics リソースの種類
description: ItemAnalytics オブジェクトは、アイテムに対して行われたアクティビティに関する分析を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9c33a79d2728b578eeab1348a655e2b7a7574955
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036583"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="49d5e-103">itemAnalytics リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49d5e-103">itemAnalytics resource type</span></span>

<span data-ttu-id="49d5e-104">**Itemanalytics**リソースは、アイテムに対して行われたアクティビティに分析を提供します。</span><span class="sxs-lookup"><span data-stu-id="49d5e-104">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="49d5e-105">このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="49d5e-105">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="49d5e-106">[GetActivitiesByInterval][] API を使用して、カスタムの時間範囲または間隔で分析を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="49d5e-106">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="49d5e-107">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="49d5e-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="49d5e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49d5e-108">Properties</span></span>

| <span data-ttu-id="49d5e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49d5e-109">Property</span></span>      | <span data-ttu-id="49d5e-110">型</span><span class="sxs-lookup"><span data-stu-id="49d5e-110">Type</span></span>                 | <span data-ttu-id="49d5e-111">説明</span><span class="sxs-lookup"><span data-stu-id="49d5e-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="49d5e-112">allTime</span><span class="sxs-lookup"><span data-stu-id="49d5e-112">allTime</span></span>       | <span data-ttu-id="49d5e-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="49d5e-113">[itemActivityStat][]</span></span> | <span data-ttu-id="49d5e-114">アイテムの寿命を超えた分析。</span><span class="sxs-lookup"><span data-stu-id="49d5e-114">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="49d5e-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="49d5e-115">lastSevenDays</span></span> | <span data-ttu-id="49d5e-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="49d5e-116">[itemActivityStat][]</span></span> | <span data-ttu-id="49d5e-117">過去7日間の分析。</span><span class="sxs-lookup"><span data-stu-id="49d5e-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="49d5e-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49d5e-120">JSON representation</span></span>

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
