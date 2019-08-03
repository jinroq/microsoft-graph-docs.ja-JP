---
title: rubricQualityFeedbackModel リソースの種類
description: EducationRubric の特定の品質に関連するフィードバック
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0a7c2b80a2cef18b50157ae9a54c66d35822fa51
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173301"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="e740b-103">rubricQualityFeedbackModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e740b-103">rubricQualityFeedbackModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e740b-104">[EducationRubric](educationrubric.md)の特定の[品質](rubricquality.md)に関連するフィードバック。</span><span class="sxs-lookup"><span data-stu-id="e740b-104">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e740b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e740b-105">Properties</span></span>

| <span data-ttu-id="e740b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e740b-106">Property</span></span>     | <span data-ttu-id="e740b-107">型</span><span class="sxs-lookup"><span data-stu-id="e740b-107">Type</span></span>        | <span data-ttu-id="e740b-108">説明</span><span class="sxs-lookup"><span data-stu-id="e740b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e740b-109">feedback</span><span class="sxs-lookup"><span data-stu-id="e740b-109">feedback</span></span>|[<span data-ttu-id="e740b-110">itemBody</span><span class="sxs-lookup"><span data-stu-id="e740b-110">itemBody</span></span>](itembody.md)|<span data-ttu-id="e740b-111">この1つの品質に関する特定のフィードバック。</span><span class="sxs-lookup"><span data-stu-id="e740b-111">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="e740b-112">qualityId</span><span class="sxs-lookup"><span data-stu-id="e740b-112">qualityId</span></span>|<span data-ttu-id="e740b-113">String</span><span class="sxs-lookup"><span data-stu-id="e740b-113">String</span></span>|<span data-ttu-id="e740b-114">このフィードバックが関連付け[](rubricquality.md)られている、の ID。</span><span class="sxs-lookup"><span data-stu-id="e740b-114">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e740b-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e740b-115">JSON representation</span></span>

<span data-ttu-id="e740b-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e740b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualityFeedbackModel",
  "baseType": null
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.itemBody"},
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualityFeedbackModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->