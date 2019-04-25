---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemanalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581647"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="44383-102">itemanalytics リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44383-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44383-103">**itemanalytics**リソースは、アイテムに対して行われたアクティビティに分析を提供します。</span><span class="sxs-lookup"><span data-stu-id="44383-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="44383-104">このリソースは現在、SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="44383-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="44383-105">[getActivitiesByInterval][] API を使用して、カスタムの時間範囲または間隔で分析を取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="44383-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="44383-106">**注:\*\*\*\*itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="44383-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="44383-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44383-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="44383-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44383-108">Properties</span></span>

| <span data-ttu-id="44383-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44383-109">Property</span></span>      | <span data-ttu-id="44383-110">型</span><span class="sxs-lookup"><span data-stu-id="44383-110">Type</span></span>                 | <span data-ttu-id="44383-111">説明</span><span class="sxs-lookup"><span data-stu-id="44383-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="44383-112">alltime</span><span class="sxs-lookup"><span data-stu-id="44383-112">allTime</span></span>       | <span data-ttu-id="44383-113">[itemactiv][]</span><span class="sxs-lookup"><span data-stu-id="44383-113">[itemActivityStat][]</span></span> | <span data-ttu-id="44383-114">アイテムの寿命を超えた分析。</span><span class="sxs-lookup"><span data-stu-id="44383-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="44383-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="44383-115">lastSevenDays</span></span> | <span data-ttu-id="44383-116">[itemactiv][]</span><span class="sxs-lookup"><span data-stu-id="44383-116">[itemActivityStat][]</span></span> | <span data-ttu-id="44383-117">過去7日間の分析。</span><span class="sxs-lookup"><span data-stu-id="44383-117">Analytics for the last seven days.</span></span>

[itemactiv]: itemactivitystat.md
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
