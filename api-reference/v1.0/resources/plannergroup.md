---
title: plannerGroup リソースの種類
description: '**PlannerGroup**リソースでは、グループの計画のリソースへのアクセスを提供します。 使用可能なプロパティが含まれていません。'
localization_priority: Normal
ms.openlocfilehash: ac55c0acd3561205654383cbb1b3d264c219d1a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871968"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="c80fc-104">plannerGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c80fc-104">plannerGroup resource type</span></span>

<span data-ttu-id="c80fc-p102">**plannerGroup** リソースは、[group](group.md) の Planner リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="c80fc-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="c80fc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c80fc-107">Methods</span></span>

| <span data-ttu-id="c80fc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c80fc-108">Method</span></span>           | <span data-ttu-id="c80fc-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c80fc-109">Return Type</span></span>    |<span data-ttu-id="c80fc-110">説明</span><span class="sxs-lookup"><span data-stu-id="c80fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c80fc-111">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c80fc-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="c80fc-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c80fc-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c80fc-113">**plannerPlan** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c80fc-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="c80fc-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c80fc-114">Properties</span></span>
| <span data-ttu-id="c80fc-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c80fc-115">Property</span></span>     | <span data-ttu-id="c80fc-116">種類</span><span class="sxs-lookup"><span data-stu-id="c80fc-116">Type</span></span>   |<span data-ttu-id="c80fc-117">説明</span><span class="sxs-lookup"><span data-stu-id="c80fc-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c80fc-118">ID</span><span class="sxs-lookup"><span data-stu-id="c80fc-118">id</span></span>|<span data-ttu-id="c80fc-119">String</span><span class="sxs-lookup"><span data-stu-id="c80fc-119">String</span></span>| <span data-ttu-id="c80fc-p103">読み取り専用です。**plannerGroup** の識別子</span><span class="sxs-lookup"><span data-stu-id="c80fc-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="c80fc-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c80fc-122">Relationships</span></span>
| <span data-ttu-id="c80fc-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c80fc-123">Relationship</span></span> | <span data-ttu-id="c80fc-124">型</span><span class="sxs-lookup"><span data-stu-id="c80fc-124">Type</span></span>   |<span data-ttu-id="c80fc-125">説明</span><span class="sxs-lookup"><span data-stu-id="c80fc-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c80fc-126">plans</span><span class="sxs-lookup"><span data-stu-id="c80fc-126">plans</span></span>|<span data-ttu-id="c80fc-127">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c80fc-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c80fc-p104">読み取り専用です。Null 許容型。グループが所有する [plannerPlans](plannerplan.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="c80fc-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c80fc-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c80fc-131">JSON representation</span></span>
<span data-ttu-id="c80fc-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c80fc-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
