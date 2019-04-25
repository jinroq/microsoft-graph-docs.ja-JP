---
title: プラン? カテゴリの説明リソースの種類
description: 'プラン**** に対して定義されているカテゴリの説明的なラベルを表します。 プランの詳細オブジェクトに属します。 最大6つのカテゴリが定義されています。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 33031dc3c688e1fefb34109cb0a4a303dbe1c183
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579031"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="d85f0-105">プラン? カテゴリの説明リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d85f0-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d85f0-106">プラン\*\*\*\* に対して定義されているカテゴリの説明的なラベルを表します。</span><span class="sxs-lookup"><span data-stu-id="d85f0-106">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="d85f0-107">[プランの詳細](plannerplandetails.md)オブジェクトに属します。</span><span class="sxs-lookup"><span data-stu-id="d85f0-107">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="d85f0-108">最大6つのカテゴリが定義されています。</span><span class="sxs-lookup"><span data-stu-id="d85f0-108">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="d85f0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d85f0-109">Properties</span></span>
| <span data-ttu-id="d85f0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d85f0-110">Property</span></span>     | <span data-ttu-id="d85f0-111">型</span><span class="sxs-lookup"><span data-stu-id="d85f0-111">Type</span></span>   |<span data-ttu-id="d85f0-112">説明</span><span class="sxs-lookup"><span data-stu-id="d85f0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d85f0-113">category1</span><span class="sxs-lookup"><span data-stu-id="d85f0-113">category1</span></span>|<span data-ttu-id="d85f0-114">String</span><span class="sxs-lookup"><span data-stu-id="d85f0-114">String</span></span>|<span data-ttu-id="d85f0-115">カテゴリ1に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="d85f0-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="d85f0-116">category2</span><span class="sxs-lookup"><span data-stu-id="d85f0-116">category2</span></span>|<span data-ttu-id="d85f0-117">String</span><span class="sxs-lookup"><span data-stu-id="d85f0-117">String</span></span>|<span data-ttu-id="d85f0-118">カテゴリ2に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="d85f0-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="d85f0-119">category3</span><span class="sxs-lookup"><span data-stu-id="d85f0-119">category3</span></span>|<span data-ttu-id="d85f0-120">String</span><span class="sxs-lookup"><span data-stu-id="d85f0-120">String</span></span>|<span data-ttu-id="d85f0-121">カテゴリ3に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="d85f0-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="d85f0-122">category4</span><span class="sxs-lookup"><span data-stu-id="d85f0-122">category4</span></span>|<span data-ttu-id="d85f0-123">String</span><span class="sxs-lookup"><span data-stu-id="d85f0-123">String</span></span>|<span data-ttu-id="d85f0-124">Category 4 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="d85f0-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="d85f0-125">category5</span><span class="sxs-lookup"><span data-stu-id="d85f0-125">category5</span></span>|<span data-ttu-id="d85f0-126">String</span><span class="sxs-lookup"><span data-stu-id="d85f0-126">String</span></span>|<span data-ttu-id="d85f0-127">カテゴリ5に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="d85f0-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="d85f0-128">category6</span><span class="sxs-lookup"><span data-stu-id="d85f0-128">category6</span></span>|<span data-ttu-id="d85f0-129">String</span><span class="sxs-lookup"><span data-stu-id="d85f0-129">String</span></span>|<span data-ttu-id="d85f0-130">カテゴリ6に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="d85f0-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d85f0-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d85f0-131">JSON representation</span></span>
<span data-ttu-id="d85f0-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d85f0-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannercategorydescriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
