---
title: educationAssignmentGrade リソースの種類
description: " ただし、このサブクラスは、すべてのタイプ (点、合格/不合格、) のグレーディングの"
localization_priority: Normal
ms.openlocfilehash: 371346c6ff23623a118b9ee169e563e75e2429f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889013"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="d3237-103">educationAssignmentGrade リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3237-103">educationAssignmentGrade resource type</span></span>

> <span data-ttu-id="d3237-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d3237-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3237-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3237-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3237-106">提出書類の**成績**のオブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="d3237-106">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="d3237-107">これは、抽象型はインスタンス化します。ただし、グレーディング、(ポイント、合格/不合格、) のすべての種類は、このリソースの種類のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="d3237-107">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="d3237-108">このオブジェクトは、グレーディングを行っているにも追跡します。</span><span class="sxs-lookup"><span data-stu-id="d3237-108">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="d3237-109">**Submission.grade**プロパティで使用されます。</span><span class="sxs-lookup"><span data-stu-id="d3237-109">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="d3237-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3237-110">Properties</span></span>
| <span data-ttu-id="d3237-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3237-111">Property</span></span>     | <span data-ttu-id="d3237-112">種類</span><span class="sxs-lookup"><span data-stu-id="d3237-112">Type</span></span>   |<span data-ttu-id="d3237-113">説明</span><span class="sxs-lookup"><span data-stu-id="d3237-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3237-114">gradedBy</span><span class="sxs-lookup"><span data-stu-id="d3237-114">gradedBy</span></span>|[<span data-ttu-id="d3237-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="d3237-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="d3237-116">グレーディングをしたユーザーです。</span><span class="sxs-lookup"><span data-stu-id="d3237-116">User who did the grading.</span></span> |
|<span data-ttu-id="d3237-117">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3237-117">gradedDateTime</span></span>|<span data-ttu-id="d3237-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3237-118">DateTimeOffset</span></span>| <span data-ttu-id="d3237-119">グレードがこの送信オブジェクトに適用されたときの時点です。</span><span class="sxs-lookup"><span data-stu-id="d3237-119">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="d3237-120">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d3237-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d3237-121">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d3237-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3237-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3237-122">JSON representation</span></span>

<span data-ttu-id="d3237-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3237-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
