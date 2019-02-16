---
title: findmeetingtimesresponse リソースの種類
description: 会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0d52da8e5798932d4f78463d6e4bea08ecb7c793
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057399"
---
# <a name="findmeetingtimesresponse-resource-type"></a><span data-ttu-id="f6de8-103">findmeetingtimesresponse リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6de8-103">findMeetingTimesResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6de8-104">会議の提案がある場合は、そのコレクション。また、存在しない場合は理由があります。</span><span class="sxs-lookup"><span data-stu-id="f6de8-104">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="f6de8-105">[findMeetingTimes](../api/user-findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="f6de8-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="f6de8-106">**emptySuggestionsReason value**</span><span class="sxs-lookup"><span data-stu-id="f6de8-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="f6de8-107">**理由**</span><span class="sxs-lookup"><span data-stu-id="f6de8-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="f6de8-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="f6de8-108">attendeesUnavailable</span></span> | <span data-ttu-id="f6de8-109">すべての出席者の空き時間情報を把握していますが、[会議の確実性](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)しきい値 (既定では 50%) に達するにはすべての時間帯で出席者が足りません。</span><span class="sxs-lookup"><span data-stu-id="f6de8-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="f6de8-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="f6de8-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="f6de8-p101">一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。</span><span class="sxs-lookup"><span data-stu-id="f6de8-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="f6de8-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="f6de8-113">locationsUnavailable</span></span> | <span data-ttu-id="f6de8-114">**locationConstraint**パラメーターの**isRequired**プロパティは true と指定されていますが、計算された時間帯に使用可能な場所がありません。</span><span class="sxs-lookup"><span data-stu-id="f6de8-114">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="f6de8-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="f6de8-115">organizerUnavailable</span></span> | <span data-ttu-id="f6de8-116">**IsOrganizerOptional** パラメーターが false で、要求された時間枠では、主催者が現時点で出席可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="f6de8-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="f6de8-117">不明</span><span class="sxs-lookup"><span data-stu-id="f6de8-117">unknown</span></span> | <span data-ttu-id="f6de8-118">会議提案が 1 つも返されない理由が不明です。</span><span class="sxs-lookup"><span data-stu-id="f6de8-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6de8-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6de8-119">JSON representation</span></span>

<span data-ttu-id="f6de8-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f6de8-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesResponse"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a><span data-ttu-id="f6de8-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6de8-121">Properties</span></span>
| <span data-ttu-id="f6de8-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6de8-122">Property</span></span>     | <span data-ttu-id="f6de8-123">型</span><span class="sxs-lookup"><span data-stu-id="f6de8-123">Type</span></span>   |<span data-ttu-id="f6de8-124">説明</span><span class="sxs-lookup"><span data-stu-id="f6de8-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6de8-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="f6de8-125">emptySuggestionsReason</span></span>|<span data-ttu-id="f6de8-126">String</span><span class="sxs-lookup"><span data-stu-id="f6de8-126">String</span></span>|<span data-ttu-id="f6de8-p102">会議提案が 1 つも返されない理由。使用可能な値: `attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、`unknown`。このプロパティは、**meetingTimeSuggestions** プロパティに会議提案が含まれる場合は空の文字列です。</span><span class="sxs-lookup"><span data-stu-id="f6de8-p102">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="f6de8-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="f6de8-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="f6de8-131">[meetingTimeSuggestion](meetingtimesuggestion.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f6de8-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="f6de8-132">会議提案の配列。</span><span class="sxs-lookup"><span data-stu-id="f6de8-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimesresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->