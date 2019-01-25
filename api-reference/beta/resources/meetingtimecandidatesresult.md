---
title: meetingTimeCandidatesResult リソースの種類
description: 会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: e60c0092ca5724e4019a4c3f75f1239a0e7e9c0b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507517"
---
# <a name="meetingtimecandidatesresult-resource-type"></a><span data-ttu-id="90ff2-103">meetingTimeCandidatesResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90ff2-103">meetingTimeCandidatesResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90ff2-104">会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。</span><span class="sxs-lookup"><span data-stu-id="90ff2-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="90ff2-105">findMeetingTimes が会議の提案を何も返さない理由として考えられるものを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="90ff2-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="90ff2-106">**emptySuggestionsHint 値**</span><span class="sxs-lookup"><span data-stu-id="90ff2-106">**emptySuggestionsHint value**</span></span>|<span data-ttu-id="90ff2-107">**理由**</span><span class="sxs-lookup"><span data-stu-id="90ff2-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="90ff2-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="90ff2-108">attendeesUnavailable</span></span> | <span data-ttu-id="90ff2-109">すべての出席者の空き時間情報を把握していますが、会議の確実性しきい値 (既定では 50%) に達するにはすべての時間帯で出席者が足りません。</span><span class="sxs-lookup"><span data-stu-id="90ff2-109">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period.</span></span> <span data-ttu-id="90ff2-110">このしきい値は、出席者の空き/予約済みの状態の提案された会議の期間、出勤、[不明] 状態の 50%、および 0% のビジー状態の可能性が 100% に対応する出席者の空きの状態に基づきます。</span><span class="sxs-lookup"><span data-stu-id="90ff2-110">This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 50%, and busy status 0%.</span></span>|
| <span data-ttu-id="90ff2-111">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="90ff2-111">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="90ff2-p102">一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。</span><span class="sxs-lookup"><span data-stu-id="90ff2-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="90ff2-114">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="90ff2-114">locationsUnavailable</span></span> | <span data-ttu-id="90ff2-115">[locationConstraint](locationconstraint.md) の **isRequired** プロパティが必須に指定されているものの、算出された時間範囲で利用可能な場所がありません。</span><span class="sxs-lookup"><span data-stu-id="90ff2-115">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="90ff2-116">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="90ff2-116">organizerUnavailable</span></span> | <span data-ttu-id="90ff2-117">**IsOrganizerOptional** パラメーターが false で、要求された時間枠では、主催者が現時点で出席可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="90ff2-117">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="90ff2-118">不明</span><span class="sxs-lookup"><span data-stu-id="90ff2-118">unknown</span></span> | <span data-ttu-id="90ff2-119">会議提案が 1 つも返されない理由が不明です。</span><span class="sxs-lookup"><span data-stu-id="90ff2-119">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90ff2-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90ff2-120">JSON representation</span></span>

<span data-ttu-id="90ff2-121">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="90ff2-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a><span data-ttu-id="90ff2-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90ff2-122">Properties</span></span>
| <span data-ttu-id="90ff2-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90ff2-123">Property</span></span>     | <span data-ttu-id="90ff2-124">型</span><span class="sxs-lookup"><span data-stu-id="90ff2-124">Type</span></span>   |<span data-ttu-id="90ff2-125">説明</span><span class="sxs-lookup"><span data-stu-id="90ff2-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90ff2-126">emptySuggestionsHint</span><span class="sxs-lookup"><span data-stu-id="90ff2-126">emptySuggestionsHint</span></span>|<span data-ttu-id="90ff2-127">String</span><span class="sxs-lookup"><span data-stu-id="90ff2-127">String</span></span>|<span data-ttu-id="90ff2-p103">会議提案が 1 つも返されない理由。可能な値: `attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、または `unknown`。</span><span class="sxs-lookup"><span data-stu-id="90ff2-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span>|
|<span data-ttu-id="90ff2-130">meetingTimeSlots</span><span class="sxs-lookup"><span data-stu-id="90ff2-130">meetingTimeSlots</span></span>|<span data-ttu-id="90ff2-131">[meetingTimeCandidate](meetingtimecandidate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="90ff2-131">[meetingTimeCandidate](meetingtimecandidate.md) collection</span></span>|<span data-ttu-id="90ff2-132">会議提案の配列。</span><span class="sxs-lookup"><span data-stu-id="90ff2-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimecandidatesresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
