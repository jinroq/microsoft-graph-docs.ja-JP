---
title: plannerGroup リソースの種類
description: '**PlannerGroup**リソースでは、グループの計画のリソースへのアクセスを提供します。 使用可能なプロパティが含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 54b6b1d61a98aae3918fd3fcb888f470179ece15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961709"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="b9bcf-104">plannerGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9bcf-104">plannerGroup resource type</span></span>

> <span data-ttu-id="b9bcf-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b9bcf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9bcf-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9bcf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9bcf-p103">**plannerGroup** リソースは、[group](group.md) の Planner リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="b9bcf-p103">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="b9bcf-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b9bcf-109">Methods</span></span>

| <span data-ttu-id="b9bcf-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="b9bcf-110">Method</span></span>           | <span data-ttu-id="b9bcf-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b9bcf-111">Return Type</span></span>    |<span data-ttu-id="b9bcf-112">説明</span><span class="sxs-lookup"><span data-stu-id="b9bcf-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b9bcf-113">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b9bcf-113">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="b9bcf-114">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b9bcf-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="b9bcf-115">**plannerPlan** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b9bcf-115">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="b9bcf-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9bcf-116">Properties</span></span>
| <span data-ttu-id="b9bcf-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9bcf-117">Property</span></span>     | <span data-ttu-id="b9bcf-118">種類</span><span class="sxs-lookup"><span data-stu-id="b9bcf-118">Type</span></span>   |<span data-ttu-id="b9bcf-119">説明</span><span class="sxs-lookup"><span data-stu-id="b9bcf-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9bcf-120">ID</span><span class="sxs-lookup"><span data-stu-id="b9bcf-120">id</span></span>|<span data-ttu-id="b9bcf-121">String</span><span class="sxs-lookup"><span data-stu-id="b9bcf-121">String</span></span>| <span data-ttu-id="b9bcf-p104">読み取り専用です。**plannerGroup** の識別子</span><span class="sxs-lookup"><span data-stu-id="b9bcf-p104">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9bcf-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b9bcf-124">Relationships</span></span>
| <span data-ttu-id="b9bcf-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b9bcf-125">Relationship</span></span> | <span data-ttu-id="b9bcf-126">型</span><span class="sxs-lookup"><span data-stu-id="b9bcf-126">Type</span></span>   |<span data-ttu-id="b9bcf-127">説明</span><span class="sxs-lookup"><span data-stu-id="b9bcf-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9bcf-128">plans</span><span class="sxs-lookup"><span data-stu-id="b9bcf-128">plans</span></span>|<span data-ttu-id="b9bcf-129">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b9bcf-129">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="b9bcf-p105">読み取り専用です。Null 許容型。グループが所有する [plannerPlans](plannerplan.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="b9bcf-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9bcf-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9bcf-133">JSON representation</span></span>
<span data-ttu-id="b9bcf-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b9bcf-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
