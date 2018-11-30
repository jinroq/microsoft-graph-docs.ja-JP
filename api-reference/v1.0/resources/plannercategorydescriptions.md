---
title: plannerCategoryDescriptions リソースの種類
description: '**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、計画の詳細オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。 '
ms.openlocfilehash: e71cbd1f41d23747691b3738b5a46ff302a72168
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021219"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="067ba-105">plannerCategoryDescriptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="067ba-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="067ba-p102">**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、[計画の詳細](plannerplandetails.md)オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="067ba-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="067ba-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="067ba-109">Properties</span></span>
| <span data-ttu-id="067ba-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="067ba-110">Property</span></span>     | <span data-ttu-id="067ba-111">型</span><span class="sxs-lookup"><span data-stu-id="067ba-111">Type</span></span>   |<span data-ttu-id="067ba-112">説明</span><span class="sxs-lookup"><span data-stu-id="067ba-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="067ba-113">category1</span><span class="sxs-lookup"><span data-stu-id="067ba-113">category1</span></span>|<span data-ttu-id="067ba-114">String</span><span class="sxs-lookup"><span data-stu-id="067ba-114">String</span></span>|<span data-ttu-id="067ba-115">Category 1 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="067ba-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="067ba-116">category2</span><span class="sxs-lookup"><span data-stu-id="067ba-116">category2</span></span>|<span data-ttu-id="067ba-117">String</span><span class="sxs-lookup"><span data-stu-id="067ba-117">String</span></span>|<span data-ttu-id="067ba-118">Category 2 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="067ba-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="067ba-119">category3</span><span class="sxs-lookup"><span data-stu-id="067ba-119">category3</span></span>|<span data-ttu-id="067ba-120">String</span><span class="sxs-lookup"><span data-stu-id="067ba-120">String</span></span>|<span data-ttu-id="067ba-121">Category 3 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="067ba-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="067ba-122">category4</span><span class="sxs-lookup"><span data-stu-id="067ba-122">category4</span></span>|<span data-ttu-id="067ba-123">String</span><span class="sxs-lookup"><span data-stu-id="067ba-123">String</span></span>|<span data-ttu-id="067ba-124">Category 4 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="067ba-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="067ba-125">category5</span><span class="sxs-lookup"><span data-stu-id="067ba-125">category5</span></span>|<span data-ttu-id="067ba-126">String</span><span class="sxs-lookup"><span data-stu-id="067ba-126">String</span></span>|<span data-ttu-id="067ba-127">Category 5 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="067ba-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="067ba-128">category6</span><span class="sxs-lookup"><span data-stu-id="067ba-128">category6</span></span>|<span data-ttu-id="067ba-129">String</span><span class="sxs-lookup"><span data-stu-id="067ba-129">String</span></span>|<span data-ttu-id="067ba-130">Category 6 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="067ba-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="067ba-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="067ba-131">JSON representation</span></span>
<span data-ttu-id="067ba-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="067ba-132">Here is a JSON representation of the resource.</span></span>

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