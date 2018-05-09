# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="cddca-101">standardTimeZoneOffset リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cddca-101">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="cddca-102">タイム ゾーンが夏時間から標準時に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="cddca-102">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="cddca-103">たとえば、タイム ゾーンに次のプロパティが指定されているとします。</span><span class="sxs-lookup"><span data-stu-id="cddca-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="cddca-104">**dayOccurrence**: 3</span><span class="sxs-lookup"><span data-stu-id="cddca-104">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="cddca-105">**dayOfWeek**: "日曜日"</span><span class="sxs-lookup"><span data-stu-id="cddca-105">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="cddca-106">**month**: 10</span><span class="sxs-lookup"><span data-stu-id="cddca-106">**month** is 10</span></span>
- <span data-ttu-id="cddca-107">**time** は 02:00:00 で、_ **year** は 0 です。つまり、夏時間から標準時への切り替えは、毎年 10 月の第 3 日曜日の午前 2 時に行われることを意味します。</span><span class="sxs-lookup"><span data-stu-id="cddca-107">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="cddca-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cddca-108">Properties</span></span>
| <span data-ttu-id="cddca-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cddca-109">Property</span></span>     | <span data-ttu-id="cddca-110">型</span><span class="sxs-lookup"><span data-stu-id="cddca-110">Type</span></span>   |<span data-ttu-id="cddca-111">説明</span><span class="sxs-lookup"><span data-stu-id="cddca-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cddca-112">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="cddca-112">dayOccurrence</span></span> | <span data-ttu-id="cddca-113">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="cddca-113">Edm.Int32</span></span> | <span data-ttu-id="cddca-114">夏時間から標準時への切り替えが月の何番目の曜日に行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="cddca-114">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="cddca-115">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="cddca-115">DayOfWeek</span></span> | <span data-ttu-id="cddca-116">string</span><span class="sxs-lookup"><span data-stu-id="cddca-116">string</span></span> | <span data-ttu-id="cddca-117">夏時間から標準時への切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="cddca-117">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="cddca-118">month</span><span class="sxs-lookup"><span data-stu-id="cddca-118">month</span></span> | <span data-ttu-id="cddca-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="cddca-119">Edm.Int32</span></span> | <span data-ttu-id="cddca-120">夏時間から標準時への切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="cddca-120">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="cddca-121">time</span><span class="sxs-lookup"><span data-stu-id="cddca-121">time</span></span> | <span data-ttu-id="cddca-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cddca-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="cddca-123">夏時間から標準時への切り替えが行われる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="cddca-123">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="cddca-124">year</span><span class="sxs-lookup"><span data-stu-id="cddca-124">year</span></span> | <span data-ttu-id="cddca-125">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="cddca-125">Edm.Int32</span></span> | <span data-ttu-id="cddca-126">夏時間から標準時への切り替えが年に何回行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="cddca-126">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="cddca-127">たとえば、値 0 は年に 1 回を意味します。</span><span class="sxs-lookup"><span data-stu-id="cddca-127">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cddca-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cddca-128">JSON representation</span></span>

<span data-ttu-id="cddca-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cddca-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
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
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->