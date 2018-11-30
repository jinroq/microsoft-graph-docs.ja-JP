---
title: planner リソースの種類
description: '**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。'
ms.openlocfilehash: e5980f6f4037b57e977b12ef223e8a5a2cf7c77c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023523"
---
# <a name="planner-resource-type"></a><span data-ttu-id="15677-105">planner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15677-105">planner resource type</span></span>

<span data-ttu-id="15677-p102">**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="15677-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="15677-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="15677-109">Methods</span></span>

| <span data-ttu-id="15677-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="15677-110">Method</span></span>           | <span data-ttu-id="15677-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="15677-111">Return Type</span></span>    |<span data-ttu-id="15677-112">説明</span><span class="sxs-lookup"><span data-stu-id="15677-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="15677-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="15677-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="15677-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="15677-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="15677-115">バケット コレクションの投稿によって新しい **plannerBucket** を作成します。</span><span class="sxs-lookup"><span data-stu-id="15677-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="15677-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="15677-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="15677-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="15677-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="15677-118">計画コレクションの投稿によって新しい **plannerPlan** を作成します。</span><span class="sxs-lookup"><span data-stu-id="15677-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="15677-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="15677-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="15677-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="15677-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="15677-121">タスク コレクションの投稿によって新しい **plannerTask** を作成します。</span><span class="sxs-lookup"><span data-stu-id="15677-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15677-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15677-122">Relationships</span></span>
| <span data-ttu-id="15677-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15677-123">Relationship</span></span> | <span data-ttu-id="15677-124">型</span><span class="sxs-lookup"><span data-stu-id="15677-124">Type</span></span>   |<span data-ttu-id="15677-125">説明</span><span class="sxs-lookup"><span data-stu-id="15677-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15677-126">buckets</span><span class="sxs-lookup"><span data-stu-id="15677-126">buckets</span></span>|<span data-ttu-id="15677-127">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="15677-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="15677-p103">読み取り専用です。Null 許容型。指定されたバケットのコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="15677-p103">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="15677-131">plans</span><span class="sxs-lookup"><span data-stu-id="15677-131">plans</span></span>|<span data-ttu-id="15677-132">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="15677-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="15677-p104">読み取り専用です。Null 許容型。指定された計画のコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="15677-p104">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="15677-136">tasks</span><span class="sxs-lookup"><span data-stu-id="15677-136">tasks</span></span>|<span data-ttu-id="15677-137">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="15677-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="15677-p105">読み取り専用です。Null 許容型。指定されたタスクのコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="15677-p105">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15677-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15677-141">JSON representation</span></span>
<span data-ttu-id="15677-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15677-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="15677-143">使用例</span><span class="sxs-lookup"><span data-stu-id="15677-143">Example</span></span>

<span data-ttu-id="15677-144">**プランナー**のリソースは、グラフのルートに使用できます。</span><span class="sxs-lookup"><span data-stu-id="15677-144">The **planner** resource is available at the root of the graph.</span></span>

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