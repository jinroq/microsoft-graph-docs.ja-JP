---
title: educationFeedback リソースの種類
description: 教師から学生へのフィードバック。 このプロパティは、フィードバックのテキスト部分と who の両方を表します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7ef923870d94479d7ea1d9d762ee729b5060afd6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340525"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="07087-104">educationFeedback リソースの種類</span><span class="sxs-lookup"><span data-stu-id="07087-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07087-105">教師から学生へのフィードバック。</span><span class="sxs-lookup"><span data-stu-id="07087-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="07087-106">このプロパティは、フィードバックのテキスト部分と who の両方を表します。</span><span class="sxs-lookup"><span data-stu-id="07087-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="07087-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07087-107">Properties</span></span>
| <span data-ttu-id="07087-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07087-108">Property</span></span>     | <span data-ttu-id="07087-109">型</span><span class="sxs-lookup"><span data-stu-id="07087-109">Type</span></span>   |<span data-ttu-id="07087-110">説明</span><span class="sxs-lookup"><span data-stu-id="07087-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07087-111">フィードバック</span><span class="sxs-lookup"><span data-stu-id="07087-111">feedbackBy</span></span>|[<span data-ttu-id="07087-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="07087-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="07087-113">フィードバックを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="07087-113">User who created the feedback.</span></span>|
|<span data-ttu-id="07087-114">フィードバック datetime</span><span class="sxs-lookup"><span data-stu-id="07087-114">feedbackDateTime</span></span>|<span data-ttu-id="07087-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07087-115">DateTimeOffset</span></span>|<span data-ttu-id="07087-116">フィードバックが提供された時点の時間。</span><span class="sxs-lookup"><span data-stu-id="07087-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="07087-117">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="07087-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07087-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="07087-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="07087-119">text</span><span class="sxs-lookup"><span data-stu-id="07087-119">text</span></span>|[<span data-ttu-id="07087-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="07087-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="07087-121">フィードバック.</span><span class="sxs-lookup"><span data-stu-id="07087-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07087-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07087-122">JSON representation</span></span>

<span data-ttu-id="07087-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="07087-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String (timestamp)",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
