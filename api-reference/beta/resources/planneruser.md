---
title: plannerUser リソースの種類
description: '**PlannerUser**リソースでは、ユーザーの計画のリソースへのアクセスを提供します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526880"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="d11f9-103">plannerUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d11f9-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d11f9-104">**PlannerUser**リソースでは、[ユーザー](user.md)の計画のリソースへのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="d11f9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d11f9-105">Methods</span></span>

| <span data-ttu-id="d11f9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d11f9-106">Method</span></span>           | <span data-ttu-id="d11f9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d11f9-107">Return Type</span></span>    |<span data-ttu-id="d11f9-108">説明</span><span class="sxs-lookup"><span data-stu-id="d11f9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d11f9-109">List tasks</span><span class="sxs-lookup"><span data-stu-id="d11f9-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="d11f9-110">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d11f9-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d11f9-111">ユーザーに割り当てられている[plannerTasks](plannertask.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="d11f9-112">リスト favoritePlans</span><span class="sxs-lookup"><span data-stu-id="d11f9-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="d11f9-113">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d11f9-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d11f9-114">ユーザーがお気に入りとしてマークされている[plannerPlans](plannerplan.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="d11f9-115">リスト recentPlans</span><span class="sxs-lookup"><span data-stu-id="d11f9-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="d11f9-116">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d11f9-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d11f9-117">ユーザーが最近表示した[plannerPlans](plannerplan.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="d11f9-118">Update</span><span class="sxs-lookup"><span data-stu-id="d11f9-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="d11f9-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="d11f9-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="d11f9-120">**PlannerUser**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="d11f9-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d11f9-121">Properties</span></span>
| <span data-ttu-id="d11f9-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d11f9-122">Property</span></span>     | <span data-ttu-id="d11f9-123">型</span><span class="sxs-lookup"><span data-stu-id="d11f9-123">Type</span></span>   |<span data-ttu-id="d11f9-124">説明</span><span class="sxs-lookup"><span data-stu-id="d11f9-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d11f9-125">id</span><span class="sxs-lookup"><span data-stu-id="d11f9-125">id</span></span>|<span data-ttu-id="d11f9-126">String</span><span class="sxs-lookup"><span data-stu-id="d11f9-126">String</span></span>| <span data-ttu-id="d11f9-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d11f9-127">Read-only.</span></span> <span data-ttu-id="d11f9-128">PlannerUser の識別子</span><span class="sxs-lookup"><span data-stu-id="d11f9-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="d11f9-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="d11f9-129">favoritePlanReferences</span></span>|[<span data-ttu-id="d11f9-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="d11f9-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="d11f9-131">ユーザーは、お気に入りとしてマークする計画への参照を格納するコレクション。</span><span class="sxs-lookup"><span data-stu-id="d11f9-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="d11f9-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="d11f9-132">recentPlanReferences</span></span>|[<span data-ttu-id="d11f9-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="d11f9-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="d11f9-134">最近の計画をサポートするアプリケーションでユーザーが最近表示された計画への参照を格納するコレクション。</span><span class="sxs-lookup"><span data-stu-id="d11f9-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d11f9-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d11f9-135">Relationships</span></span>
| <span data-ttu-id="d11f9-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d11f9-136">Relationship</span></span> | <span data-ttu-id="d11f9-137">型</span><span class="sxs-lookup"><span data-stu-id="d11f9-137">Type</span></span>   |<span data-ttu-id="d11f9-138">説明</span><span class="sxs-lookup"><span data-stu-id="d11f9-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d11f9-139">tasks</span><span class="sxs-lookup"><span data-stu-id="d11f9-139">tasks</span></span>|<span data-ttu-id="d11f9-140">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d11f9-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d11f9-p102">読み取り専用です。Null 許容型。ユーザーに割り当てられている [plannerTasks](plannertask.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-p102">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="d11f9-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="d11f9-144">favoritePlans</span></span>|<span data-ttu-id="d11f9-145">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d11f9-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d11f9-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d11f9-146">Read-only.</span></span> <span data-ttu-id="d11f9-147">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d11f9-147">Nullable.</span></span> <span data-ttu-id="d11f9-148">ユーザーは、お気に入りとしてマークされている[plannerPlans](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="d11f9-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="d11f9-149">recentPlans</span></span>|<span data-ttu-id="d11f9-150">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d11f9-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d11f9-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d11f9-151">Read-only.</span></span> <span data-ttu-id="d11f9-152">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d11f9-152">Nullable.</span></span> <span data-ttu-id="d11f9-153">最近の計画をサポートするアプリケーションでユーザーが最近表示した[plannerPlans](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d11f9-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d11f9-154">JSON representation</span></span>
<span data-ttu-id="d11f9-155">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d11f9-155">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planneruser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
