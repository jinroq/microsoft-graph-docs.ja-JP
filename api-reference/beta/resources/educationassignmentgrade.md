---
title: educationAssignmentGrade リソースの種類
description: " ただし、すべての種類の種類 (ポイント、合格/失敗など) は、この"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: e925059a5eb06e5cc9795f78368b884fa40dd3ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334543"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="4158a-103">educationAssignmentGrade リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4158a-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4158a-104">提出物の**学年**オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="4158a-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="4158a-105">これは、インスタンス化されない抽象型です。ただし、すべての種類の種類 (ポイント、合格/失敗など) は、このリソースの種類のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="4158a-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="4158a-106">また、このオブジェクトは、対象とするユーザーを追跡します。</span><span class="sxs-lookup"><span data-stu-id="4158a-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="4158a-107">これは、"**成績**" プロパティで使用されます。</span><span class="sxs-lookup"><span data-stu-id="4158a-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="4158a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4158a-108">Properties</span></span>
| <span data-ttu-id="4158a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4158a-109">Property</span></span>     | <span data-ttu-id="4158a-110">型</span><span class="sxs-lookup"><span data-stu-id="4158a-110">Type</span></span>   |<span data-ttu-id="4158a-111">説明</span><span class="sxs-lookup"><span data-stu-id="4158a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4158a-112">gradedBy</span><span class="sxs-lookup"><span data-stu-id="4158a-112">gradedBy</span></span>|[<span data-ttu-id="4158a-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="4158a-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="4158a-114">対象をしたユーザー。</span><span class="sxs-lookup"><span data-stu-id="4158a-114">User who did the grading.</span></span> |
|<span data-ttu-id="4158a-115">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="4158a-115">gradedDateTime</span></span>|<span data-ttu-id="4158a-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4158a-116">DateTimeOffset</span></span>| <span data-ttu-id="4158a-117">成績がこの提出物オブジェクトに適用された時点での時間。</span><span class="sxs-lookup"><span data-stu-id="4158a-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="4158a-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4158a-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4158a-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4158a-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4158a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4158a-120">JSON representation</span></span>

<span data-ttu-id="4158a-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4158a-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
