# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="62ba5-101">meetingTimeSuggestionsResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62ba5-101">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="62ba5-102">会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。</span><span class="sxs-lookup"><span data-stu-id="62ba5-102">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="62ba5-103">[findMeetingTimes](../api/user_findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="62ba5-103">The following are the possible reasons that [findMeetingTimes](../api/user_findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="62ba5-104">**emptySuggestionsReason 値**</span><span class="sxs-lookup"><span data-stu-id="62ba5-104">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="62ba5-105">**理由**</span><span class="sxs-lookup"><span data-stu-id="62ba5-105">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="62ba5-106">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="62ba5-106">attendeesUnavailable</span></span> | <span data-ttu-id="62ba5-107">すべての出席者の空き時間情報を把握していますが、[会議の確実性](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)しきい値 (既定では 50%) に達するにはすべての時間帯で出席者が足りません。</span><span class="sxs-lookup"><span data-stu-id="62ba5-107">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="62ba5-108">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="62ba5-108">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="62ba5-p101">一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。</span><span class="sxs-lookup"><span data-stu-id="62ba5-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="62ba5-111">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="62ba5-111">locationsUnavailable</span></span> | <span data-ttu-id="62ba5-112">**LocationConstraint** の [IsRequired](locationconstraint.md) プロパティが必須に指定されているものの、算出された時間範囲で利用可能な場所がありません。</span><span class="sxs-lookup"><span data-stu-id="62ba5-112">The **IsRequired** property of the [LocationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="62ba5-113">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="62ba5-113">organizerUnavailable</span></span> | <span data-ttu-id="62ba5-114">**IsOrganizerOptional** パラメーターが false で、要求された期間中、主催者が現時点で出席可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="62ba5-114">The **IsOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="62ba5-115">不明</span><span class="sxs-lookup"><span data-stu-id="62ba5-115">unknown</span></span> | <span data-ttu-id="62ba5-116">会議提案が 1 つも返されない理由が不明です。</span><span class="sxs-lookup"><span data-stu-id="62ba5-116">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62ba5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62ba5-117">JSON representation</span></span>

<span data-ttu-id="62ba5-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="62ba5-118">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="62ba5-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62ba5-119">Properties</span></span>
| <span data-ttu-id="62ba5-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62ba5-120">Property</span></span>     | <span data-ttu-id="62ba5-121">タイプ</span><span class="sxs-lookup"><span data-stu-id="62ba5-121">Type</span></span>   |<span data-ttu-id="62ba5-122">説明</span><span class="sxs-lookup"><span data-stu-id="62ba5-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62ba5-123">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="62ba5-123">emptySuggestionsReason</span></span>|<span data-ttu-id="62ba5-124">文字列</span><span class="sxs-lookup"><span data-stu-id="62ba5-124">String</span></span>|<span data-ttu-id="62ba5-125">会議提案が 1 つも返されない理由。</span><span class="sxs-lookup"><span data-stu-id="62ba5-125">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="62ba5-126">使用可能な値は、`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="62ba5-126">The possible values are `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, , , , , , , , or `unknown`.</span></span> <span data-ttu-id="62ba5-127"> **MeetingTimeSuggestions** プロパティは、会議の提案を含める場合、このプロパティは空の文字列をします。</span><span class="sxs-lookup"><span data-stu-id="62ba5-127">A reason for not returning any meeting suggestions. Possible values are: , , , , or . This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="62ba5-128">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="62ba5-128">meetingTimeSuggestions</span></span>|<span data-ttu-id="62ba5-129">[meetingTimeSuggestion](meetingTimeSuggestion.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62ba5-129">[meetingTimeSuggestion](meetingTimeSuggestion.md) collection</span></span>|<span data-ttu-id="62ba5-130">会議提案の配列。</span><span class="sxs-lookup"><span data-stu-id="62ba5-130">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->