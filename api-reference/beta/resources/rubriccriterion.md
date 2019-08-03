---
title: 検索基準リソースの種類
description: 検索基準 (標準)
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 250132ab5304ab9df94707349df951e5b1e995a6
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173343"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="2f197-103">検索基準リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f197-103">rubricCriterion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f197-104">検索基準を示します。</span><span class="sxs-lookup"><span data-stu-id="2f197-104">A criterion of a rubric.</span></span> <span data-ttu-id="2f197-105">EducationRubric については、「 [](educationrubric.md) 」を参照し\*\* てください\*\*。 \*\*</span><span class="sxs-lookup"><span data-stu-id="2f197-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="2f197-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f197-106">Properties</span></span>

| <span data-ttu-id="2f197-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f197-107">Property</span></span>     | <span data-ttu-id="2f197-108">型</span><span class="sxs-lookup"><span data-stu-id="2f197-108">Type</span></span>        | <span data-ttu-id="2f197-109">説明</span><span class="sxs-lookup"><span data-stu-id="2f197-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f197-110">description</span><span class="sxs-lookup"><span data-stu-id="2f197-110">description</span></span>|[<span data-ttu-id="2f197-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="2f197-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="2f197-112">この条件の説明。</span><span class="sxs-lookup"><span data-stu-id="2f197-112">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f197-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f197-113">JSON representation</span></span>

<span data-ttu-id="2f197-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f197-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricCriterion",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricCriterion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->