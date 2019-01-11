---
title: meetingTimeSuggestionsResult リソースの種類
description: 会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。
localization_priority: Normal
ms.openlocfilehash: 85a0c3ade54204cb78957e81325869197f403c5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823696"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="543fb-103">meetingTimeSuggestionsResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="543fb-103">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="543fb-104">会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。</span><span class="sxs-lookup"><span data-stu-id="543fb-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="543fb-105">[findMeetingTimes](../api/user-findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="543fb-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="543fb-106">**emptySuggestionsReason value**</span><span class="sxs-lookup"><span data-stu-id="543fb-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="543fb-107">**理由**</span><span class="sxs-lookup"><span data-stu-id="543fb-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="543fb-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="543fb-108">attendeesUnavailable</span></span> | <span data-ttu-id="543fb-109">すべての出席者の空き時間情報を把握していますが、[会議の確実性](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)しきい値 (既定では 50%) に達するにはすべての時間帯で出席者が足りません。</span><span class="sxs-lookup"><span data-stu-id="543fb-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="543fb-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="543fb-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="543fb-p101">一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。</span><span class="sxs-lookup"><span data-stu-id="543fb-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="543fb-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="543fb-113">locationsUnavailable</span></span> | <span data-ttu-id="543fb-114">[locationConstraint](locationconstraint.md) の **isRequired** プロパティが必須に指定されているものの、算出された時間範囲で利用可能な場所がありません。</span><span class="sxs-lookup"><span data-stu-id="543fb-114">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="543fb-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="543fb-115">organizerUnavailable</span></span> | <span data-ttu-id="543fb-116">**IsOrganizerOptional** パラメーターが false で、要求された時間枠では、主催者が現時点で出席可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="543fb-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="543fb-117">不明</span><span class="sxs-lookup"><span data-stu-id="543fb-117">unknown</span></span> | <span data-ttu-id="543fb-118">会議提案が 1 つも返されない理由が不明です。</span><span class="sxs-lookup"><span data-stu-id="543fb-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="543fb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="543fb-119">JSON representation</span></span>

<span data-ttu-id="543fb-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="543fb-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="543fb-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="543fb-121">Properties</span></span>
| <span data-ttu-id="543fb-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="543fb-122">Property</span></span>     | <span data-ttu-id="543fb-123">種類</span><span class="sxs-lookup"><span data-stu-id="543fb-123">Type</span></span>   |<span data-ttu-id="543fb-124">説明</span><span class="sxs-lookup"><span data-stu-id="543fb-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="543fb-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="543fb-125">emptySuggestionsReason</span></span>|<span data-ttu-id="543fb-126">String</span><span class="sxs-lookup"><span data-stu-id="543fb-126">String</span></span>|<span data-ttu-id="543fb-127">会議提案が 1 つも返されない理由。</span><span class="sxs-lookup"><span data-stu-id="543fb-127">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="543fb-128">可能な値: `attendeesUnavailable`、 `attendeesUnavailableOrUnknown`、 `locationsUnavailable`、 `organizerUnavailable`、または`unknown`。</span><span class="sxs-lookup"><span data-stu-id="543fb-128">The possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="543fb-129">**MeetingTimeSuggestions**プロパティは、会議の提案を含める場合、このプロパティは空の文字列をします。</span><span class="sxs-lookup"><span data-stu-id="543fb-129">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="543fb-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="543fb-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="543fb-131">[meetingTimeSuggestion](meetingtimesuggestion.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="543fb-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="543fb-132">会議提案の配列。</span><span class="sxs-lookup"><span data-stu-id="543fb-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
