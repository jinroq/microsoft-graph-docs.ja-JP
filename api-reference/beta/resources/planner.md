---
title: planner リソースの種類
description: '**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523401"
---
# <a name="planner-resource-type"></a><span data-ttu-id="384ab-105">planner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="384ab-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="384ab-p102">**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="384ab-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="384ab-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="384ab-109">Methods</span></span>

| <span data-ttu-id="384ab-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="384ab-110">Method</span></span>           | <span data-ttu-id="384ab-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="384ab-111">Return Type</span></span>    |<span data-ttu-id="384ab-112">説明</span><span class="sxs-lookup"><span data-stu-id="384ab-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="384ab-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="384ab-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="384ab-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="384ab-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="384ab-115">バケット コレクションの投稿によって新しい **plannerBucket** を作成します。</span><span class="sxs-lookup"><span data-stu-id="384ab-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="384ab-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="384ab-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="384ab-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="384ab-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="384ab-118">計画コレクションの投稿によって新しい **plannerPlan** を作成します。</span><span class="sxs-lookup"><span data-stu-id="384ab-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="384ab-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="384ab-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="384ab-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="384ab-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="384ab-121">タスク コレクションの投稿によって新しい **plannerTask** を作成します。</span><span class="sxs-lookup"><span data-stu-id="384ab-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="384ab-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="384ab-122">Properties</span></span>
| <span data-ttu-id="384ab-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="384ab-123">Property</span></span>     | <span data-ttu-id="384ab-124">型</span><span class="sxs-lookup"><span data-stu-id="384ab-124">Type</span></span>   |<span data-ttu-id="384ab-125">説明</span><span class="sxs-lookup"><span data-stu-id="384ab-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="384ab-126">id</span><span class="sxs-lookup"><span data-stu-id="384ab-126">id</span></span>|<span data-ttu-id="384ab-127">String</span><span class="sxs-lookup"><span data-stu-id="384ab-127">String</span></span>| <span data-ttu-id="384ab-p103">読み取り専用です。**planner** リソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="384ab-p103">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="384ab-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="384ab-130">Relationships</span></span>
| <span data-ttu-id="384ab-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="384ab-131">Relationship</span></span> | <span data-ttu-id="384ab-132">型</span><span class="sxs-lookup"><span data-stu-id="384ab-132">Type</span></span>   |<span data-ttu-id="384ab-133">説明</span><span class="sxs-lookup"><span data-stu-id="384ab-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="384ab-134">buckets</span><span class="sxs-lookup"><span data-stu-id="384ab-134">buckets</span></span>|<span data-ttu-id="384ab-135">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="384ab-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="384ab-p104">読み取り専用です。Null 許容型。指定されたバケットのコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="384ab-p104">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="384ab-139">plans</span><span class="sxs-lookup"><span data-stu-id="384ab-139">plans</span></span>|<span data-ttu-id="384ab-140">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="384ab-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="384ab-p105">読み取り専用です。Null 許容型。指定された計画のコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="384ab-p105">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="384ab-144">tasks</span><span class="sxs-lookup"><span data-stu-id="384ab-144">tasks</span></span>|<span data-ttu-id="384ab-145">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="384ab-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="384ab-p106">読み取り専用です。Null 許容型。指定されたタスクのコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="384ab-p106">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="384ab-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="384ab-149">JSON representation</span></span>
<span data-ttu-id="384ab-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="384ab-150">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planner.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
