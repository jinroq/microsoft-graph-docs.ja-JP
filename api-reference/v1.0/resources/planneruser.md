---
title: プランユーザーリソースの種類
description: '**Plan ユーザー**リソースは、ユーザーの Planner リソースへのアクセスを提供します。 使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d995888b55282ac9db8aef9cc047f069a3cf20fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035141"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="ce5de-104">プランユーザーリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce5de-104">plannerUser resource type</span></span>

<span data-ttu-id="ce5de-105">**Plan ユーザー**リソースは、[ユーザー](user.md)の Planner リソースへのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="ce5de-105">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="ce5de-106">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="ce5de-106">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="ce5de-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce5de-107">Methods</span></span>

| <span data-ttu-id="ce5de-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce5de-108">Method</span></span>           | <span data-ttu-id="ce5de-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce5de-109">Return Type</span></span>    |<span data-ttu-id="ce5de-110">説明</span><span class="sxs-lookup"><span data-stu-id="ce5de-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce5de-111">計画を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ce5de-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="ce5de-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ce5de-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ce5de-113">**プラン**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ce5de-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="ce5de-114">List tasks</span><span class="sxs-lookup"><span data-stu-id="ce5de-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="ce5de-115">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ce5de-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ce5de-116">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ce5de-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce5de-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce5de-117">Properties</span></span>
| <span data-ttu-id="ce5de-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce5de-118">Property</span></span>     | <span data-ttu-id="ce5de-119">型</span><span class="sxs-lookup"><span data-stu-id="ce5de-119">Type</span></span>   |<span data-ttu-id="ce5de-120">説明</span><span class="sxs-lookup"><span data-stu-id="ce5de-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce5de-121">id</span><span class="sxs-lookup"><span data-stu-id="ce5de-121">id</span></span>|<span data-ttu-id="ce5de-122">String</span><span class="sxs-lookup"><span data-stu-id="ce5de-122">String</span></span>| <span data-ttu-id="ce5de-123">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ce5de-123">Read-only.</span></span> <span data-ttu-id="ce5de-124">プラン Enruser の識別子</span><span class="sxs-lookup"><span data-stu-id="ce5de-124">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce5de-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce5de-125">Relationships</span></span>
| <span data-ttu-id="ce5de-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce5de-126">Relationship</span></span> | <span data-ttu-id="ce5de-127">型</span><span class="sxs-lookup"><span data-stu-id="ce5de-127">Type</span></span>   |<span data-ttu-id="ce5de-128">説明</span><span class="sxs-lookup"><span data-stu-id="ce5de-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce5de-129">plans</span><span class="sxs-lookup"><span data-stu-id="ce5de-129">plans</span></span>|<span data-ttu-id="ce5de-130">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ce5de-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ce5de-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce5de-131">Read-only.</span></span> <span data-ttu-id="ce5de-132">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ce5de-132">Nullable.</span></span> <span data-ttu-id="ce5de-133">ユーザーに割り当てられた担当者の[タスク](plannertask.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="ce5de-133">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="ce5de-134">tasks</span><span class="sxs-lookup"><span data-stu-id="ce5de-134">tasks</span></span>|<span data-ttu-id="ce5de-135">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ce5de-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ce5de-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce5de-136">Read-only.</span></span> <span data-ttu-id="ce5de-137">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ce5de-137">Nullable.</span></span> <span data-ttu-id="ce5de-138">ユーザーと共有している[プラン](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="ce5de-138">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce5de-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce5de-139">JSON representation</span></span>
<span data-ttu-id="ce5de-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce5de-140">Here is a JSON representation of the resource.</span></span>

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
