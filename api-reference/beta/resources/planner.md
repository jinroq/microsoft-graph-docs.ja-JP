---
title: planner リソースの種類
description: '**planner**リソースは、planner オブジェクトモデルのエントリポイントです。 シングルトン**プランナー**リソースを返します。  使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2f1fb3b7058a87dd7b8390408590371cf1b0e9cd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344626"
---
# <a name="planner-resource-type"></a><span data-ttu-id="88470-105">planner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88470-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88470-106">**planner**リソースは、planner オブジェクトモデルのエントリポイントです。</span><span class="sxs-lookup"><span data-stu-id="88470-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="88470-107">シングルトン**プランナー**リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="88470-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="88470-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="88470-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="88470-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="88470-109">Methods</span></span>

| <span data-ttu-id="88470-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="88470-110">Method</span></span>           | <span data-ttu-id="88470-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="88470-111">Return Type</span></span>    |<span data-ttu-id="88470-112">説明</span><span class="sxs-lookup"><span data-stu-id="88470-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88470-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="88470-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="88470-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="88470-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="88470-115">バケットコレクションへの投稿により、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="88470-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="88470-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="88470-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="88470-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="88470-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="88470-118">プランコレクションへの投稿によって、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="88470-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="88470-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="88470-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="88470-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="88470-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="88470-121">タスクコレクションへの投稿によって、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="88470-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="88470-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88470-122">Properties</span></span>
| <span data-ttu-id="88470-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88470-123">Property</span></span>     | <span data-ttu-id="88470-124">型</span><span class="sxs-lookup"><span data-stu-id="88470-124">Type</span></span>   |<span data-ttu-id="88470-125">説明</span><span class="sxs-lookup"><span data-stu-id="88470-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88470-126">id</span><span class="sxs-lookup"><span data-stu-id="88470-126">id</span></span>|<span data-ttu-id="88470-127">String</span><span class="sxs-lookup"><span data-stu-id="88470-127">String</span></span>| <span data-ttu-id="88470-128">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="88470-128">Read-only.</span></span> <span data-ttu-id="88470-129">**planner**リソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="88470-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88470-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="88470-130">Relationships</span></span>
| <span data-ttu-id="88470-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="88470-131">Relationship</span></span> | <span data-ttu-id="88470-132">型</span><span class="sxs-lookup"><span data-stu-id="88470-132">Type</span></span>   |<span data-ttu-id="88470-133">説明</span><span class="sxs-lookup"><span data-stu-id="88470-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88470-134">buckets</span><span class="sxs-lookup"><span data-stu-id="88470-134">buckets</span></span>|<span data-ttu-id="88470-135">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88470-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="88470-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="88470-136">Read-only.</span></span> <span data-ttu-id="88470-137">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="88470-137">Nullable.</span></span> <span data-ttu-id="88470-138">指定したバケットのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="88470-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="88470-139">plans</span><span class="sxs-lookup"><span data-stu-id="88470-139">plans</span></span>|<span data-ttu-id="88470-140">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88470-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="88470-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="88470-141">Read-only.</span></span> <span data-ttu-id="88470-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="88470-142">Nullable.</span></span> <span data-ttu-id="88470-143">指定したプランのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="88470-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="88470-144">tasks</span><span class="sxs-lookup"><span data-stu-id="88470-144">tasks</span></span>|<span data-ttu-id="88470-145">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88470-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="88470-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="88470-146">Read-only.</span></span> <span data-ttu-id="88470-147">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="88470-147">Nullable.</span></span> <span data-ttu-id="88470-148">指定したタスクのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="88470-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88470-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88470-149">JSON representation</span></span>
<span data-ttu-id="88470-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88470-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
