---
title: plannerUser リソースの種類
description: '**PlannerUser**リソースでは、ユーザーの計画のリソースへのアクセスを提供します。 使用可能なプロパティが含まれていません。'
localization_priority: Normal
ms.openlocfilehash: 733c20d45e1c0b1e0e454b2c5ae03105a9ab5d24
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805944"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="1bd6e-104">plannerUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1bd6e-104">plannerUser resource type</span></span>

<span data-ttu-id="1bd6e-p102">**plannerUser** リソースは、[user](user.md) のプランナー リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="1bd6e-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="1bd6e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1bd6e-107">Methods</span></span>

| <span data-ttu-id="1bd6e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1bd6e-108">Method</span></span>           | <span data-ttu-id="1bd6e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1bd6e-109">Return Type</span></span>    |<span data-ttu-id="1bd6e-110">説明</span><span class="sxs-lookup"><span data-stu-id="1bd6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1bd6e-111">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1bd6e-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="1bd6e-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1bd6e-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1bd6e-113">**plannerPlan** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1bd6e-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="1bd6e-114">List tasks</span><span class="sxs-lookup"><span data-stu-id="1bd6e-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="1bd6e-115">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1bd6e-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1bd6e-116">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1bd6e-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="1bd6e-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bd6e-117">Properties</span></span>
| <span data-ttu-id="1bd6e-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bd6e-118">Property</span></span>     | <span data-ttu-id="1bd6e-119">種類</span><span class="sxs-lookup"><span data-stu-id="1bd6e-119">Type</span></span>   |<span data-ttu-id="1bd6e-120">説明</span><span class="sxs-lookup"><span data-stu-id="1bd6e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bd6e-121">ID</span><span class="sxs-lookup"><span data-stu-id="1bd6e-121">id</span></span>|<span data-ttu-id="1bd6e-122">String</span><span class="sxs-lookup"><span data-stu-id="1bd6e-122">String</span></span>| <span data-ttu-id="1bd6e-p103">読み取り専用です。planenrUser の識別子</span><span class="sxs-lookup"><span data-stu-id="1bd6e-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bd6e-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1bd6e-125">Relationships</span></span>
| <span data-ttu-id="1bd6e-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1bd6e-126">Relationship</span></span> | <span data-ttu-id="1bd6e-127">型</span><span class="sxs-lookup"><span data-stu-id="1bd6e-127">Type</span></span>   |<span data-ttu-id="1bd6e-128">説明</span><span class="sxs-lookup"><span data-stu-id="1bd6e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bd6e-129">plans</span><span class="sxs-lookup"><span data-stu-id="1bd6e-129">plans</span></span>|<span data-ttu-id="1bd6e-130">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1bd6e-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1bd6e-p104">読み取り専用です。Null 許容型。ユーザーに割り当てられている [plannerTasks](plannertask.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="1bd6e-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="1bd6e-134">tasks</span><span class="sxs-lookup"><span data-stu-id="1bd6e-134">tasks</span></span>|<span data-ttu-id="1bd6e-135">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1bd6e-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1bd6e-p105">読み取り専用です。Null 許容型。ユーザーと共有している [plannerPlans](plannerplan.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="1bd6e-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1bd6e-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1bd6e-139">JSON representation</span></span>
<span data-ttu-id="1bd6e-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1bd6e-140">Here is a JSON representation of the resource.</span></span>

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
