---
title: meetingTimeSuggestion リソースの種類
description: '会議の時間、出席の可能性、個人などの情報を含む会議の提案 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4c5a4cb4d094e7fd7fe9b0e56227a556c6e5b5d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573978"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="e1ff8-103">meetingTimeSuggestion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1ff8-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="e1ff8-104">会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1ff8-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1ff8-105">JSON representation</span></span>

<span data-ttu-id="e1ff8-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e1ff8-106">Here is a JSON representation of the resource</span></span>

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
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="e1ff8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1ff8-107">Properties</span></span>
| <span data-ttu-id="e1ff8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1ff8-108">Property</span></span>     | <span data-ttu-id="e1ff8-109">型</span><span class="sxs-lookup"><span data-stu-id="e1ff8-109">Type</span></span>   |<span data-ttu-id="e1ff8-110">説明</span><span class="sxs-lookup"><span data-stu-id="e1ff8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1ff8-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="e1ff8-111">attendeeAvailability</span></span>|<span data-ttu-id="e1ff8-112">[attendeeAvailability](attendeeavailability.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1ff8-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="e1ff8-113">この提案された会議の各出席者の空き時間情報の状態を示す配列。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="e1ff8-114">confidence</span><span class="sxs-lookup"><span data-stu-id="e1ff8-114">confidence</span></span>|<span data-ttu-id="e1ff8-115">Double</span><span class="sxs-lookup"><span data-stu-id="e1ff8-115">Double</span></span>|<span data-ttu-id="e1ff8-116">すべての出席者が出席する見込みを表すパーセンテージ。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="e1ff8-117">locations</span><span class="sxs-lookup"><span data-stu-id="e1ff8-117">locations</span></span>|<span data-ttu-id="e1ff8-118">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1ff8-118">[location](location.md) collection</span></span>|<span data-ttu-id="e1ff8-119">この提案された会議の各会議場所の名前と地理的な場所を指定する配列。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="e1ff8-120">会議タイムスロット</span><span class="sxs-lookup"><span data-stu-id="e1ff8-120">meetingTimeSlot</span></span>|[<span data-ttu-id="e1ff8-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="e1ff8-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="e1ff8-122">会議の提案されている期間。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="e1ff8-123">降順</span><span class="sxs-lookup"><span data-stu-id="e1ff8-123">order</span></span>|<span data-ttu-id="e1ff8-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ff8-124">Int32</span></span>|<span data-ttu-id="e1ff8-125">同じ信頼度がある場合に、chronology によって並べ替えられた、会議の時間の候補の順序 (高から低まで)。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-125">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="e1ff8-126">組織の空き時間情報</span><span class="sxs-lookup"><span data-stu-id="e1ff8-126">organizerAvailability</span></span>|<span data-ttu-id="e1ff8-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="e1ff8-127">freeBusyStatus</span></span>| <span data-ttu-id="e1ff8-128">この提案されている会議の開催者の空き時間情報。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-128">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="e1ff8-129">使用可能な値は`free`、 `tentative`、 `busy` `oof` `workingElsewhere`、、、 `unknown`、です。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="e1ff8-130">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="e1ff8-130">suggestionReason</span></span>|<span data-ttu-id="e1ff8-131">String</span><span class="sxs-lookup"><span data-stu-id="e1ff8-131">String</span></span>|<span data-ttu-id="e1ff8-132">会議時間を提案する理由。</span><span class="sxs-lookup"><span data-stu-id="e1ff8-132">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
