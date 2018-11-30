---
title: educationAssignmentPointsGrade リソースの種類
description: ポイント グレード タイプに割り当てを設定すると、各提出書類は、このオブジェクトの**submission.grade**プロパティに関連付けられているがあります。 これから educationAssignmentGrade、サブクラスを作成します。
ms.openlocfilehash: 2439ac8946fea588bd7bc1afe7f1ff1042b9179a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068503"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="a2e62-104">educationAssignmentPointsGrade リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2e62-104">educationAssignmentPointsGrade resource type</span></span>

> <span data-ttu-id="a2e62-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2e62-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2e62-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2e62-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2e62-107">ポイント グレード タイプに割り当てを設定すると、各提出書類は、このオブジェクトの**submission.grade**プロパティに関連付けられているがあります。</span><span class="sxs-lookup"><span data-stu-id="a2e62-107">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="a2e62-108">これは、 [educationAssignmentGrade](educationassignmentgrade.md)データが追加されます、ユーザーにこのプロパティをからサブクラスを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2e62-108">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="a2e62-109">最大のポイントは、 **assignments.grading**プロパティに格納されます。</span><span class="sxs-lookup"><span data-stu-id="a2e62-109">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="a2e62-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2e62-110">Properties</span></span>
| <span data-ttu-id="a2e62-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2e62-111">Property</span></span>     | <span data-ttu-id="a2e62-112">型</span><span class="sxs-lookup"><span data-stu-id="a2e62-112">Type</span></span>   |<span data-ttu-id="a2e62-113">説明</span><span class="sxs-lookup"><span data-stu-id="a2e62-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2e62-114">points</span><span class="sxs-lookup"><span data-stu-id="a2e62-114">points</span></span>|<span data-ttu-id="a2e62-115">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="a2e62-115">Single</span></span>|<span data-ttu-id="a2e62-116">先生をポイント数では、この送信オブジェクト、といいます。</span><span class="sxs-lookup"><span data-stu-id="a2e62-116">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2e62-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2e62-117">JSON representation</span></span>

<span data-ttu-id="a2e62-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2e62-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->