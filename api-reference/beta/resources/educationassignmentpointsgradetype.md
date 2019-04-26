---
title: educationAssignmentPointsGradeType リソースの種類
description: '**assignments**プロパティと組み合わせて使用します。 これは、educationAssignmentGradeType のサブクラスです。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 61e6e425730685d4447875cdb074526e7ebc0a17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334437"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="388a3-104">educationAssignmentPointsGradeType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="388a3-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="388a3-105">**assignments**プロパティと組み合わせて使用します。</span><span class="sxs-lookup"><span data-stu-id="388a3-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="388a3-106">これは、 [educationAssignmentGradeType](educationassignmentgradetype.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="388a3-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="388a3-107">これは、割り当てが採点され、各学生がこの作業項目に対して達成できる最大ポイント数を格納することを示します。</span><span class="sxs-lookup"><span data-stu-id="388a3-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="388a3-108">割り当てに対してこのプロパティを設定すると、各学生のポイントの保存用に、各送信に関連付けられている[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)プロパティが取得されます。</span><span class="sxs-lookup"><span data-stu-id="388a3-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="388a3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="388a3-109">Properties</span></span>
| <span data-ttu-id="388a3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="388a3-110">Property</span></span>     | <span data-ttu-id="388a3-111">型</span><span class="sxs-lookup"><span data-stu-id="388a3-111">Type</span></span>   |<span data-ttu-id="388a3-112">説明</span><span class="sxs-lookup"><span data-stu-id="388a3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="388a3-113">maxpoints</span><span class="sxs-lookup"><span data-stu-id="388a3-113">maxPoints</span></span>|<span data-ttu-id="388a3-114">1 行</span><span class="sxs-lookup"><span data-stu-id="388a3-114">Single</span></span>| <span data-ttu-id="388a3-115">この割り当てで可能な最大ポイント。</span><span class="sxs-lookup"><span data-stu-id="388a3-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="388a3-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="388a3-116">JSON representation</span></span>

<span data-ttu-id="388a3-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="388a3-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
