---
title: のリソースの種類
description: 1レベルののレベル
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dd8e67cbf4ba8994e03d683665928f9e62608d8e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173336"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="f86d4-103">のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="f86d4-103">rubricLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f86d4-104">1レベルの単位。</span><span class="sxs-lookup"><span data-stu-id="f86d4-104">A level of a rubric.</span></span> <span data-ttu-id="f86d4-105">EducationRubric については、「 [](educationrubric.md) 」を参照し\*\* てください\*\*。 \*\*</span><span class="sxs-lookup"><span data-stu-id="f86d4-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="f86d4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f86d4-106">Properties</span></span>

| <span data-ttu-id="f86d4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f86d4-107">Property</span></span>     | <span data-ttu-id="f86d4-108">型</span><span class="sxs-lookup"><span data-stu-id="f86d4-108">Type</span></span>        | <span data-ttu-id="f86d4-109">説明</span><span class="sxs-lookup"><span data-stu-id="f86d4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f86d4-110">description</span><span class="sxs-lookup"><span data-stu-id="f86d4-110">description</span></span>|[<span data-ttu-id="f86d4-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="f86d4-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="f86d4-112">このフォルダーの説明。</span><span class="sxs-lookup"><span data-stu-id="f86d4-112">The description of this rubric level.</span></span>|
|<span data-ttu-id="f86d4-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f86d4-113">displayName</span></span>|<span data-ttu-id="f86d4-114">String</span><span class="sxs-lookup"><span data-stu-id="f86d4-114">String</span></span>|<span data-ttu-id="f86d4-115">この名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="f86d4-115">The name of this rubric level.</span></span>|
|<span data-ttu-id="f86d4-116">変化</span><span class="sxs-lookup"><span data-stu-id="f86d4-116">grading</span></span>|[<span data-ttu-id="f86d4-117">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="f86d4-117">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="f86d4-118">これが非ポイントの場合は Null になります。[educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md)の場合は、この点を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f86d4-118">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="f86d4-119">levelId</span><span class="sxs-lookup"><span data-stu-id="f86d4-119">levelId</span></span>|<span data-ttu-id="f86d4-120">String</span><span class="sxs-lookup"><span data-stu-id="f86d4-120">String</span></span>|<span data-ttu-id="f86d4-121">このリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="f86d4-121">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f86d4-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f86d4-122">JSON representation</span></span>

<span data-ttu-id="f86d4-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f86d4-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricLevel",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "levelId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->