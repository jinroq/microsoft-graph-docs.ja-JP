---
title: rubricQualitySelectedColumnModel リソースの種類
description: EducationRubric の優先度を指定するときに教師が選択したかどうかを示します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6fd6ff5d9def23a6a6fb180c8d12398437e5dce0
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173294"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="a2a2e-103">rubricQualitySelectedColumnModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2a2e-103">rubricQualitySelectedColumnModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2a2e-104">[EducationRubric](educationrubric.md)の優先[度](rubriclevel.md)を指定するときに教師によって選択されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a2a2e-104">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a2a2e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2a2e-105">Properties</span></span>

| <span data-ttu-id="a2a2e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2a2e-106">Property</span></span>     | <span data-ttu-id="a2a2e-107">型</span><span class="sxs-lookup"><span data-stu-id="a2a2e-107">Type</span></span>        | <span data-ttu-id="a2a2e-108">説明</span><span class="sxs-lookup"><span data-stu-id="a2a2e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2a2e-109">columnId</span><span class="sxs-lookup"><span data-stu-id="a2a2e-109">columnId</span></span>|<span data-ttu-id="a2a2e-110">String</span><span class="sxs-lookup"><span data-stu-id="a2a2e-110">String</span></span>|<span data-ttu-id="a2a2e-111">この品質の選択されたレベルの ID。</span><span class="sxs-lookup"><span data-stu-id="a2a2e-111">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="a2a2e-112">qualityId</span><span class="sxs-lookup"><span data-stu-id="a2a2e-112">qualityId</span></span>|<span data-ttu-id="a2a2e-113">String</span><span class="sxs-lookup"><span data-stu-id="a2a2e-113">String</span></span>|<span data-ttu-id="a2a2e-114">関連付けられている品質の ID です。</span><span class="sxs-lookup"><span data-stu-id="a2a2e-114">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2a2e-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2a2e-115">JSON representation</span></span>

<span data-ttu-id="a2a2e-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2a2e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->