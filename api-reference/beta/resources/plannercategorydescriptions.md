---
title: plannerCategoryDescriptions リソースの種類
description: '**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、計画の詳細オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。 '
ms.openlocfilehash: eb54a42cd3e86a9f2c39ff46d45c71fb04142dad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068346"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="65c4a-105">plannerCategoryDescriptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65c4a-105">plannerCategoryDescriptions resource type</span></span>

> <span data-ttu-id="65c4a-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65c4a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65c4a-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65c4a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65c4a-p103">**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、[計画の詳細](plannerplandetails.md)オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="65c4a-p103">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="65c4a-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65c4a-111">Properties</span></span>
| <span data-ttu-id="65c4a-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65c4a-112">Property</span></span>     | <span data-ttu-id="65c4a-113">型</span><span class="sxs-lookup"><span data-stu-id="65c4a-113">Type</span></span>   |<span data-ttu-id="65c4a-114">説明</span><span class="sxs-lookup"><span data-stu-id="65c4a-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65c4a-115">category1</span><span class="sxs-lookup"><span data-stu-id="65c4a-115">category1</span></span>|<span data-ttu-id="65c4a-116">String</span><span class="sxs-lookup"><span data-stu-id="65c4a-116">String</span></span>|<span data-ttu-id="65c4a-117">Category 1 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="65c4a-117">The label associated with Category 1</span></span>|
|<span data-ttu-id="65c4a-118">category2</span><span class="sxs-lookup"><span data-stu-id="65c4a-118">category2</span></span>|<span data-ttu-id="65c4a-119">String</span><span class="sxs-lookup"><span data-stu-id="65c4a-119">String</span></span>|<span data-ttu-id="65c4a-120">Category 2 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="65c4a-120">The label associated with Category 2</span></span>|
|<span data-ttu-id="65c4a-121">category3</span><span class="sxs-lookup"><span data-stu-id="65c4a-121">category3</span></span>|<span data-ttu-id="65c4a-122">String</span><span class="sxs-lookup"><span data-stu-id="65c4a-122">String</span></span>|<span data-ttu-id="65c4a-123">Category 3 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="65c4a-123">The label associated with Category 3</span></span>|
|<span data-ttu-id="65c4a-124">category4</span><span class="sxs-lookup"><span data-stu-id="65c4a-124">category4</span></span>|<span data-ttu-id="65c4a-125">String</span><span class="sxs-lookup"><span data-stu-id="65c4a-125">String</span></span>|<span data-ttu-id="65c4a-126">Category 4 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="65c4a-126">The label associated with Category 4</span></span>|
|<span data-ttu-id="65c4a-127">category5</span><span class="sxs-lookup"><span data-stu-id="65c4a-127">category5</span></span>|<span data-ttu-id="65c4a-128">String</span><span class="sxs-lookup"><span data-stu-id="65c4a-128">String</span></span>|<span data-ttu-id="65c4a-129">Category 5 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="65c4a-129">The label associated with Category 5</span></span>|
|<span data-ttu-id="65c4a-130">category6</span><span class="sxs-lookup"><span data-stu-id="65c4a-130">category6</span></span>|<span data-ttu-id="65c4a-131">String</span><span class="sxs-lookup"><span data-stu-id="65c4a-131">String</span></span>|<span data-ttu-id="65c4a-132">Category 6 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="65c4a-132">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65c4a-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65c4a-133">JSON representation</span></span>
<span data-ttu-id="65c4a-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65c4a-134">Here is a JSON representation of the resource.</span></span>

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