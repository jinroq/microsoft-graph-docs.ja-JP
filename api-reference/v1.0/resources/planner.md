---
title: planner リソースの種類
description: '**Planner**リソースは、planner オブジェクトモデルのエントリポイントです。 シングルトン**プランナー**リソースを返します。  使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b5cbf089e2d926440999c3ec73341bb3458668db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035358"
---
# <a name="planner-resource-type"></a><span data-ttu-id="59e72-105">planner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59e72-105">planner resource type</span></span>

<span data-ttu-id="59e72-106">**Planner**リソースは、planner オブジェクトモデルのエントリポイントです。</span><span class="sxs-lookup"><span data-stu-id="59e72-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="59e72-107">シングルトン**プランナー**リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="59e72-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="59e72-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="59e72-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="59e72-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="59e72-109">Methods</span></span>

| <span data-ttu-id="59e72-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="59e72-110">Method</span></span>           | <span data-ttu-id="59e72-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="59e72-111">Return Type</span></span>    |<span data-ttu-id="59e72-112">説明</span><span class="sxs-lookup"><span data-stu-id="59e72-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="59e72-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="59e72-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="59e72-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="59e72-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="59e72-115">バケットコレクションへの投稿により、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="59e72-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="59e72-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="59e72-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="59e72-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="59e72-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="59e72-118">プランコレクションへの投稿によって、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="59e72-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="59e72-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="59e72-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="59e72-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="59e72-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="59e72-121">タスクコレクションへの投稿によって、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="59e72-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59e72-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59e72-122">Relationships</span></span>
| <span data-ttu-id="59e72-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59e72-123">Relationship</span></span> | <span data-ttu-id="59e72-124">型</span><span class="sxs-lookup"><span data-stu-id="59e72-124">Type</span></span>   |<span data-ttu-id="59e72-125">説明</span><span class="sxs-lookup"><span data-stu-id="59e72-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59e72-126">buckets</span><span class="sxs-lookup"><span data-stu-id="59e72-126">buckets</span></span>|<span data-ttu-id="59e72-127">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="59e72-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="59e72-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e72-128">Read-only.</span></span> <span data-ttu-id="59e72-129">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="59e72-129">Nullable.</span></span> <span data-ttu-id="59e72-130">指定したバケットのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="59e72-130">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="59e72-131">plans</span><span class="sxs-lookup"><span data-stu-id="59e72-131">plans</span></span>|<span data-ttu-id="59e72-132">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="59e72-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="59e72-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e72-133">Read-only.</span></span> <span data-ttu-id="59e72-134">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="59e72-134">Nullable.</span></span> <span data-ttu-id="59e72-135">指定したプランのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="59e72-135">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="59e72-136">tasks</span><span class="sxs-lookup"><span data-stu-id="59e72-136">tasks</span></span>|<span data-ttu-id="59e72-137">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="59e72-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="59e72-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e72-138">Read-only.</span></span> <span data-ttu-id="59e72-139">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="59e72-139">Nullable.</span></span> <span data-ttu-id="59e72-140">指定したタスクのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="59e72-140">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59e72-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59e72-141">JSON representation</span></span>
<span data-ttu-id="59e72-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59e72-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="59e72-143">例</span><span class="sxs-lookup"><span data-stu-id="59e72-143">Example</span></span>

<span data-ttu-id="59e72-144">**プランナー**リソースは、グラフのルートにあります。</span><span class="sxs-lookup"><span data-stu-id="59e72-144">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
