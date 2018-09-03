# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="e1805-101">meetingTimeSuggestion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1805-101">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="e1805-102">会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。</span><span class="sxs-lookup"><span data-stu-id="e1805-102">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1805-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1805-103">JSON representation</span></span>

<span data-ttu-id="e1805-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e1805-104">Here is a JSON representation of the resource</span></span>

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
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="e1805-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1805-105">Properties</span></span>
| <span data-ttu-id="e1805-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1805-106">Property</span></span>     | <span data-ttu-id="e1805-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="e1805-107">Type</span></span>   |<span data-ttu-id="e1805-108">説明</span><span class="sxs-lookup"><span data-stu-id="e1805-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1805-109">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="e1805-109">attendeeAvailability</span></span>|<span data-ttu-id="e1805-110">[attendeeAvailability](attendeeavailability.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1805-110">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="e1805-111">この提案された会議の各出席者の空き時間情報の状態を示す配列。</span><span class="sxs-lookup"><span data-stu-id="e1805-111">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="e1805-112">confidence</span><span class="sxs-lookup"><span data-stu-id="e1805-112">confidence</span></span>|<span data-ttu-id="e1805-113">Double</span><span class="sxs-lookup"><span data-stu-id="e1805-113">Double</span></span>|<span data-ttu-id="e1805-114">すべての出席者が出席する見込みを表すパーセンテージ。</span><span class="sxs-lookup"><span data-stu-id="e1805-114">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="e1805-115">locations</span><span class="sxs-lookup"><span data-stu-id="e1805-115">locations</span></span>|<span data-ttu-id="e1805-116">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1805-116">[location](location.md) collection</span></span>|<span data-ttu-id="e1805-117">この提案された会議の各会議場所の名前と地理的な場所を指定する配列。</span><span class="sxs-lookup"><span data-stu-id="e1805-117">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="e1805-118">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="e1805-118">meetingTimeSlot</span></span>|[<span data-ttu-id="e1805-119">timeSlot</span><span class="sxs-lookup"><span data-stu-id="e1805-119">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="e1805-120">会議の提案されている期間。</span><span class="sxs-lookup"><span data-stu-id="e1805-120">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="e1805-121">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="e1805-121">organizerAvailability</span></span>|<span data-ttu-id="e1805-122">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="e1805-122">FreeBusyStatus</span></span>| <span data-ttu-id="e1805-123">この提案された会議の会議の開催者の可用性。</span><span class="sxs-lookup"><span data-stu-id="e1805-123">Availability of the meeting organizer for this meeting suggestion: , , , , , .</span></span> <span data-ttu-id="e1805-124">可能な値は、`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="e1805-124">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|
|<span data-ttu-id="e1805-125">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="e1805-125">suggestionReason</span></span>|<span data-ttu-id="e1805-126">文字列</span><span class="sxs-lookup"><span data-stu-id="e1805-126">String</span></span>|<span data-ttu-id="e1805-127">会議時間を提案する理由。</span><span class="sxs-lookup"><span data-stu-id="e1805-127">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->