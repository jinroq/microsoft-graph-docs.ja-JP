---
title: meetingTimeSuggestionsResult リソースの種類
description: 会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 3593abdeed0d4c2e5ff1031e559f1f5ce4a66814
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983857"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="fcb59-103">meetingTimeSuggestionsResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fcb59-103">meetingTimeSuggestionsResult resource type</span></span>

> <span data-ttu-id="fcb59-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fcb59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcb59-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fcb59-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fcb59-106">会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb59-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="fcb59-107">[findMeetingTimes](../api/user-findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="fcb59-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="fcb59-108">**emptySuggestionsReason value**</span><span class="sxs-lookup"><span data-stu-id="fcb59-108">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="fcb59-109">**理由**</span><span class="sxs-lookup"><span data-stu-id="fcb59-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="fcb59-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="fcb59-110">attendeesUnavailable</span></span> | <span data-ttu-id="fcb59-111">すべての出席者の空き時間情報を把握していますが、[会議の確実性](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)しきい値 (既定では 50%) に達するにはすべての時間帯で出席者が足りません。</span><span class="sxs-lookup"><span data-stu-id="fcb59-111">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="fcb59-112">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="fcb59-112">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="fcb59-p102">一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。</span><span class="sxs-lookup"><span data-stu-id="fcb59-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="fcb59-115">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="fcb59-115">locationsUnavailable</span></span> | <span data-ttu-id="fcb59-116">[locationConstraint](locationconstraint.md) の **isRequired** プロパティが必須に指定されているものの、算出された時間範囲で利用可能な場所がありません。</span><span class="sxs-lookup"><span data-stu-id="fcb59-116">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="fcb59-117">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="fcb59-117">organizerUnavailable</span></span> | <span data-ttu-id="fcb59-118">**IsOrganizerOptional** パラメーターが false で、要求された時間枠では、主催者が現時点で出席可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="fcb59-118">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="fcb59-119">不明</span><span class="sxs-lookup"><span data-stu-id="fcb59-119">unknown</span></span> | <span data-ttu-id="fcb59-120">会議提案が 1 つも返されない理由が不明です。</span><span class="sxs-lookup"><span data-stu-id="fcb59-120">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fcb59-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fcb59-121">JSON representation</span></span>

<span data-ttu-id="fcb59-122">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fcb59-122">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="fcb59-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fcb59-123">Properties</span></span>
| <span data-ttu-id="fcb59-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fcb59-124">Property</span></span>     | <span data-ttu-id="fcb59-125">型</span><span class="sxs-lookup"><span data-stu-id="fcb59-125">Type</span></span>   |<span data-ttu-id="fcb59-126">説明</span><span class="sxs-lookup"><span data-stu-id="fcb59-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcb59-127">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="fcb59-127">emptySuggestionsReason</span></span>|<span data-ttu-id="fcb59-128">String</span><span class="sxs-lookup"><span data-stu-id="fcb59-128">String</span></span>|<span data-ttu-id="fcb59-p103">会議提案が 1 つも返されない理由。使用可能な値: `attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、`unknown`。このプロパティは、**meetingTimeSuggestions** プロパティに会議提案が含まれる場合は空の文字列です。</span><span class="sxs-lookup"><span data-stu-id="fcb59-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="fcb59-132">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="fcb59-132">meetingTimeSuggestions</span></span>|<span data-ttu-id="fcb59-133">[meetingTimeSuggestion](meetingtimesuggestion.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fcb59-133">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="fcb59-134">会議提案の配列。</span><span class="sxs-lookup"><span data-stu-id="fcb59-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
