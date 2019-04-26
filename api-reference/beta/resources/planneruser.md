---
title: プランユーザーリソースの種類
description: '**plan ユーザー**リソースは、ユーザーの Planner リソースへのアクセスを提供します。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563670"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="52da6-103">プランユーザーリソースの種類</span><span class="sxs-lookup"><span data-stu-id="52da6-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52da6-104">**plan ユーザー**リソースは、[ユーザー](user.md)の Planner リソースへのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="52da6-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="52da6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="52da6-105">Methods</span></span>

| <span data-ttu-id="52da6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="52da6-106">Method</span></span>           | <span data-ttu-id="52da6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="52da6-107">Return Type</span></span>    |<span data-ttu-id="52da6-108">説明</span><span class="sxs-lookup"><span data-stu-id="52da6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52da6-109">タスクを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="52da6-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="52da6-110">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="52da6-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="52da6-111">ユーザーに割り当てられている[プラン](plannertask.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="52da6-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="52da6-112">お気に入りのプランを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="52da6-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="52da6-113">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="52da6-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="52da6-114">ユーザーによってお気に入りとしてマークされた[プラン](plannerplan.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="52da6-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="52da6-115">リスト recentPlans</span><span class="sxs-lookup"><span data-stu-id="52da6-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="52da6-116">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="52da6-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="52da6-117">ユーザーが最近閲覧した[プラン](plannerplan.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="52da6-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="52da6-118">更新する</span><span class="sxs-lookup"><span data-stu-id="52da6-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="52da6-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="52da6-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="52da6-120">プランの**ユーザー**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="52da6-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="52da6-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52da6-121">Properties</span></span>
| <span data-ttu-id="52da6-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52da6-122">Property</span></span>     | <span data-ttu-id="52da6-123">型</span><span class="sxs-lookup"><span data-stu-id="52da6-123">Type</span></span>   |<span data-ttu-id="52da6-124">説明</span><span class="sxs-lookup"><span data-stu-id="52da6-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52da6-125">id</span><span class="sxs-lookup"><span data-stu-id="52da6-125">id</span></span>|<span data-ttu-id="52da6-126">String</span><span class="sxs-lookup"><span data-stu-id="52da6-126">String</span></span>| <span data-ttu-id="52da6-127">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="52da6-127">Read-only.</span></span> <span data-ttu-id="52da6-128">プランユーザーの識別子</span><span class="sxs-lookup"><span data-stu-id="52da6-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="52da6-129">お気に入りプランの参照</span><span class="sxs-lookup"><span data-stu-id="52da6-129">favoritePlanReferences</span></span>|[<span data-ttu-id="52da6-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="52da6-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="52da6-131">ユーザーがお気に入りとしてマークしたプランへの参照を含むコレクション。</span><span class="sxs-lookup"><span data-stu-id="52da6-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="52da6-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="52da6-132">recentPlanReferences</span></span>|[<span data-ttu-id="52da6-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="52da6-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="52da6-134">最近のプランをサポートするアプリで、ユーザーが最近表示したプランへの参照を含むコレクション。</span><span class="sxs-lookup"><span data-stu-id="52da6-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52da6-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52da6-135">Relationships</span></span>
| <span data-ttu-id="52da6-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52da6-136">Relationship</span></span> | <span data-ttu-id="52da6-137">型</span><span class="sxs-lookup"><span data-stu-id="52da6-137">Type</span></span>   |<span data-ttu-id="52da6-138">説明</span><span class="sxs-lookup"><span data-stu-id="52da6-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52da6-139">tasks</span><span class="sxs-lookup"><span data-stu-id="52da6-139">tasks</span></span>|<span data-ttu-id="52da6-140">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="52da6-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="52da6-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="52da6-141">Read-only.</span></span> <span data-ttu-id="52da6-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="52da6-142">Nullable.</span></span> <span data-ttu-id="52da6-143">ユーザーに割り当てられた担当者の[タスク](plannertask.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="52da6-143">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="52da6-144">お気に入りのプラン</span><span class="sxs-lookup"><span data-stu-id="52da6-144">favoritePlans</span></span>|<span data-ttu-id="52da6-145">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="52da6-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="52da6-146">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="52da6-146">Read-only.</span></span> <span data-ttu-id="52da6-147">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="52da6-147">Nullable.</span></span> <span data-ttu-id="52da6-148">ユーザーがお気に入りとしてマークした[プラン](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="52da6-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="52da6-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="52da6-149">recentPlans</span></span>|<span data-ttu-id="52da6-150">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="52da6-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="52da6-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="52da6-151">Read-only.</span></span> <span data-ttu-id="52da6-152">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="52da6-152">Nullable.</span></span> <span data-ttu-id="52da6-153">最近のプランをサポートするアプリで、ユーザーによって最近参照された[プラン](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="52da6-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52da6-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52da6-154">JSON representation</span></span>
<span data-ttu-id="52da6-155">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52da6-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "suppressions": []
}
-->
