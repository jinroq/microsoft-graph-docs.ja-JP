---
title: planner リソースの種類
description: '**planner**リソースは、planner オブジェクトモデルのエントリポイントです。 シングルトン**プランナー**リソースを返します。  使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f6d25238436b79dec0397df1d005e67e6b17239a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462278"
---
# <a name="planner-resource-type"></a><span data-ttu-id="408a4-105">planner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="408a4-105">planner resource type</span></span>

<span data-ttu-id="408a4-106">**planner**リソースは、planner オブジェクトモデルのエントリポイントです。</span><span class="sxs-lookup"><span data-stu-id="408a4-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="408a4-107">シングルトン**プランナー**リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="408a4-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="408a4-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="408a4-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="408a4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="408a4-109">Methods</span></span>

| <span data-ttu-id="408a4-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="408a4-110">Method</span></span>           | <span data-ttu-id="408a4-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="408a4-111">Return Type</span></span>    |<span data-ttu-id="408a4-112">説明</span><span class="sxs-lookup"><span data-stu-id="408a4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="408a4-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="408a4-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="408a4-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="408a4-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="408a4-115">バケットコレクションへの投稿により、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="408a4-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="408a4-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="408a4-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="408a4-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="408a4-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="408a4-118">プランコレクションへの投稿によって、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="408a4-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="408a4-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="408a4-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="408a4-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="408a4-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="408a4-121">タスクコレクションへの投稿によって、新しい**プラン**を作成します。</span><span class="sxs-lookup"><span data-stu-id="408a4-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="408a4-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="408a4-122">Relationships</span></span>
| <span data-ttu-id="408a4-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="408a4-123">Relationship</span></span> | <span data-ttu-id="408a4-124">型</span><span class="sxs-lookup"><span data-stu-id="408a4-124">Type</span></span>   |<span data-ttu-id="408a4-125">説明</span><span class="sxs-lookup"><span data-stu-id="408a4-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="408a4-126">buckets</span><span class="sxs-lookup"><span data-stu-id="408a4-126">buckets</span></span>|<span data-ttu-id="408a4-127">[プラン | バケット](plannerbucket.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="408a4-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="408a4-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="408a4-128">Read-only.</span></span> <span data-ttu-id="408a4-129">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="408a4-129">Nullable.</span></span> <span data-ttu-id="408a4-130">指定したバケットのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="408a4-130">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="408a4-131">plans</span><span class="sxs-lookup"><span data-stu-id="408a4-131">plans</span></span>|<span data-ttu-id="408a4-132">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="408a4-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="408a4-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="408a4-133">Read-only.</span></span> <span data-ttu-id="408a4-134">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="408a4-134">Nullable.</span></span> <span data-ttu-id="408a4-135">指定したプランのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="408a4-135">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="408a4-136">tasks</span><span class="sxs-lookup"><span data-stu-id="408a4-136">tasks</span></span>|<span data-ttu-id="408a4-137">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="408a4-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="408a4-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="408a4-138">Read-only.</span></span> <span data-ttu-id="408a4-139">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="408a4-139">Nullable.</span></span> <span data-ttu-id="408a4-140">指定したタスクのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="408a4-140">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="408a4-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="408a4-141">JSON representation</span></span>
<span data-ttu-id="408a4-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="408a4-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="408a4-143">例</span><span class="sxs-lookup"><span data-stu-id="408a4-143">Example</span></span>

<span data-ttu-id="408a4-144">**プランナー**リソースは、グラフのルートにあります。</span><span class="sxs-lookup"><span data-stu-id="408a4-144">The **planner** resource is available at the root of the graph.</span></span>

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
