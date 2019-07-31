---
title: planner リソースの種類
description: '**Planner**リソースは、planner オブジェクトモデルのエントリポイントです。 シングルトン**プランナー**リソースを返します。  使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2ef94a7507558279e5295239588e2a8eda512882
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009133"
---
# <a name="planner-resource-type"></a><span data-ttu-id="46a29-105">planner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46a29-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46a29-106">**Planner**リソースは、planner オブジェクトモデルのエントリポイントです。</span><span class="sxs-lookup"><span data-stu-id="46a29-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="46a29-107">シングルトン**プランナー**リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="46a29-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="46a29-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="46a29-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="46a29-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="46a29-109">Methods</span></span>

| <span data-ttu-id="46a29-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="46a29-110">Method</span></span>           | <span data-ttu-id="46a29-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="46a29-111">Return Type</span></span>    |<span data-ttu-id="46a29-112">説明</span><span class="sxs-lookup"><span data-stu-id="46a29-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46a29-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="46a29-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="46a29-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="46a29-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="46a29-115">バケットコレクションへの投稿により、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="46a29-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="46a29-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="46a29-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="46a29-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="46a29-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="46a29-118">プランコレクションへの投稿によって、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="46a29-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="46a29-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="46a29-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="46a29-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="46a29-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="46a29-121">タスクコレクションへの投稿によって、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="46a29-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="46a29-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46a29-122">Properties</span></span>
| <span data-ttu-id="46a29-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46a29-123">Property</span></span>     | <span data-ttu-id="46a29-124">型</span><span class="sxs-lookup"><span data-stu-id="46a29-124">Type</span></span>   |<span data-ttu-id="46a29-125">説明</span><span class="sxs-lookup"><span data-stu-id="46a29-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46a29-126">id</span><span class="sxs-lookup"><span data-stu-id="46a29-126">id</span></span>|<span data-ttu-id="46a29-127">String</span><span class="sxs-lookup"><span data-stu-id="46a29-127">String</span></span>| <span data-ttu-id="46a29-128">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="46a29-128">Read-only.</span></span> <span data-ttu-id="46a29-129">**Planner**リソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="46a29-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46a29-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46a29-130">Relationships</span></span>
| <span data-ttu-id="46a29-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46a29-131">Relationship</span></span> | <span data-ttu-id="46a29-132">型</span><span class="sxs-lookup"><span data-stu-id="46a29-132">Type</span></span>   |<span data-ttu-id="46a29-133">説明</span><span class="sxs-lookup"><span data-stu-id="46a29-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46a29-134">buckets</span><span class="sxs-lookup"><span data-stu-id="46a29-134">buckets</span></span>|<span data-ttu-id="46a29-135">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="46a29-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="46a29-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="46a29-136">Read-only.</span></span> <span data-ttu-id="46a29-137">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="46a29-137">Nullable.</span></span> <span data-ttu-id="46a29-138">指定したバケットのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="46a29-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="46a29-139">plans</span><span class="sxs-lookup"><span data-stu-id="46a29-139">plans</span></span>|<span data-ttu-id="46a29-140">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="46a29-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="46a29-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="46a29-141">Read-only.</span></span> <span data-ttu-id="46a29-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="46a29-142">Nullable.</span></span> <span data-ttu-id="46a29-143">指定したプランのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="46a29-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="46a29-144">tasks</span><span class="sxs-lookup"><span data-stu-id="46a29-144">tasks</span></span>|<span data-ttu-id="46a29-145">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="46a29-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="46a29-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="46a29-146">Read-only.</span></span> <span data-ttu-id="46a29-147">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="46a29-147">Nullable.</span></span> <span data-ttu-id="46a29-148">指定したタスクのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="46a29-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46a29-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46a29-149">JSON representation</span></span>
<span data-ttu-id="46a29-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="46a29-150">Here is a JSON representation of the resource.</span></span>

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
