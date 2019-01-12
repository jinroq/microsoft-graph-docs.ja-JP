---
title: plannerUser リソースの種類
description: '**PlannerUser**リソースでは、ユーザーの計画のリソースへのアクセスを提供します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1b240092e7476884399f88fad61551763f33fe69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928284"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="4bdc4-103">plannerUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4bdc4-103">plannerUser resource type</span></span>

> <span data-ttu-id="4bdc4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bdc4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bdc4-106">**PlannerUser**リソースでは、[ユーザー](user.md)の計画のリソースへのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="4bdc4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4bdc4-107">Methods</span></span>

| <span data-ttu-id="4bdc4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4bdc4-108">Method</span></span>           | <span data-ttu-id="4bdc4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4bdc4-109">Return Type</span></span>    |<span data-ttu-id="4bdc4-110">説明</span><span class="sxs-lookup"><span data-stu-id="4bdc4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bdc4-111">List tasks</span><span class="sxs-lookup"><span data-stu-id="4bdc4-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="4bdc4-112">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4bdc4-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="4bdc4-113">ユーザーに割り当てられている[plannerTasks](plannertask.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="4bdc4-114">リスト favoritePlans</span><span class="sxs-lookup"><span data-stu-id="4bdc4-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="4bdc4-115">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4bdc4-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4bdc4-116">ユーザーがお気に入りとしてマークされている[plannerPlans](plannerplan.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="4bdc4-117">リスト recentPlans</span><span class="sxs-lookup"><span data-stu-id="4bdc4-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="4bdc4-118">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4bdc4-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4bdc4-119">ユーザーが最近表示した[plannerPlans](plannerplan.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="4bdc4-120">Update</span><span class="sxs-lookup"><span data-stu-id="4bdc4-120">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="4bdc4-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="4bdc4-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="4bdc4-122">**PlannerUser**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="4bdc4-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bdc4-123">Properties</span></span>
| <span data-ttu-id="4bdc4-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bdc4-124">Property</span></span>     | <span data-ttu-id="4bdc4-125">型</span><span class="sxs-lookup"><span data-stu-id="4bdc4-125">Type</span></span>   |<span data-ttu-id="4bdc4-126">説明</span><span class="sxs-lookup"><span data-stu-id="4bdc4-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bdc4-127">ID</span><span class="sxs-lookup"><span data-stu-id="4bdc4-127">id</span></span>|<span data-ttu-id="4bdc4-128">String</span><span class="sxs-lookup"><span data-stu-id="4bdc4-128">String</span></span>| <span data-ttu-id="4bdc4-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-129">Read-only.</span></span> <span data-ttu-id="4bdc4-130">PlannerUser の識別子</span><span class="sxs-lookup"><span data-stu-id="4bdc4-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="4bdc4-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="4bdc4-131">favoritePlanReferences</span></span>|[<span data-ttu-id="4bdc4-132">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="4bdc4-132">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="4bdc4-133">ユーザーは、お気に入りとしてマークする計画への参照を格納するコレクション。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="4bdc4-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="4bdc4-134">recentPlanReferences</span></span>|[<span data-ttu-id="4bdc4-135">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="4bdc4-135">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="4bdc4-136">最近の計画をサポートするアプリケーションでユーザーが最近表示された計画への参照を格納するコレクション。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bdc4-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4bdc4-137">Relationships</span></span>
| <span data-ttu-id="4bdc4-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4bdc4-138">Relationship</span></span> | <span data-ttu-id="4bdc4-139">型</span><span class="sxs-lookup"><span data-stu-id="4bdc4-139">Type</span></span>   |<span data-ttu-id="4bdc4-140">説明</span><span class="sxs-lookup"><span data-stu-id="4bdc4-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bdc4-141">tasks</span><span class="sxs-lookup"><span data-stu-id="4bdc4-141">tasks</span></span>|<span data-ttu-id="4bdc4-142">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4bdc4-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="4bdc4-p103">読み取り専用です。Null 許容型。ユーザーに割り当てられている [plannerTasks](plannertask.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="4bdc4-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="4bdc4-146">favoritePlans</span></span>|<span data-ttu-id="4bdc4-147">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4bdc4-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4bdc4-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-148">Read-only.</span></span> <span data-ttu-id="4bdc4-149">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-149">Nullable.</span></span> <span data-ttu-id="4bdc4-150">ユーザーは、お気に入りとしてマークされている[plannerPlans](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="4bdc4-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="4bdc4-151">recentPlans</span></span>|<span data-ttu-id="4bdc4-152">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4bdc4-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4bdc4-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-153">Read-only.</span></span> <span data-ttu-id="4bdc4-154">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-154">Nullable.</span></span> <span data-ttu-id="4bdc4-155">最近の計画をサポートするアプリケーションでユーザーが最近表示した[plannerPlans](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4bdc4-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4bdc4-156">JSON representation</span></span>
<span data-ttu-id="4bdc4-157">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bdc4-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
