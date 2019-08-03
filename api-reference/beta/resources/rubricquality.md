---
title: リソースの種類 (最高)
description: の品質 (最高)
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e63fd8ad7aa7d0a19fe1774e18bba5d59af52140
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173308"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="94d18-103">リソースの種類 (最高)</span><span class="sxs-lookup"><span data-stu-id="94d18-103">rubricQuality resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d18-104">高品質 (最高)</span><span class="sxs-lookup"><span data-stu-id="94d18-104">A quality of a rubric.</span></span> <span data-ttu-id="94d18-105">EducationRubric については、「 [](educationrubric.md) 」を参照し\*\* てください\*\*。 \*\*</span><span class="sxs-lookup"><span data-stu-id="94d18-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="94d18-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94d18-106">Properties</span></span>

| <span data-ttu-id="94d18-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94d18-107">Property</span></span>     | <span data-ttu-id="94d18-108">型</span><span class="sxs-lookup"><span data-stu-id="94d18-108">Type</span></span>        | <span data-ttu-id="94d18-109">説明</span><span class="sxs-lookup"><span data-stu-id="94d18-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94d18-110">criteria</span><span class="sxs-lookup"><span data-stu-id="94d18-110">criteria</span></span>|<span data-ttu-id="94d18-111">の[条件](rubriccriterion.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="94d18-111">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="94d18-112">この検索基準のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="94d18-112">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="94d18-113">description</span><span class="sxs-lookup"><span data-stu-id="94d18-113">description</span></span>|[<span data-ttu-id="94d18-114">itemBody</span><span class="sxs-lookup"><span data-stu-id="94d18-114">itemBody</span></span>](itembody.md)|<span data-ttu-id="94d18-115">このテンプレートの説明。</span><span class="sxs-lookup"><span data-stu-id="94d18-115">The description of this rubric quality.</span></span>|
|<span data-ttu-id="94d18-116">displayName</span><span class="sxs-lookup"><span data-stu-id="94d18-116">displayName</span></span>|<span data-ttu-id="94d18-117">String</span><span class="sxs-lookup"><span data-stu-id="94d18-117">String</span></span>|<span data-ttu-id="94d18-118">この名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="94d18-118">The name of this rubric quality.</span></span>|
|<span data-ttu-id="94d18-119">qualityId</span><span class="sxs-lookup"><span data-stu-id="94d18-119">qualityId</span></span>|<span data-ttu-id="94d18-120">String</span><span class="sxs-lookup"><span data-stu-id="94d18-120">String</span></span>|<span data-ttu-id="94d18-121">このリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="94d18-121">The ID of this resource.</span></span>|
|<span data-ttu-id="94d18-122">weight</span><span class="sxs-lookup"><span data-stu-id="94d18-122">weight</span></span>|<span data-ttu-id="94d18-123">1 行</span><span class="sxs-lookup"><span data-stu-id="94d18-123">Single</span></span>|<span data-ttu-id="94d18-124">存在する場合は、この品質の数値ウェイトを指定します。</span><span class="sxs-lookup"><span data-stu-id="94d18-124">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="94d18-125">重みは100まで追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94d18-125">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94d18-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="94d18-126">JSON representation</span></span>

<span data-ttu-id="94d18-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94d18-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->