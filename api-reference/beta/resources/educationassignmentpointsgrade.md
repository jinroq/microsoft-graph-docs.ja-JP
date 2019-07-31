---
title: educationAssignmentPointsGrade リソースの種類
description: 1つの割り当てがポイントグレードの種類に設定されている場合、各提出物には、"**成績**" プロパティに関連付けられたオブジェクトがあります。 これにより、educationAssignmentGrade からサブクラスが作成されます。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6e74c6bb74c830cb1ceb80e149903282c4da33ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972818"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="f0935-104">educationAssignmentPointsGrade リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0935-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0935-105">1つの割り当てがポイントグレードの種類に設定されている場合、各提出物には、"**成績**" プロパティに関連付けられたオブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="f0935-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="f0935-106">これにより、 [educationAssignmentGrade](educationassignmentgrade.md)からサブクラスが作成され、このプロパティに who データが追加されます。</span><span class="sxs-lookup"><span data-stu-id="f0935-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="f0935-107">Max 要素は、 **assignments**プロパティに格納されます。</span><span class="sxs-lookup"><span data-stu-id="f0935-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="f0935-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0935-108">Properties</span></span>
| <span data-ttu-id="f0935-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0935-109">Property</span></span>     | <span data-ttu-id="f0935-110">型</span><span class="sxs-lookup"><span data-stu-id="f0935-110">Type</span></span>   |<span data-ttu-id="f0935-111">説明</span><span class="sxs-lookup"><span data-stu-id="f0935-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0935-112">points</span><span class="sxs-lookup"><span data-stu-id="f0935-112">points</span></span>|<span data-ttu-id="f0935-113">1 行</span><span class="sxs-lookup"><span data-stu-id="f0935-113">Single</span></span>|<span data-ttu-id="f0935-114">教師がこの送信オブジェクトを提供しているポイントの数。</span><span class="sxs-lookup"><span data-stu-id="f0935-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0935-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0935-115">JSON representation</span></span>

<span data-ttu-id="f0935-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0935-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
