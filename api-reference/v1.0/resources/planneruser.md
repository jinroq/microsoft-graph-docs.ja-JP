---
title: plannerUser リソースの種類
description: '**PlannerUser**リソースでは、ユーザーの計画のリソースへのアクセスを提供します。 使用可能なプロパティが含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953564"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="84e94-104">plannerUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84e94-104">plannerUser resource type</span></span>

<span data-ttu-id="84e94-p102">**plannerUser** リソースは、[user](user.md) のプランナー リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="84e94-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="84e94-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="84e94-107">Methods</span></span>

| <span data-ttu-id="84e94-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="84e94-108">Method</span></span>           | <span data-ttu-id="84e94-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="84e94-109">Return Type</span></span>    |<span data-ttu-id="84e94-110">説明</span><span class="sxs-lookup"><span data-stu-id="84e94-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84e94-111">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="84e94-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="84e94-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="84e94-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="84e94-113">**plannerPlan** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="84e94-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="84e94-114">List tasks</span><span class="sxs-lookup"><span data-stu-id="84e94-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="84e94-115">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="84e94-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="84e94-116">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="84e94-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="84e94-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84e94-117">Properties</span></span>
| <span data-ttu-id="84e94-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84e94-118">Property</span></span>     | <span data-ttu-id="84e94-119">種類</span><span class="sxs-lookup"><span data-stu-id="84e94-119">Type</span></span>   |<span data-ttu-id="84e94-120">説明</span><span class="sxs-lookup"><span data-stu-id="84e94-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84e94-121">ID</span><span class="sxs-lookup"><span data-stu-id="84e94-121">id</span></span>|<span data-ttu-id="84e94-122">String</span><span class="sxs-lookup"><span data-stu-id="84e94-122">String</span></span>| <span data-ttu-id="84e94-p103">読み取り専用です。planenrUser の識別子</span><span class="sxs-lookup"><span data-stu-id="84e94-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="84e94-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="84e94-125">Relationships</span></span>
| <span data-ttu-id="84e94-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="84e94-126">Relationship</span></span> | <span data-ttu-id="84e94-127">型</span><span class="sxs-lookup"><span data-stu-id="84e94-127">Type</span></span>   |<span data-ttu-id="84e94-128">説明</span><span class="sxs-lookup"><span data-stu-id="84e94-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84e94-129">plans</span><span class="sxs-lookup"><span data-stu-id="84e94-129">plans</span></span>|<span data-ttu-id="84e94-130">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="84e94-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="84e94-p104">読み取り専用です。Null 許容型。ユーザーに割り当てられている [plannerTasks](plannertask.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="84e94-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="84e94-134">tasks</span><span class="sxs-lookup"><span data-stu-id="84e94-134">tasks</span></span>|<span data-ttu-id="84e94-135">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="84e94-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="84e94-p105">読み取り専用です。Null 許容型。ユーザーと共有している [plannerPlans](plannerplan.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="84e94-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84e94-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84e94-139">JSON representation</span></span>
<span data-ttu-id="84e94-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84e94-140">Here is a JSON representation of the resource.</span></span>

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
