---
title: plan グループリソースの種類
description: '**plan グループ**リソースは、グループの Planner リソースへのアクセスを提供します。 使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 043cec9c3953f8c78a37e141a7b0f1259eb89d52
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344481"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="8f774-104">plan グループリソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f774-104">plannerGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f774-105">**plan グループ**リソースは、[グループ](group.md)の Planner リソースへのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="8f774-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="8f774-106">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="8f774-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="8f774-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f774-107">Methods</span></span>

| <span data-ttu-id="8f774-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f774-108">Method</span></span>           | <span data-ttu-id="8f774-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8f774-109">Return Type</span></span>    |<span data-ttu-id="8f774-110">説明</span><span class="sxs-lookup"><span data-stu-id="8f774-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f774-111">計画を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8f774-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="8f774-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8f774-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8f774-113">**プラン**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8f774-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f774-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f774-114">Properties</span></span>
| <span data-ttu-id="8f774-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f774-115">Property</span></span>     | <span data-ttu-id="8f774-116">型</span><span class="sxs-lookup"><span data-stu-id="8f774-116">Type</span></span>   |<span data-ttu-id="8f774-117">説明</span><span class="sxs-lookup"><span data-stu-id="8f774-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f774-118">id</span><span class="sxs-lookup"><span data-stu-id="8f774-118">id</span></span>|<span data-ttu-id="8f774-119">String</span><span class="sxs-lookup"><span data-stu-id="8f774-119">String</span></span>| <span data-ttu-id="8f774-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8f774-120">Read-only.</span></span> <span data-ttu-id="8f774-121">**plan グループ**の識別子</span><span class="sxs-lookup"><span data-stu-id="8f774-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f774-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8f774-122">Relationships</span></span>
| <span data-ttu-id="8f774-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8f774-123">Relationship</span></span> | <span data-ttu-id="8f774-124">型</span><span class="sxs-lookup"><span data-stu-id="8f774-124">Type</span></span>   |<span data-ttu-id="8f774-125">説明</span><span class="sxs-lookup"><span data-stu-id="8f774-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f774-126">plans</span><span class="sxs-lookup"><span data-stu-id="8f774-126">plans</span></span>|<span data-ttu-id="8f774-127">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8f774-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8f774-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8f774-128">Read-only.</span></span> <span data-ttu-id="8f774-129">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="8f774-129">Nullable.</span></span> <span data-ttu-id="8f774-130">グループが所有している[plan プラン](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="8f774-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f774-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f774-131">JSON representation</span></span>
<span data-ttu-id="8f774-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8f774-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
