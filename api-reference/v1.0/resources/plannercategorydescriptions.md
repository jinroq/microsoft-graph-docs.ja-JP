---
title: plannerCategoryDescriptions リソースの種類
description: '**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、計画の詳細オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1cf1ee1c6e8ccc4e90f78985b352062fce37df88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984347"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="6408a-105">plannerCategoryDescriptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6408a-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="6408a-p102">**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、[計画の詳細](plannerplandetails.md)オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="6408a-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="6408a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6408a-109">Properties</span></span>
| <span data-ttu-id="6408a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6408a-110">Property</span></span>     | <span data-ttu-id="6408a-111">型</span><span class="sxs-lookup"><span data-stu-id="6408a-111">Type</span></span>   |<span data-ttu-id="6408a-112">説明</span><span class="sxs-lookup"><span data-stu-id="6408a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6408a-113">category1</span><span class="sxs-lookup"><span data-stu-id="6408a-113">category1</span></span>|<span data-ttu-id="6408a-114">String</span><span class="sxs-lookup"><span data-stu-id="6408a-114">String</span></span>|<span data-ttu-id="6408a-115">Category 1 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="6408a-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="6408a-116">category2</span><span class="sxs-lookup"><span data-stu-id="6408a-116">category2</span></span>|<span data-ttu-id="6408a-117">String</span><span class="sxs-lookup"><span data-stu-id="6408a-117">String</span></span>|<span data-ttu-id="6408a-118">Category 2 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="6408a-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="6408a-119">category3</span><span class="sxs-lookup"><span data-stu-id="6408a-119">category3</span></span>|<span data-ttu-id="6408a-120">String</span><span class="sxs-lookup"><span data-stu-id="6408a-120">String</span></span>|<span data-ttu-id="6408a-121">Category 3 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="6408a-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="6408a-122">category4</span><span class="sxs-lookup"><span data-stu-id="6408a-122">category4</span></span>|<span data-ttu-id="6408a-123">String</span><span class="sxs-lookup"><span data-stu-id="6408a-123">String</span></span>|<span data-ttu-id="6408a-124">Category 4 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="6408a-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="6408a-125">category5</span><span class="sxs-lookup"><span data-stu-id="6408a-125">category5</span></span>|<span data-ttu-id="6408a-126">String</span><span class="sxs-lookup"><span data-stu-id="6408a-126">String</span></span>|<span data-ttu-id="6408a-127">Category 5 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="6408a-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="6408a-128">category6</span><span class="sxs-lookup"><span data-stu-id="6408a-128">category6</span></span>|<span data-ttu-id="6408a-129">String</span><span class="sxs-lookup"><span data-stu-id="6408a-129">String</span></span>|<span data-ttu-id="6408a-130">Category 6 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="6408a-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6408a-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6408a-131">JSON representation</span></span>
<span data-ttu-id="6408a-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6408a-132">Here is a JSON representation of the resource.</span></span>

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
