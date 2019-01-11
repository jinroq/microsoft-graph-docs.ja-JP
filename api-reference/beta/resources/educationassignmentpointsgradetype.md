---
title: educationAssignmentPointsGradeType リソースの種類
description: '**Assignments.grading**プロパティと共に使用します。 これは、educationAssignmentGradeType のサブクラスです。'
localization_priority: Normal
ms.openlocfilehash: f00014eab1dbf7bc8eb78a8898c6abba9977e8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860971"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="d7755-104">educationAssignmentPointsGradeType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7755-104">educationAssignmentPointsGradeType resource type</span></span>

> <span data-ttu-id="d7755-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d7755-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7755-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7755-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7755-107">**Assignments.grading**プロパティと共に使用します。</span><span class="sxs-lookup"><span data-stu-id="d7755-107">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="d7755-108">これは、 [educationAssignmentGradeType](educationassignmentgradetype.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="d7755-108">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="d7755-109">これは、割り当てが焼き付けるし、この作業項目に各受講者が達成できるポイントの最大数を格納することを示します。</span><span class="sxs-lookup"><span data-stu-id="d7755-109">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="d7755-110">割り当てに設定すると、送信するたびに、各受講者用のポイントを格納するために関連付けられている[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)プロパティが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d7755-110">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="d7755-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7755-111">Properties</span></span>
| <span data-ttu-id="d7755-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7755-112">Property</span></span>     | <span data-ttu-id="d7755-113">種類</span><span class="sxs-lookup"><span data-stu-id="d7755-113">Type</span></span>   |<span data-ttu-id="d7755-114">説明</span><span class="sxs-lookup"><span data-stu-id="d7755-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7755-115">maxPoints</span><span class="sxs-lookup"><span data-stu-id="d7755-115">maxPoints</span></span>|<span data-ttu-id="d7755-116">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="d7755-116">Single</span></span>| <span data-ttu-id="d7755-117">最大は、この割り当ての可能性を指しています。</span><span class="sxs-lookup"><span data-stu-id="d7755-117">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d7755-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7755-118">JSON representation</span></span>

<span data-ttu-id="d7755-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7755-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
