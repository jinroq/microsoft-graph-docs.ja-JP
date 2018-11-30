---
title: meetingTimeCandidate リソースの種類
description: '提案された会議の時間、出勤の可能性、個人情報が含まれる会議 '
ms.openlocfilehash: 56aae66cf4c532108d2db2f8f4cfc71487f09150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068186"
---
# <a name="meetingtimecandidate-resource-type"></a><span data-ttu-id="dfd33-103">meetingTimeCandidate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfd33-103">meetingTimeCandidate resource type</span></span>

> <span data-ttu-id="dfd33-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dfd33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfd33-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfd33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfd33-106">会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。</span><span class="sxs-lookup"><span data-stu-id="dfd33-106">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfd33-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfd33-107">JSON representation</span></span>

<span data-ttu-id="dfd33-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="dfd33-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidate"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionHint": "String"
}

```
## <a name="properties"></a><span data-ttu-id="dfd33-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfd33-109">Properties</span></span>
| <span data-ttu-id="dfd33-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfd33-110">Property</span></span>     | <span data-ttu-id="dfd33-111">型</span><span class="sxs-lookup"><span data-stu-id="dfd33-111">Type</span></span>   |<span data-ttu-id="dfd33-112">説明</span><span class="sxs-lookup"><span data-stu-id="dfd33-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfd33-113">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="dfd33-113">attendeeAvailability</span></span>|<span data-ttu-id="dfd33-114">[attendeeAvailability](attendeeavailability.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dfd33-114">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="dfd33-115">この提案された会議の各出席者の空き時間情報の状態を示す配列。</span><span class="sxs-lookup"><span data-stu-id="dfd33-115">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="dfd33-116">confidence</span><span class="sxs-lookup"><span data-stu-id="dfd33-116">confidence</span></span>|<span data-ttu-id="dfd33-117">Double</span><span class="sxs-lookup"><span data-stu-id="dfd33-117">Double</span></span>|<span data-ttu-id="dfd33-118">すべての出席者が出席する見込みを表すパーセンテージ。</span><span class="sxs-lookup"><span data-stu-id="dfd33-118">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="dfd33-119">locations</span><span class="sxs-lookup"><span data-stu-id="dfd33-119">locations</span></span>|<span data-ttu-id="dfd33-120">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dfd33-120">[location](location.md) collection</span></span>|<span data-ttu-id="dfd33-121">この提案された会議の各会議場所の名前と地理的な場所を指定する配列。</span><span class="sxs-lookup"><span data-stu-id="dfd33-121">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="dfd33-122">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="dfd33-122">meetingTimeSlot</span></span>|[<span data-ttu-id="dfd33-123">timeSlot</span><span class="sxs-lookup"><span data-stu-id="dfd33-123">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="dfd33-124">会議の提案されている期間。</span><span class="sxs-lookup"><span data-stu-id="dfd33-124">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="dfd33-125">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="dfd33-125">organizerAvailability</span></span>|<span data-ttu-id="dfd33-126">String</span><span class="sxs-lookup"><span data-stu-id="dfd33-126">String</span></span>| <span data-ttu-id="dfd33-p102">この提案されている会議の開催者の空き時間情報。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="dfd33-p102">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="dfd33-129">suggestionHint</span><span class="sxs-lookup"><span data-stu-id="dfd33-129">suggestionHint</span></span>|<span data-ttu-id="dfd33-130">String</span><span class="sxs-lookup"><span data-stu-id="dfd33-130">String</span></span>|<span data-ttu-id="dfd33-131">会議時間を提案する理由。</span><span class="sxs-lookup"><span data-stu-id="dfd33-131">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->