---
title: meetingTimeSuggestion リソースの種類
description: '会議の時間、出席の可能性、個人などの情報を含む会議の提案 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d0f6c36d0fb76c1bc115b9cd0490a79a3f94a77b
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936235"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="b7b6d-103">meetingTimeSuggestion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7b6d-103">meetingTimeSuggestion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b6d-104">会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。</span><span class="sxs-lookup"><span data-stu-id="b7b6d-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7b6d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7b6d-105">JSON representation</span></span>

<span data-ttu-id="b7b6d-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b7b6d-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="b7b6d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7b6d-107">Properties</span></span>
| <span data-ttu-id="b7b6d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7b6d-108">Property</span></span>     | <span data-ttu-id="b7b6d-109">型</span><span class="sxs-lookup"><span data-stu-id="b7b6d-109">Type</span></span>   |<span data-ttu-id="b7b6d-110">説明</span><span class="sxs-lookup"><span data-stu-id="b7b6d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7b6d-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="b7b6d-111">attendeeAvailability</span></span>|<span data-ttu-id="b7b6d-112">[attendeeAvailability](attendeeavailability.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b7b6d-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="b7b6d-113">この提案された会議の各出席者の空き時間情報の状態を示す配列。</span><span class="sxs-lookup"><span data-stu-id="b7b6d-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="b7b6d-114">confidence</span><span class="sxs-lookup"><span data-stu-id="b7b6d-114">confidence</span></span>|<span data-ttu-id="b7b6d-115">Double</span><span class="sxs-lookup"><span data-stu-id="b7b6d-115">Double</span></span>|<span data-ttu-id="b7b6d-116">すべての出席者が出席する見込みを表すパーセンテージ。</span><span class="sxs-lookup"><span data-stu-id="b7b6d-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="b7b6d-117">locations</span><span class="sxs-lookup"><span data-stu-id="b7b6d-117">locations</span></span>|<span data-ttu-id="b7b6d-118">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b7b6d-118">[location](location.md) collection</span></span>|<span data-ttu-id="b7b6d-119">この提案された会議の各会議場所の名前と地理的な場所を指定する配列。</span><span class="sxs-lookup"><span data-stu-id="b7b6d-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="b7b6d-120">会議タイムスロット</span><span class="sxs-lookup"><span data-stu-id="b7b6d-120">meetingTimeSlot</span></span>|[<span data-ttu-id="b7b6d-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="b7b6d-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="b7b6d-122">会議の提案されている期間。</span><span class="sxs-lookup"><span data-stu-id="b7b6d-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="b7b6d-123">降順</span><span class="sxs-lookup"><span data-stu-id="b7b6d-123">order</span></span>|<span data-ttu-id="b7b6d-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b7b6d-124">Int32</span></span>|<span data-ttu-id="b7b6d-125">同じ信頼度がある場合に、chronology によって並べ替えられた、会議の時間の候補の順序 (高から低まで)。</span><span class="sxs-lookup"><span data-stu-id="b7b6d-125">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="b7b6d-126">組織の空き時間情報</span><span class="sxs-lookup"><span data-stu-id="b7b6d-126">organizerAvailability</span></span>|<span data-ttu-id="b7b6d-127">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="b7b6d-127">availabilityStatus</span></span>| <span data-ttu-id="b7b6d-p101">この提案されている会議の開催者の空き時間情報。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="b7b6d-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="b7b6d-130">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="b7b6d-130">suggestionReason</span></span>|<span data-ttu-id="b7b6d-131">String</span><span class="sxs-lookup"><span data-stu-id="b7b6d-131">String</span></span>|<span data-ttu-id="b7b6d-132">会議時間を提案する理由。</span><span class="sxs-lookup"><span data-stu-id="b7b6d-132">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
