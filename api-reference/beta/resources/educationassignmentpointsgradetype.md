---
title: educationAssignmentPointsGradeType リソースの種類
description: '**Assignments.grading**プロパティと共に使用します。 これは、educationAssignmentGradeType のサブクラスです。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 567bff38f8a20456dffffdd91775a1e32852fe20
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508896"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="52b3e-104">educationAssignmentPointsGradeType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52b3e-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52b3e-105">**Assignments.grading**プロパティと共に使用します。</span><span class="sxs-lookup"><span data-stu-id="52b3e-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="52b3e-106">これは、 [educationAssignmentGradeType](educationassignmentgradetype.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="52b3e-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="52b3e-107">これは、割り当てが焼き付けるし、この作業項目に各受講者が達成できるポイントの最大数を格納することを示します。</span><span class="sxs-lookup"><span data-stu-id="52b3e-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="52b3e-108">割り当てに設定すると、送信するたびに、各受講者用のポイントを格納するために関連付けられている[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)プロパティが表示されます。</span><span class="sxs-lookup"><span data-stu-id="52b3e-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="52b3e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52b3e-109">Properties</span></span>
| <span data-ttu-id="52b3e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52b3e-110">Property</span></span>     | <span data-ttu-id="52b3e-111">型</span><span class="sxs-lookup"><span data-stu-id="52b3e-111">Type</span></span>   |<span data-ttu-id="52b3e-112">説明</span><span class="sxs-lookup"><span data-stu-id="52b3e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52b3e-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="52b3e-113">maxPoints</span></span>|<span data-ttu-id="52b3e-114">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="52b3e-114">Single</span></span>| <span data-ttu-id="52b3e-115">最大は、この割り当ての可能性を指しています。</span><span class="sxs-lookup"><span data-stu-id="52b3e-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="52b3e-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52b3e-116">JSON representation</span></span>

<span data-ttu-id="52b3e-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52b3e-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgradetype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
