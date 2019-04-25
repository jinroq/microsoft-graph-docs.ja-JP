---
title: meetingTimeSuggestionsResult リソースの種類
description: 会議の提案がある場合は、そのコレクション。また、存在しない場合は理由があります。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 654e53c5a3a329774e1b78065bb8cbcd41d6721f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581596"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="9b9a5-103">meetingTimeSuggestionsResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b9a5-103">meetingTimeSuggestionsResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b9a5-104">会議の提案がある場合は、そのコレクション。また、存在しない場合は理由があります。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-104">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="9b9a5-105">[findMeetingTimes](../api/user-findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="9b9a5-106">**emptySuggestionsReason value**</span><span class="sxs-lookup"><span data-stu-id="9b9a5-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="9b9a5-107">**理由**</span><span class="sxs-lookup"><span data-stu-id="9b9a5-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="9b9a5-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="9b9a5-108">attendeesUnavailable</span></span> | <span data-ttu-id="9b9a5-109">すべての出席者の空き時間情報がわかっていますが、[会議の信頼度](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)のしきい値 (既定では 50%) に到達できる十分な出席者がいません。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="9b9a5-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="9b9a5-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="9b9a5-p101">一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="9b9a5-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="9b9a5-113">locationsUnavailable</span></span> | <span data-ttu-id="9b9a5-114">**locationConstraint**パラメーターの**isRequired**プロパティは true と指定されていますが、計算された時間帯に使用可能な場所がありません。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-114">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="9b9a5-115">組織が利用できません</span><span class="sxs-lookup"><span data-stu-id="9b9a5-115">organizerUnavailable</span></span> | <span data-ttu-id="9b9a5-116">**IsOrganizerOptional** パラメーターが false で、要求された時間枠では、主催者が現時点で出席可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="9b9a5-117">不明</span><span class="sxs-lookup"><span data-stu-id="9b9a5-117">unknown</span></span> | <span data-ttu-id="9b9a5-118">会議提案が 1 つも返されない理由が不明です。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b9a5-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b9a5-119">JSON representation</span></span>

<span data-ttu-id="9b9a5-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9b9a5-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a><span data-ttu-id="9b9a5-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b9a5-121">Properties</span></span>
| <span data-ttu-id="9b9a5-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b9a5-122">Property</span></span>     | <span data-ttu-id="9b9a5-123">型</span><span class="sxs-lookup"><span data-stu-id="9b9a5-123">Type</span></span>   |<span data-ttu-id="9b9a5-124">説明</span><span class="sxs-lookup"><span data-stu-id="9b9a5-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b9a5-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="9b9a5-125">emptySuggestionsReason</span></span>|<span data-ttu-id="9b9a5-126">String</span><span class="sxs-lookup"><span data-stu-id="9b9a5-126">String</span></span>|<span data-ttu-id="9b9a5-127">会議提案が 1 つも返されない理由。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-127">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="9b9a5-128">可能な値は、`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-128">Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="9b9a5-129">会議の**タイム times/ge/アドオン**プロパティに会議の提案が含まれている場合、このプロパティは空の文字列になります。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-129">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="9b9a5-130">会議のタイムスパン</span><span class="sxs-lookup"><span data-stu-id="9b9a5-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="9b9a5-131">[meetingTimeSuggestion](meetingtimesuggestion.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9b9a5-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="9b9a5-132">会議提案の配列。</span><span class="sxs-lookup"><span data-stu-id="9b9a5-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestionsresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->