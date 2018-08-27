# <a name="reminder-resource-type"></a><span data-ttu-id="53747-101">アラーム リソースの種類</span><span class="sxs-lookup"><span data-stu-id="53747-101">reminder resource type</span></span>

<span data-ttu-id="53747-102">ユーザーの[予定表](event.md)の[イベント](calendar.md)を通知します。</span><span class="sxs-lookup"><span data-stu-id="53747-102">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="53747-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53747-103">Properties</span></span>
| <span data-ttu-id="53747-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53747-104">Property</span></span>     | <span data-ttu-id="53747-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="53747-105">Type</span></span>   |<span data-ttu-id="53747-106">説明</span><span class="sxs-lookup"><span data-stu-id="53747-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53747-107">changeKey</span><span class="sxs-lookup"><span data-stu-id="53747-107">changeKey</span></span>|<span data-ttu-id="53747-108">文字列</span><span class="sxs-lookup"><span data-stu-id="53747-108">String</span></span>|<span data-ttu-id="53747-p101">アラームのバージョンを識別します。アラームを変更するたびに **changeKey** も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="53747-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="53747-112">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="53747-112">eventEndTime</span></span>|[<span data-ttu-id="53747-113">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="53747-113">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="53747-114">イベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="53747-114">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="53747-115">eventId</span><span class="sxs-lookup"><span data-stu-id="53747-115">eventId</span></span>|<span data-ttu-id="53747-116">文字列</span><span class="sxs-lookup"><span data-stu-id="53747-116">String</span></span>|<span data-ttu-id="53747-p102">イベントの一意の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53747-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="53747-119">eventLocation</span><span class="sxs-lookup"><span data-stu-id="53747-119">eventLocation</span></span>|[<span data-ttu-id="53747-120">Location</span><span class="sxs-lookup"><span data-stu-id="53747-120">Location</span></span>](location.md)|<span data-ttu-id="53747-121">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="53747-121">The location of the event.</span></span>|
|<span data-ttu-id="53747-122">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="53747-122">eventStartTime</span></span>|[<span data-ttu-id="53747-123">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="53747-123">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="53747-124">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="53747-124">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="53747-125">eventSubject</span><span class="sxs-lookup"><span data-stu-id="53747-125">eventSubject</span></span>|<span data-ttu-id="53747-126">文字列</span><span class="sxs-lookup"><span data-stu-id="53747-126">String</span></span>|<span data-ttu-id="53747-127">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="53747-127">The text of the event's subject line.</span></span>|
|<span data-ttu-id="53747-128">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="53747-128">eventWebLink</span></span>|<span data-ttu-id="53747-129">文字列</span><span class="sxs-lookup"><span data-stu-id="53747-129">String</span></span>|<span data-ttu-id="53747-130">Web 上の Outlook でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="53747-130">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="53747-p103">Web 上の Outlook のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="53747-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="53747-133">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="53747-133">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="53747-134">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="53747-134">reminderFireTime</span></span>|[<span data-ttu-id="53747-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="53747-135">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="53747-136">アラームの発生を設定する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="53747-136">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53747-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="53747-137">JSON representation</span></span>

<span data-ttu-id="53747-138">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="53747-138">Here is a JSON representation of the resource</span></span>

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