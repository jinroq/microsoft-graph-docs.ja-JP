# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="4b2a2-101">daylightTimeZoneOffset リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b2a2-101">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="4b2a2-102">タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-102">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="4b2a2-103">たとえば、タイム ゾーンに次のプロパティが指定されているとします。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="4b2a2-104">**bias**: 300</span><span class="sxs-lookup"><span data-stu-id="4b2a2-104">**bias** is 300</span></span>
- <span data-ttu-id="4b2a2-105">**daylightBias**: -100</span><span class="sxs-lookup"><span data-stu-id="4b2a2-105">**daylightBias** is -100</span></span>
- <span data-ttu-id="4b2a2-106">**dayOccurrence**: 4</span><span class="sxs-lookup"><span data-stu-id="4b2a2-106">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="4b2a2-107">**dayOfWeek**: "日曜日"</span><span class="sxs-lookup"><span data-stu-id="4b2a2-107">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="4b2a2-108">**month**: 5</span><span class="sxs-lookup"><span data-stu-id="4b2a2-108">**month** is 5</span></span>
- <span data-ttu-id="4b2a2-109">**time** は 02:00:00 で、_ **year** は 0 です。つまり、夏時間の間は、時刻が UTC より +300-100=200 分進んでいることを意味します。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-109">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="4b2a2-110">夏時間から標準時への切り替えは、毎年 5 月の第 4 日曜日の午前 2 時に行われます。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-110">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="4b2a2-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b2a2-111">Properties</span></span>
| <span data-ttu-id="4b2a2-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b2a2-112">Property</span></span>     | <span data-ttu-id="4b2a2-113">タイプ</span><span class="sxs-lookup"><span data-stu-id="4b2a2-113">Type</span></span>   |<span data-ttu-id="4b2a2-114">説明</span><span class="sxs-lookup"><span data-stu-id="4b2a2-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b2a2-115">daylightBias</span><span class="sxs-lookup"><span data-stu-id="4b2a2-115">daylightBias</span></span> | <span data-ttu-id="4b2a2-116">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="4b2a2-116">Edm.Int32</span></span> | <span data-ttu-id="4b2a2-117">夏時間の協定世界時 (UTC) からの時間オフセットです。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-117">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="4b2a2-118">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-118">This value is in minutes.</span></span>  |
| <span data-ttu-id="4b2a2-119">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="4b2a2-119">dayOccurrence</span></span> | <span data-ttu-id="4b2a2-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="4b2a2-120">Edm.Int32</span></span> | <span data-ttu-id="4b2a2-121">標準時から夏時間への切り替えが月の何番目の曜日に行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-121">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="4b2a2-122">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="4b2a2-122">dayOfWeek</span></span> | <span data-ttu-id="4b2a2-123">文字列</span><span class="sxs-lookup"><span data-stu-id="4b2a2-123">string</span></span> | <span data-ttu-id="4b2a2-124">標準時から夏時間への切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-124">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="4b2a2-125">month</span><span class="sxs-lookup"><span data-stu-id="4b2a2-125">month</span></span> | <span data-ttu-id="4b2a2-126">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="4b2a2-126">Edm.Int32</span></span> | <span data-ttu-id="4b2a2-127">標準時から夏時間への切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-127">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="4b2a2-128">time</span><span class="sxs-lookup"><span data-stu-id="4b2a2-128">time</span></span> | <span data-ttu-id="4b2a2-129">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4b2a2-129">Edm.TimeOfDay</span></span> | <span data-ttu-id="4b2a2-130">標準時から夏時間への切り替えが行われる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-130">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="4b2a2-131">year</span><span class="sxs-lookup"><span data-stu-id="4b2a2-131">year</span></span> | <span data-ttu-id="4b2a2-132">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="4b2a2-132">Edm.Int32</span></span> | <span data-ttu-id="4b2a2-133">標準時から夏時間への切り替えが年に何回行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-133">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="4b2a2-134">たとえば、値 0 は年に 1 回を意味します。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-134">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4b2a2-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b2a2-135">JSON representation</span></span>

<span data-ttu-id="4b2a2-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b2a2-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.standardTimeZoneOffset",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->