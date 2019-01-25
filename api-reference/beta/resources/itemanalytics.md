---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514965"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="d5014-102">itemAnalytics リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5014-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5014-103">**ItemAnalytics**リソースでは、アイテムに対して行われたアクティビティに関する分析を提供します。</span><span class="sxs-lookup"><span data-stu-id="d5014-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="d5014-104">このリソースは、現在 SharePoint およびビジネスのための OneDrive で使用可能なのみです。</span><span class="sxs-lookup"><span data-stu-id="d5014-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="d5014-105">間隔またはユーザー設定の時刻の範囲の上で分析を取得するために、 [getActivitiesByInterval][] API を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="d5014-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="d5014-106">**注:\*\*\*\*ItemAnalytics**リソースはまだすべての[国内展開](/graph/deployments)で使用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="d5014-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5014-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5014-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d5014-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5014-108">Properties</span></span>

| <span data-ttu-id="d5014-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5014-109">Property</span></span>      | <span data-ttu-id="d5014-110">型</span><span class="sxs-lookup"><span data-stu-id="d5014-110">Type</span></span>                 | <span data-ttu-id="d5014-111">説明</span><span class="sxs-lookup"><span data-stu-id="d5014-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="d5014-112">allTime</span><span class="sxs-lookup"><span data-stu-id="d5014-112">allTime</span></span>       | <span data-ttu-id="d5014-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="d5014-113">[itemActivityStat][]</span></span> | <span data-ttu-id="d5014-114">分析で、アイテムの有効期間です。</span><span class="sxs-lookup"><span data-stu-id="d5014-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="d5014-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="d5014-115">lastSevenDays</span></span> | <span data-ttu-id="d5014-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="d5014-116">[itemActivityStat][]</span></span> | <span data-ttu-id="d5014-117">過去 7 日間の分析。</span><span class="sxs-lookup"><span data-stu-id="d5014-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemanalytics.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
