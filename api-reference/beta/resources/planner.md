---
title: planner リソースの種類
description: '**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。'
localization_priority: Normal
ms.openlocfilehash: 9dc6904da25d7612b94649264001dcae98859925
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889097"
---
# <a name="planner-resource-type"></a><span data-ttu-id="18966-105">planner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18966-105">planner resource type</span></span>

> <span data-ttu-id="18966-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18966-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18966-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18966-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18966-p103">**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="18966-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="18966-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="18966-111">Methods</span></span>

| <span data-ttu-id="18966-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="18966-112">Method</span></span>           | <span data-ttu-id="18966-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="18966-113">Return Type</span></span>    |<span data-ttu-id="18966-114">説明</span><span class="sxs-lookup"><span data-stu-id="18966-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18966-115">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="18966-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="18966-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="18966-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="18966-117">バケット コレクションの投稿によって新しい **plannerBucket** を作成します。</span><span class="sxs-lookup"><span data-stu-id="18966-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="18966-118">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="18966-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="18966-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="18966-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="18966-120">計画コレクションの投稿によって新しい **plannerPlan** を作成します。</span><span class="sxs-lookup"><span data-stu-id="18966-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="18966-121">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="18966-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="18966-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="18966-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="18966-123">タスク コレクションの投稿によって新しい **plannerTask** を作成します。</span><span class="sxs-lookup"><span data-stu-id="18966-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="18966-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18966-124">Properties</span></span>
| <span data-ttu-id="18966-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18966-125">Property</span></span>     | <span data-ttu-id="18966-126">種類</span><span class="sxs-lookup"><span data-stu-id="18966-126">Type</span></span>   |<span data-ttu-id="18966-127">説明</span><span class="sxs-lookup"><span data-stu-id="18966-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18966-128">ID</span><span class="sxs-lookup"><span data-stu-id="18966-128">id</span></span>|<span data-ttu-id="18966-129">String</span><span class="sxs-lookup"><span data-stu-id="18966-129">String</span></span>| <span data-ttu-id="18966-p104">読み取り専用です。**planner** リソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="18966-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18966-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18966-132">Relationships</span></span>
| <span data-ttu-id="18966-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18966-133">Relationship</span></span> | <span data-ttu-id="18966-134">型</span><span class="sxs-lookup"><span data-stu-id="18966-134">Type</span></span>   |<span data-ttu-id="18966-135">説明</span><span class="sxs-lookup"><span data-stu-id="18966-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18966-136">buckets</span><span class="sxs-lookup"><span data-stu-id="18966-136">buckets</span></span>|<span data-ttu-id="18966-137">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="18966-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="18966-p105">読み取り専用です。Null 許容型。指定されたバケットのコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="18966-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="18966-141">plans</span><span class="sxs-lookup"><span data-stu-id="18966-141">plans</span></span>|<span data-ttu-id="18966-142">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="18966-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="18966-p106">読み取り専用です。Null 許容型。指定された計画のコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="18966-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="18966-146">tasks</span><span class="sxs-lookup"><span data-stu-id="18966-146">tasks</span></span>|<span data-ttu-id="18966-147">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="18966-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="18966-p107">読み取り専用です。Null 許容型。指定されたタスクのコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="18966-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18966-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18966-151">JSON representation</span></span>
<span data-ttu-id="18966-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18966-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
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
