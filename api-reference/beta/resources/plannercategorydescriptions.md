---
title: plannerCategoryDescriptions リソースの種類
description: '**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、計画の詳細オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4175692182d115e884642ef8f9956cc4db5dae2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930944"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="78df3-105">plannerCategoryDescriptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78df3-105">plannerCategoryDescriptions resource type</span></span>

> <span data-ttu-id="78df3-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78df3-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78df3-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78df3-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78df3-p103">**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、[計画の詳細](plannerplandetails.md)オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="78df3-p103">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="78df3-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78df3-111">Properties</span></span>
| <span data-ttu-id="78df3-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78df3-112">Property</span></span>     | <span data-ttu-id="78df3-113">種類</span><span class="sxs-lookup"><span data-stu-id="78df3-113">Type</span></span>   |<span data-ttu-id="78df3-114">説明</span><span class="sxs-lookup"><span data-stu-id="78df3-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78df3-115">category1</span><span class="sxs-lookup"><span data-stu-id="78df3-115">category1</span></span>|<span data-ttu-id="78df3-116">String</span><span class="sxs-lookup"><span data-stu-id="78df3-116">String</span></span>|<span data-ttu-id="78df3-117">Category 1 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="78df3-117">The label associated with Category 1</span></span>|
|<span data-ttu-id="78df3-118">category2</span><span class="sxs-lookup"><span data-stu-id="78df3-118">category2</span></span>|<span data-ttu-id="78df3-119">String</span><span class="sxs-lookup"><span data-stu-id="78df3-119">String</span></span>|<span data-ttu-id="78df3-120">Category 2 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="78df3-120">The label associated with Category 2</span></span>|
|<span data-ttu-id="78df3-121">category3</span><span class="sxs-lookup"><span data-stu-id="78df3-121">category3</span></span>|<span data-ttu-id="78df3-122">String</span><span class="sxs-lookup"><span data-stu-id="78df3-122">String</span></span>|<span data-ttu-id="78df3-123">Category 3 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="78df3-123">The label associated with Category 3</span></span>|
|<span data-ttu-id="78df3-124">category4</span><span class="sxs-lookup"><span data-stu-id="78df3-124">category4</span></span>|<span data-ttu-id="78df3-125">String</span><span class="sxs-lookup"><span data-stu-id="78df3-125">String</span></span>|<span data-ttu-id="78df3-126">Category 4 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="78df3-126">The label associated with Category 4</span></span>|
|<span data-ttu-id="78df3-127">category5</span><span class="sxs-lookup"><span data-stu-id="78df3-127">category5</span></span>|<span data-ttu-id="78df3-128">String</span><span class="sxs-lookup"><span data-stu-id="78df3-128">String</span></span>|<span data-ttu-id="78df3-129">Category 5 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="78df3-129">The label associated with Category 5</span></span>|
|<span data-ttu-id="78df3-130">category6</span><span class="sxs-lookup"><span data-stu-id="78df3-130">category6</span></span>|<span data-ttu-id="78df3-131">String</span><span class="sxs-lookup"><span data-stu-id="78df3-131">String</span></span>|<span data-ttu-id="78df3-132">Category 6 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="78df3-132">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78df3-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78df3-133">JSON representation</span></span>
<span data-ttu-id="78df3-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78df3-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
