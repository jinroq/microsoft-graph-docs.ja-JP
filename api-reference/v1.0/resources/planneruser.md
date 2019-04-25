---
title: プランユーザーリソースの種類
description: '**plan ユーザー**リソースは、ユーザーの Planner リソースへのアクセスを提供します。 使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549826"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="765ca-104">プランユーザーリソースの種類</span><span class="sxs-lookup"><span data-stu-id="765ca-104">plannerUser resource type</span></span>

<span data-ttu-id="765ca-105">**plan ユーザー**リソースは、[ユーザー](user.md)の Planner リソースへのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="765ca-105">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="765ca-106">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="765ca-106">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="765ca-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="765ca-107">Methods</span></span>

| <span data-ttu-id="765ca-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="765ca-108">Method</span></span>           | <span data-ttu-id="765ca-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="765ca-109">Return Type</span></span>    |<span data-ttu-id="765ca-110">説明</span><span class="sxs-lookup"><span data-stu-id="765ca-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="765ca-111">計画を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="765ca-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="765ca-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="765ca-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="765ca-113">**プラン**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="765ca-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="765ca-114">タスクを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="765ca-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="765ca-115">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="765ca-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="765ca-116">プランを取得する**タスク**オブジェクトコレクション。</span><span class="sxs-lookup"><span data-stu-id="765ca-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="765ca-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="765ca-117">Properties</span></span>
| <span data-ttu-id="765ca-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="765ca-118">Property</span></span>     | <span data-ttu-id="765ca-119">型</span><span class="sxs-lookup"><span data-stu-id="765ca-119">Type</span></span>   |<span data-ttu-id="765ca-120">説明</span><span class="sxs-lookup"><span data-stu-id="765ca-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="765ca-121">id</span><span class="sxs-lookup"><span data-stu-id="765ca-121">id</span></span>|<span data-ttu-id="765ca-122">String</span><span class="sxs-lookup"><span data-stu-id="765ca-122">String</span></span>| <span data-ttu-id="765ca-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="765ca-123">Read-only.</span></span> <span data-ttu-id="765ca-124">プラン enruser の識別子</span><span class="sxs-lookup"><span data-stu-id="765ca-124">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="765ca-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="765ca-125">Relationships</span></span>
| <span data-ttu-id="765ca-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="765ca-126">Relationship</span></span> | <span data-ttu-id="765ca-127">型</span><span class="sxs-lookup"><span data-stu-id="765ca-127">Type</span></span>   |<span data-ttu-id="765ca-128">説明</span><span class="sxs-lookup"><span data-stu-id="765ca-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="765ca-129">plans</span><span class="sxs-lookup"><span data-stu-id="765ca-129">plans</span></span>|<span data-ttu-id="765ca-130">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="765ca-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="765ca-131">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="765ca-131">Read-only.</span></span> <span data-ttu-id="765ca-132">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="765ca-132">Nullable.</span></span> <span data-ttu-id="765ca-133">ユーザーに割り当てられた担当者の[タスク](plannertask.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="765ca-133">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="765ca-134">tasks</span><span class="sxs-lookup"><span data-stu-id="765ca-134">tasks</span></span>|<span data-ttu-id="765ca-135">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="765ca-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="765ca-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="765ca-136">Read-only.</span></span> <span data-ttu-id="765ca-137">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="765ca-137">Nullable.</span></span> <span data-ttu-id="765ca-138">ユーザーと共有している[プラン](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="765ca-138">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="765ca-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="765ca-139">JSON representation</span></span>
<span data-ttu-id="765ca-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="765ca-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
