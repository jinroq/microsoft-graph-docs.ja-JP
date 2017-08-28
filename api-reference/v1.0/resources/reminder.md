# <a name="reminder-resource-type"></a><span data-ttu-id="aa6f1-101">アラーム リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa6f1-101">reminder resource type</span></span>



## <a name="properties"></a><span data-ttu-id="aa6f1-102">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa6f1-102">Properties</span></span>
| <span data-ttu-id="aa6f1-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa6f1-103">Property</span></span>     | <span data-ttu-id="aa6f1-104">型</span><span class="sxs-lookup"><span data-stu-id="aa6f1-104">Type</span></span>   |<span data-ttu-id="aa6f1-105">説明</span><span class="sxs-lookup"><span data-stu-id="aa6f1-105">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa6f1-106">changeKey</span><span class="sxs-lookup"><span data-stu-id="aa6f1-106">changeKey</span></span>|<span data-ttu-id="aa6f1-107">String</span><span class="sxs-lookup"><span data-stu-id="aa6f1-107">String</span></span>|<span data-ttu-id="aa6f1-p101">アラームのバージョンを識別します。アラームを変更するたびに **changeKey** も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="aa6f1-111">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="aa6f1-111">eventEndTime</span></span>|[<span data-ttu-id="aa6f1-112">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="aa6f1-112">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="aa6f1-113">イベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-113">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="aa6f1-114">eventId</span><span class="sxs-lookup"><span data-stu-id="aa6f1-114">eventId</span></span>|<span data-ttu-id="aa6f1-115">String</span><span class="sxs-lookup"><span data-stu-id="aa6f1-115">String</span></span>|<span data-ttu-id="aa6f1-p102">イベントの一意の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="aa6f1-118">eventLocation</span><span class="sxs-lookup"><span data-stu-id="aa6f1-118">eventLocation</span></span>|[<span data-ttu-id="aa6f1-119">Location</span><span class="sxs-lookup"><span data-stu-id="aa6f1-119">Location</span></span>](location.md)|<span data-ttu-id="aa6f1-120">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-120">The location of the event.</span></span>|
|<span data-ttu-id="aa6f1-121">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="aa6f1-121">eventStartTime</span></span>|[<span data-ttu-id="aa6f1-122">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="aa6f1-122">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="aa6f1-123">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-123">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="aa6f1-124">eventSubject</span><span class="sxs-lookup"><span data-stu-id="aa6f1-124">eventSubject</span></span>|<span data-ttu-id="aa6f1-125">String</span><span class="sxs-lookup"><span data-stu-id="aa6f1-125">String</span></span>|<span data-ttu-id="aa6f1-126">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-126">The text of the event's subject line.</span></span>|
|<span data-ttu-id="aa6f1-127">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="aa6f1-127">eventWebLink</span></span>|<span data-ttu-id="aa6f1-128">String</span><span class="sxs-lookup"><span data-stu-id="aa6f1-128">String</span></span>|<span data-ttu-id="aa6f1-129">Web 上の Outlook でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-129">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="aa6f1-p103">Web 上の Outlook のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="aa6f1-132">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-132">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="aa6f1-133">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="aa6f1-133">reminderFireTime</span></span>|[<span data-ttu-id="aa6f1-134">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="aa6f1-134">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="aa6f1-135">アラームの発生を設定する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-135">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa6f1-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa6f1-136">JSON representation</span></span>

<span data-ttu-id="aa6f1-137">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="aa6f1-137">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->