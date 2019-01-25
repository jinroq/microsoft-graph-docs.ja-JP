---
title: educationFeedback リソースの種類
description: 学生に教師からのフィードバックです。 このプロパティは、両方のテキスト部分に、人とのフィードバックを表します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 90e55b20b371d04bc3c6d45bb84fe6bf42157a2f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515637"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="737f2-104">educationFeedback リソースの種類</span><span class="sxs-lookup"><span data-stu-id="737f2-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="737f2-105">学生に教師からのフィードバックです。</span><span class="sxs-lookup"><span data-stu-id="737f2-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="737f2-106">このプロパティは、両方のテキスト部分に、人とのフィードバックを表します。</span><span class="sxs-lookup"><span data-stu-id="737f2-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="737f2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="737f2-107">Properties</span></span>
| <span data-ttu-id="737f2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="737f2-108">Property</span></span>     | <span data-ttu-id="737f2-109">型</span><span class="sxs-lookup"><span data-stu-id="737f2-109">Type</span></span>   |<span data-ttu-id="737f2-110">説明</span><span class="sxs-lookup"><span data-stu-id="737f2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="737f2-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="737f2-111">feedbackBy</span></span>|[<span data-ttu-id="737f2-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="737f2-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="737f2-113">フィードバックを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="737f2-113">User who created the feedback.</span></span>|
|<span data-ttu-id="737f2-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="737f2-114">feedbackDateTime</span></span>|<span data-ttu-id="737f2-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="737f2-115">DateTimeOffset</span></span>|<span data-ttu-id="737f2-116">フィードバックが与えられた瞬間です。</span><span class="sxs-lookup"><span data-stu-id="737f2-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="737f2-117">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="737f2-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="737f2-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="737f2-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="737f2-119">text</span><span class="sxs-lookup"><span data-stu-id="737f2-119">text</span></span>|[<span data-ttu-id="737f2-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="737f2-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="737f2-121">フィードバック。</span><span class="sxs-lookup"><span data-stu-id="737f2-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="737f2-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="737f2-122">JSON representation</span></span>

<span data-ttu-id="737f2-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="737f2-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfeedback.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
