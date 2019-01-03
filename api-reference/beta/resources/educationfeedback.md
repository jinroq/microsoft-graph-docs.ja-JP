---
title: educationFeedback リソースの種類
description: 学生に教師からのフィードバックです。 このプロパティは、両方のテキスト部分に、人とのフィードバックを表します。
author: mmast-msft
ms.openlocfilehash: 934d1ec104133257bb1b767e8922c2379e3fd11a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363593"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="daf57-104">educationFeedback リソースの種類</span><span class="sxs-lookup"><span data-stu-id="daf57-104">educationFeedback resource type</span></span>

> <span data-ttu-id="daf57-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="daf57-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="daf57-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="daf57-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="daf57-107">学生に教師からのフィードバックです。</span><span class="sxs-lookup"><span data-stu-id="daf57-107">Feedback from a teacher to a student.</span></span> <span data-ttu-id="daf57-108">このプロパティは、両方のテキスト部分に、人とのフィードバックを表します。</span><span class="sxs-lookup"><span data-stu-id="daf57-108">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="daf57-109">Properties</span><span class="sxs-lookup"><span data-stu-id="daf57-109">Properties</span></span>
| <span data-ttu-id="daf57-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="daf57-110">Property</span></span>     | <span data-ttu-id="daf57-111">種類</span><span class="sxs-lookup"><span data-stu-id="daf57-111">Type</span></span>   |<span data-ttu-id="daf57-112">説明</span><span class="sxs-lookup"><span data-stu-id="daf57-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daf57-113">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="daf57-113">feedbackBy</span></span>|[<span data-ttu-id="daf57-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="daf57-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="daf57-115">フィードバックを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="daf57-115">User who created the feedback.</span></span>|
|<span data-ttu-id="daf57-116">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="daf57-116">feedbackDateTime</span></span>|<span data-ttu-id="daf57-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daf57-117">DateTimeOffset</span></span>|<span data-ttu-id="daf57-118">フィードバックが与えられた瞬間です。</span><span class="sxs-lookup"><span data-stu-id="daf57-118">Moment in time when the feedback was given.</span></span> <span data-ttu-id="daf57-119">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="daf57-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="daf57-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="daf57-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="daf57-121">text</span><span class="sxs-lookup"><span data-stu-id="daf57-121">text</span></span>|[<span data-ttu-id="daf57-122">itemBody</span><span class="sxs-lookup"><span data-stu-id="daf57-122">itemBody</span></span>](itembody.md)|<span data-ttu-id="daf57-123">フィードバックします。</span><span class="sxs-lookup"><span data-stu-id="daf57-123">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="daf57-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="daf57-124">JSON representation</span></span>

<span data-ttu-id="daf57-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="daf57-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->