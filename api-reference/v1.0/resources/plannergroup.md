---
title: plannerGroup リソースの種類
description: '**PlannerGroup**リソースでは、グループの計画のリソースへのアクセスを提供します。 使用可能なプロパティが含まれていません。'
ms.openlocfilehash: 3a2bb9cfd90a36f6b0a2148e0d789ac97b2199fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022655"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="24aca-104">plannerGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24aca-104">plannerGroup resource type</span></span>

<span data-ttu-id="24aca-p102">**plannerGroup** リソースは、[group](group.md) の Planner リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="24aca-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="24aca-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="24aca-107">Methods</span></span>

| <span data-ttu-id="24aca-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="24aca-108">Method</span></span>           | <span data-ttu-id="24aca-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="24aca-109">Return Type</span></span>    |<span data-ttu-id="24aca-110">説明</span><span class="sxs-lookup"><span data-stu-id="24aca-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24aca-111">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="24aca-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="24aca-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="24aca-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="24aca-113">**plannerPlan** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="24aca-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="24aca-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24aca-114">Properties</span></span>
| <span data-ttu-id="24aca-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24aca-115">Property</span></span>     | <span data-ttu-id="24aca-116">型</span><span class="sxs-lookup"><span data-stu-id="24aca-116">Type</span></span>   |<span data-ttu-id="24aca-117">説明</span><span class="sxs-lookup"><span data-stu-id="24aca-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24aca-118">id</span><span class="sxs-lookup"><span data-stu-id="24aca-118">id</span></span>|<span data-ttu-id="24aca-119">String</span><span class="sxs-lookup"><span data-stu-id="24aca-119">String</span></span>| <span data-ttu-id="24aca-p103">読み取り専用です。**plannerGroup** の識別子</span><span class="sxs-lookup"><span data-stu-id="24aca-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="24aca-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24aca-122">Relationships</span></span>
| <span data-ttu-id="24aca-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24aca-123">Relationship</span></span> | <span data-ttu-id="24aca-124">型</span><span class="sxs-lookup"><span data-stu-id="24aca-124">Type</span></span>   |<span data-ttu-id="24aca-125">説明</span><span class="sxs-lookup"><span data-stu-id="24aca-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24aca-126">plans</span><span class="sxs-lookup"><span data-stu-id="24aca-126">plans</span></span>|<span data-ttu-id="24aca-127">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="24aca-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="24aca-p104">読み取り専用です。Null 許容型。グループが所有する [plannerPlans](plannerplan.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="24aca-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24aca-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24aca-131">JSON representation</span></span>
<span data-ttu-id="24aca-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24aca-132">Here is a JSON representation of the resource.</span></span>

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