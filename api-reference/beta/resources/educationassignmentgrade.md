---
title: educationAssignmentGrade リソースの種類
description: " ただし、すべての種類の種類 (ポイント、合格/失敗など) は、この"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5ca13ba057ef000a468d910d49288d9ae8e0c962
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543022"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="3856e-103">educationAssignmentGrade リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3856e-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3856e-104">提出物の**学年**オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="3856e-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="3856e-105">これは、インスタンス化されない抽象型です。ただし、すべての種類の種類 (ポイント、合格/失敗など) は、このリソースの種類のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="3856e-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="3856e-106">また、このオブジェクトは、対象とするユーザーを追跡します。</span><span class="sxs-lookup"><span data-stu-id="3856e-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="3856e-107">これは、"**成績**" プロパティで使用されます。</span><span class="sxs-lookup"><span data-stu-id="3856e-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="3856e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3856e-108">Properties</span></span>
| <span data-ttu-id="3856e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3856e-109">Property</span></span>     | <span data-ttu-id="3856e-110">型</span><span class="sxs-lookup"><span data-stu-id="3856e-110">Type</span></span>   |<span data-ttu-id="3856e-111">説明</span><span class="sxs-lookup"><span data-stu-id="3856e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3856e-112">gradedBy</span><span class="sxs-lookup"><span data-stu-id="3856e-112">gradedBy</span></span>|[<span data-ttu-id="3856e-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="3856e-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="3856e-114">対象をしたユーザー。</span><span class="sxs-lookup"><span data-stu-id="3856e-114">User who did the grading.</span></span> |
|<span data-ttu-id="3856e-115">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="3856e-115">gradedDateTime</span></span>|<span data-ttu-id="3856e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3856e-116">DateTimeOffset</span></span>| <span data-ttu-id="3856e-117">成績がこの提出物オブジェクトに適用された時点での時間。</span><span class="sxs-lookup"><span data-stu-id="3856e-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="3856e-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="3856e-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3856e-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3856e-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3856e-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3856e-120">JSON representation</span></span>

<span data-ttu-id="3856e-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3856e-121">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
