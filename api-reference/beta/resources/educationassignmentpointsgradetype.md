---
title: educationAssignmentPointsGradeType リソースの種類
description: '**Assignments.grading**プロパティと共に使用します。 これは、educationAssignmentGradeType のサブクラスです。'
ms.openlocfilehash: 5c170540e99003a78df0550d4d6542c07df8f1ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073487"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="25652-104">educationAssignmentPointsGradeType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25652-104">educationAssignmentPointsGradeType resource type</span></span>

> <span data-ttu-id="25652-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="25652-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25652-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25652-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25652-107">**Assignments.grading**プロパティと共に使用します。</span><span class="sxs-lookup"><span data-stu-id="25652-107">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="25652-108">これは、 [educationAssignmentGradeType](educationassignmentgradetype.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="25652-108">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="25652-109">これは、割り当てが焼き付けるし、この作業項目に各受講者が達成できるポイントの最大数を格納することを示します。</span><span class="sxs-lookup"><span data-stu-id="25652-109">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="25652-110">割り当てに設定すると、送信するたびに、各受講者用のポイントを格納するために関連付けられている[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)プロパティが表示されます。</span><span class="sxs-lookup"><span data-stu-id="25652-110">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="25652-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25652-111">Properties</span></span>
| <span data-ttu-id="25652-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25652-112">Property</span></span>     | <span data-ttu-id="25652-113">型</span><span class="sxs-lookup"><span data-stu-id="25652-113">Type</span></span>   |<span data-ttu-id="25652-114">説明</span><span class="sxs-lookup"><span data-stu-id="25652-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25652-115">maxPoints</span><span class="sxs-lookup"><span data-stu-id="25652-115">maxPoints</span></span>|<span data-ttu-id="25652-116">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="25652-116">Single</span></span>| <span data-ttu-id="25652-117">最大は、この割り当ての可能性を指しています。</span><span class="sxs-lookup"><span data-stu-id="25652-117">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="25652-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25652-118">JSON representation</span></span>

<span data-ttu-id="25652-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="25652-119">The following is a JSON representation of the resource.</span></span>

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