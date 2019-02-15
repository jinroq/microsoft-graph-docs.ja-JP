---
title: meetingTimeSuggestion リソースの種類
description: '会議の時間、出席の可能性、個人などの情報を含む会議の提案 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 379bb4ac4be8e2d8d1bec494cf4d573550d46b55
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057030"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="7ac7d-103">meetingTimeSuggestion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7ac7d-103">meetingTimeSuggestion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ac7d-104">会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。</span><span class="sxs-lookup"><span data-stu-id="7ac7d-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ac7d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ac7d-105">JSON representation</span></span>

<span data-ttu-id="7ac7d-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7ac7d-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.locationDataModel"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.meetingTimeSlotDataModel"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="7ac7d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ac7d-107">Properties</span></span>
| <span data-ttu-id="7ac7d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ac7d-108">Property</span></span>     | <span data-ttu-id="7ac7d-109">種類</span><span class="sxs-lookup"><span data-stu-id="7ac7d-109">Type</span></span>   |<span data-ttu-id="7ac7d-110">説明</span><span class="sxs-lookup"><span data-stu-id="7ac7d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ac7d-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="7ac7d-111">attendeeAvailability</span></span>|<span data-ttu-id="7ac7d-112">[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ac7d-112">[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md) collection</span></span>|<span data-ttu-id="7ac7d-113">この提案された会議の各出席者の空き時間情報の状態を示す配列。</span><span class="sxs-lookup"><span data-stu-id="7ac7d-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="7ac7d-114">confidence</span><span class="sxs-lookup"><span data-stu-id="7ac7d-114">confidence</span></span>|<span data-ttu-id="7ac7d-115">Double</span><span class="sxs-lookup"><span data-stu-id="7ac7d-115">Double</span></span>|<span data-ttu-id="7ac7d-116">すべての出席者が出席する見込みを表すパーセンテージ。</span><span class="sxs-lookup"><span data-stu-id="7ac7d-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="7ac7d-117">locations</span><span class="sxs-lookup"><span data-stu-id="7ac7d-117">locations</span></span>|<span data-ttu-id="7ac7d-118">[locationDataModel](locationdatamodel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ac7d-118">[locationDataModel](locationdatamodel.md) collection</span></span>|<span data-ttu-id="7ac7d-119">この提案された会議の各会議場所の名前と地理的な場所を指定する配列。</span><span class="sxs-lookup"><span data-stu-id="7ac7d-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="7ac7d-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="7ac7d-120">meetingTimeSlot</span></span>|[<span data-ttu-id="7ac7d-121">meetingTimeSlotDataModel</span><span class="sxs-lookup"><span data-stu-id="7ac7d-121">meetingTimeSlotDataModel</span></span>](meetingtimeslotdatamodel.md)|<span data-ttu-id="7ac7d-122">会議の提案されている期間。</span><span class="sxs-lookup"><span data-stu-id="7ac7d-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="7ac7d-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="7ac7d-123">organizerAvailability</span></span>|<span data-ttu-id="7ac7d-124">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="7ac7d-124">availabilityStatus</span></span>| <span data-ttu-id="7ac7d-p101">この提案されている会議の開催者の空き時間情報。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="7ac7d-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="7ac7d-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="7ac7d-127">suggestionReason</span></span>|<span data-ttu-id="7ac7d-128">String</span><span class="sxs-lookup"><span data-stu-id="7ac7d-128">String</span></span>|<span data-ttu-id="7ac7d-129">会議時間を提案する理由。</span><span class="sxs-lookup"><span data-stu-id="7ac7d-129">Reason for suggesting the meeting time.</span></span>|

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
