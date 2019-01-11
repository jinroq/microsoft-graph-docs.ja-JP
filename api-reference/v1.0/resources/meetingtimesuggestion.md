---
title: meetingTimeSuggestion リソースの種類
description: '提案された会議の時間、出勤の可能性、個人情報が含まれる会議 '
localization_priority: Normal
ms.openlocfilehash: d1cca365c66c114063fbf859e241a5d9a81303e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845998"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="99f8b-103">meetingTimeSuggestion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99f8b-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="99f8b-104">会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。</span><span class="sxs-lookup"><span data-stu-id="99f8b-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99f8b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99f8b-105">JSON representation</span></span>

<span data-ttu-id="99f8b-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="99f8b-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="99f8b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99f8b-107">Properties</span></span>
| <span data-ttu-id="99f8b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99f8b-108">Property</span></span>     | <span data-ttu-id="99f8b-109">種類</span><span class="sxs-lookup"><span data-stu-id="99f8b-109">Type</span></span>   |<span data-ttu-id="99f8b-110">説明</span><span class="sxs-lookup"><span data-stu-id="99f8b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99f8b-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="99f8b-111">attendeeAvailability</span></span>|<span data-ttu-id="99f8b-112">[attendeeAvailability](attendeeavailability.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="99f8b-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="99f8b-113">この提案された会議の各出席者の空き時間情報の状態を示す配列。</span><span class="sxs-lookup"><span data-stu-id="99f8b-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="99f8b-114">confidence</span><span class="sxs-lookup"><span data-stu-id="99f8b-114">confidence</span></span>|<span data-ttu-id="99f8b-115">Double</span><span class="sxs-lookup"><span data-stu-id="99f8b-115">Double</span></span>|<span data-ttu-id="99f8b-116">すべての出席者が出席する見込みを表すパーセンテージ。</span><span class="sxs-lookup"><span data-stu-id="99f8b-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="99f8b-117">locations</span><span class="sxs-lookup"><span data-stu-id="99f8b-117">locations</span></span>|<span data-ttu-id="99f8b-118">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="99f8b-118">[location](location.md) collection</span></span>|<span data-ttu-id="99f8b-119">この提案された会議の各会議場所の名前と地理的な場所を指定する配列。</span><span class="sxs-lookup"><span data-stu-id="99f8b-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="99f8b-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="99f8b-120">meetingTimeSlot</span></span>|[<span data-ttu-id="99f8b-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="99f8b-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="99f8b-122">会議の提案されている期間。</span><span class="sxs-lookup"><span data-stu-id="99f8b-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="99f8b-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="99f8b-123">organizerAvailability</span></span>|<span data-ttu-id="99f8b-124">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="99f8b-124">freeBusyStatus</span></span>| <span data-ttu-id="99f8b-125">この提案された会議の開催者の可用性。</span><span class="sxs-lookup"><span data-stu-id="99f8b-125">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="99f8b-126">可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="99f8b-126">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="99f8b-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="99f8b-127">suggestionReason</span></span>|<span data-ttu-id="99f8b-128">String</span><span class="sxs-lookup"><span data-stu-id="99f8b-128">String</span></span>|<span data-ttu-id="99f8b-129">会議時間を提案する理由。</span><span class="sxs-lookup"><span data-stu-id="99f8b-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
