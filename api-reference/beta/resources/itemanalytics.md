---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 03626b5dad041181558af076b5dc0ac05b684e13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842414"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="0e10e-102">itemAnalytics リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e10e-102">itemAnalytics resource type</span></span>

> <span data-ttu-id="0e10e-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e10e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e10e-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e10e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e10e-105">**ItemAnalytics**リソースでは、アイテムに対して行われたアクティビティに関する分析を提供します。</span><span class="sxs-lookup"><span data-stu-id="0e10e-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="0e10e-106">このリソースは、現在 SharePoint およびビジネスのための OneDrive で使用可能なのみです。</span><span class="sxs-lookup"><span data-stu-id="0e10e-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="0e10e-107">間隔またはユーザー設定の時刻の範囲の上で分析を取得するために、 [getActivitiesByInterval][] API を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="0e10e-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="0e10e-108">**注:\*\*\*\*ItemAnalytics**リソースはまだすべての[国内展開](/graph/deployments)で使用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="0e10e-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e10e-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e10e-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0e10e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e10e-110">Properties</span></span>

| <span data-ttu-id="0e10e-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e10e-111">Property</span></span>      | <span data-ttu-id="0e10e-112">種類</span><span class="sxs-lookup"><span data-stu-id="0e10e-112">Type</span></span>                 | <span data-ttu-id="0e10e-113">説明</span><span class="sxs-lookup"><span data-stu-id="0e10e-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="0e10e-114">allTime</span><span class="sxs-lookup"><span data-stu-id="0e10e-114">allTime</span></span>       | <span data-ttu-id="0e10e-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="0e10e-115">[itemActivityStat][]</span></span> | <span data-ttu-id="0e10e-116">分析で、アイテムの有効期間です。</span><span class="sxs-lookup"><span data-stu-id="0e10e-116">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="0e10e-117">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="0e10e-117">lastSevenDays</span></span> | <span data-ttu-id="0e10e-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="0e10e-118">[itemActivityStat][]</span></span> | <span data-ttu-id="0e10e-119">過去 7 日間の分析。</span><span class="sxs-lookup"><span data-stu-id="0e10e-119">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->
