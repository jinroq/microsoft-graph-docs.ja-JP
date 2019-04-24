---
title: plan グループリソースの種類
description: '**plan グループ**リソースは、グループの Planner リソースへのアクセスを提供します。 使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457033"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="a83bd-104">plan グループリソースの種類</span><span class="sxs-lookup"><span data-stu-id="a83bd-104">plannerGroup resource type</span></span>

<span data-ttu-id="a83bd-105">**plan グループ**リソースは、[グループ](group.md)の Planner リソースへのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="a83bd-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="a83bd-106">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="a83bd-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="a83bd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a83bd-107">Methods</span></span>

| <span data-ttu-id="a83bd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a83bd-108">Method</span></span>           | <span data-ttu-id="a83bd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a83bd-109">Return Type</span></span>    |<span data-ttu-id="a83bd-110">説明</span><span class="sxs-lookup"><span data-stu-id="a83bd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a83bd-111">計画を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a83bd-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="a83bd-112">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a83bd-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="a83bd-113">**プラン**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a83bd-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a83bd-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a83bd-114">Properties</span></span>
| <span data-ttu-id="a83bd-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a83bd-115">Property</span></span>     | <span data-ttu-id="a83bd-116">型</span><span class="sxs-lookup"><span data-stu-id="a83bd-116">Type</span></span>   |<span data-ttu-id="a83bd-117">説明</span><span class="sxs-lookup"><span data-stu-id="a83bd-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a83bd-118">id</span><span class="sxs-lookup"><span data-stu-id="a83bd-118">id</span></span>|<span data-ttu-id="a83bd-119">String</span><span class="sxs-lookup"><span data-stu-id="a83bd-119">String</span></span>| <span data-ttu-id="a83bd-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a83bd-120">Read-only.</span></span> <span data-ttu-id="a83bd-121">**plan グループ**の識別子</span><span class="sxs-lookup"><span data-stu-id="a83bd-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="a83bd-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a83bd-122">Relationships</span></span>
| <span data-ttu-id="a83bd-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a83bd-123">Relationship</span></span> | <span data-ttu-id="a83bd-124">型</span><span class="sxs-lookup"><span data-stu-id="a83bd-124">Type</span></span>   |<span data-ttu-id="a83bd-125">説明</span><span class="sxs-lookup"><span data-stu-id="a83bd-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a83bd-126">plans</span><span class="sxs-lookup"><span data-stu-id="a83bd-126">plans</span></span>|<span data-ttu-id="a83bd-127">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a83bd-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="a83bd-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a83bd-128">Read-only.</span></span> <span data-ttu-id="a83bd-129">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a83bd-129">Nullable.</span></span> <span data-ttu-id="a83bd-130">グループが所有している[plan プラン](plannerplan.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="a83bd-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a83bd-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a83bd-131">JSON representation</span></span>
<span data-ttu-id="a83bd-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a83bd-132">Here is a JSON representation of the resource.</span></span>

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
