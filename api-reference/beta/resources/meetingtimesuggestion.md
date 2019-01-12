---
title: meetingTimeSuggestion リソースの種類
description: '提案された会議の時間、出勤の可能性、個人情報が含まれる会議 '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 6c7adf6d3b31ebdd5a068f71572b80141736a0bf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956116"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="392be-103">meetingTimeSuggestion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="392be-103">meetingTimeSuggestion resource type</span></span>

> <span data-ttu-id="392be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="392be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="392be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="392be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="392be-106">会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。</span><span class="sxs-lookup"><span data-stu-id="392be-106">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="392be-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="392be-107">JSON representation</span></span>

<span data-ttu-id="392be-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="392be-108">Here is a JSON representation of the resource</span></span>

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
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="392be-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="392be-109">Properties</span></span>
| <span data-ttu-id="392be-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="392be-110">Property</span></span>     | <span data-ttu-id="392be-111">種類</span><span class="sxs-lookup"><span data-stu-id="392be-111">Type</span></span>   |<span data-ttu-id="392be-112">説明</span><span class="sxs-lookup"><span data-stu-id="392be-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="392be-113">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="392be-113">attendeeAvailability</span></span>|<span data-ttu-id="392be-114">[attendeeAvailability](attendeeavailability.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="392be-114">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="392be-115">この提案された会議の各出席者の空き時間情報の状態を示す配列。</span><span class="sxs-lookup"><span data-stu-id="392be-115">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="392be-116">confidence</span><span class="sxs-lookup"><span data-stu-id="392be-116">confidence</span></span>|<span data-ttu-id="392be-117">Double</span><span class="sxs-lookup"><span data-stu-id="392be-117">Double</span></span>|<span data-ttu-id="392be-118">すべての出席者が出席する見込みを表すパーセンテージ。</span><span class="sxs-lookup"><span data-stu-id="392be-118">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="392be-119">locations</span><span class="sxs-lookup"><span data-stu-id="392be-119">locations</span></span>|<span data-ttu-id="392be-120">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="392be-120">[location](location.md) collection</span></span>|<span data-ttu-id="392be-121">この提案された会議の各会議場所の名前と地理的な場所を指定する配列。</span><span class="sxs-lookup"><span data-stu-id="392be-121">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="392be-122">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="392be-122">meetingTimeSlot</span></span>|[<span data-ttu-id="392be-123">timeSlot</span><span class="sxs-lookup"><span data-stu-id="392be-123">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="392be-124">会議の提案されている期間。</span><span class="sxs-lookup"><span data-stu-id="392be-124">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="392be-125">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="392be-125">organizerAvailability</span></span>|<span data-ttu-id="392be-126">String</span><span class="sxs-lookup"><span data-stu-id="392be-126">String</span></span>| <span data-ttu-id="392be-p102">この提案されている会議の開催者の空き時間情報。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="392be-p102">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="392be-129">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="392be-129">suggestionReason</span></span>|<span data-ttu-id="392be-130">String</span><span class="sxs-lookup"><span data-stu-id="392be-130">String</span></span>|<span data-ttu-id="392be-131">会議時間を提案する理由。</span><span class="sxs-lookup"><span data-stu-id="392be-131">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
