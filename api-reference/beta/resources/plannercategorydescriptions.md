---
title: プラン? カテゴリの説明リソースの種類
description: 'プラン**** に対して定義されているカテゴリの説明的なラベルを表します。 プランの詳細オブジェクトに属します。 最大6つのカテゴリが定義されています。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a410f748c43d50872936d4bcc106ffeb224d76cf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344558"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="942c3-105">プラン? カテゴリの説明リソースの種類</span><span class="sxs-lookup"><span data-stu-id="942c3-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942c3-106">プラン\*\*\*\* に対して定義されているカテゴリの説明的なラベルを表します。</span><span class="sxs-lookup"><span data-stu-id="942c3-106">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="942c3-107">[プランの詳細](plannerplandetails.md)オブジェクトに属します。</span><span class="sxs-lookup"><span data-stu-id="942c3-107">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="942c3-108">最大6つのカテゴリが定義されています。</span><span class="sxs-lookup"><span data-stu-id="942c3-108">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="942c3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="942c3-109">Properties</span></span>
| <span data-ttu-id="942c3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="942c3-110">Property</span></span>     | <span data-ttu-id="942c3-111">型</span><span class="sxs-lookup"><span data-stu-id="942c3-111">Type</span></span>   |<span data-ttu-id="942c3-112">説明</span><span class="sxs-lookup"><span data-stu-id="942c3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="942c3-113">category1</span><span class="sxs-lookup"><span data-stu-id="942c3-113">category1</span></span>|<span data-ttu-id="942c3-114">String</span><span class="sxs-lookup"><span data-stu-id="942c3-114">String</span></span>|<span data-ttu-id="942c3-115">カテゴリ1に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="942c3-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="942c3-116">category2</span><span class="sxs-lookup"><span data-stu-id="942c3-116">category2</span></span>|<span data-ttu-id="942c3-117">String</span><span class="sxs-lookup"><span data-stu-id="942c3-117">String</span></span>|<span data-ttu-id="942c3-118">カテゴリ2に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="942c3-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="942c3-119">category3</span><span class="sxs-lookup"><span data-stu-id="942c3-119">category3</span></span>|<span data-ttu-id="942c3-120">String</span><span class="sxs-lookup"><span data-stu-id="942c3-120">String</span></span>|<span data-ttu-id="942c3-121">カテゴリ3に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="942c3-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="942c3-122">category4</span><span class="sxs-lookup"><span data-stu-id="942c3-122">category4</span></span>|<span data-ttu-id="942c3-123">String</span><span class="sxs-lookup"><span data-stu-id="942c3-123">String</span></span>|<span data-ttu-id="942c3-124">Category 4 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="942c3-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="942c3-125">category5</span><span class="sxs-lookup"><span data-stu-id="942c3-125">category5</span></span>|<span data-ttu-id="942c3-126">String</span><span class="sxs-lookup"><span data-stu-id="942c3-126">String</span></span>|<span data-ttu-id="942c3-127">カテゴリ5に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="942c3-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="942c3-128">category6</span><span class="sxs-lookup"><span data-stu-id="942c3-128">category6</span></span>|<span data-ttu-id="942c3-129">String</span><span class="sxs-lookup"><span data-stu-id="942c3-129">String</span></span>|<span data-ttu-id="942c3-130">カテゴリ6に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="942c3-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="942c3-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="942c3-131">JSON representation</span></span>
<span data-ttu-id="942c3-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="942c3-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
