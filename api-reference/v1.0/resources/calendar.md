# <a name="calendar-resource-type"></a><span data-ttu-id="00789-101">calendar リソース型</span><span class="sxs-lookup"><span data-stu-id="00789-101">calendar resource type</span></span>

<span data-ttu-id="00789-102">イベントのコンテナーである予定表です。</span><span class="sxs-lookup"><span data-stu-id="00789-102">A calendar which is a container for events.</span></span> <span data-ttu-id="00789-103">[ユーザー](user.md)の予定表、または Office 365 [グループ](group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="00789-103">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="00789-104">**注:** ユーザーの予定表、グループ予定表と対話できるように、いくつかの小さな違いがあります。</span><span class="sxs-lookup"><span data-stu-id="00789-104">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

 - <span data-ttu-id="00789-105">の[calendarGroup](calendargroup.md)のユーザーの予定表のみを整理することができます。</span><span class="sxs-lookup"><span data-stu-id="00789-105">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
 - <span data-ttu-id="00789-106">Outlook は、グループのためのすべての会議出席依頼を自動的に受け入れます。</span><span class="sxs-lookup"><span data-stu-id="00789-106">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="00789-107">ユーザーの予定表のみの[承諾](../api/event_accept.md)、[仮承諾](../api/event_tentativelyaccept.md)、または会議出席依頼を[辞退する](../api/event_decline.md)ことをがします。</span><span class="sxs-lookup"><span data-stu-id="00789-107">You can [accept](../api/event_accept.md), [tentatively accept](../api/event_tentativelyaccept.md), or [decline](../api/event_decline.md)  meeting requests for user calendars only.</span></span>
  - <span data-ttu-id="00789-108">Outlook は、グループのイベントのアラームをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="00789-108">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="00789-109">[再通知](../api/event_snoozereminder.md)や[アラーム](reminder.md)を[消す](../api/event_dismissreminder.md)をユーザーの予定表のみにできます。</span><span class="sxs-lookup"><span data-stu-id="00789-109">You can [snooze](../api/event_snoozereminder.md) or [dismiss](../api/event_dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="00789-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="00789-110">Methods</span></span>

| <span data-ttu-id="00789-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="00789-111">Method</span></span>       | <span data-ttu-id="00789-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="00789-112">Return Type</span></span>  |<span data-ttu-id="00789-113">説明</span><span class="sxs-lookup"><span data-stu-id="00789-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="00789-114">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="00789-114">List calendars</span></span>](../api/user_list_calendars.md)|<span data-ttu-id="00789-115">[calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="00789-115">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="00789-116">ユーザーのすべての予定表を取得するか、既定またはその他の特定の予定表グループの予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="00789-116">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="00789-117">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="00789-117">Create calendar</span></span>](../api/user_post_calendars.md) |[<span data-ttu-id="00789-118">calendar</span><span class="sxs-lookup"><span data-stu-id="00789-118">calendar</span></span>](calendar.md)| <span data-ttu-id="00789-119">既定の予定表グループまたはユーザーの特定の予定表グループに予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="00789-119">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="00789-120">予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="00789-120">Get calendar</span></span>](../api/calendar_get.md) | [<span data-ttu-id="00789-121">calendar</span><span class="sxs-lookup"><span data-stu-id="00789-121">calendar</span></span>](calendar.md) |<span data-ttu-id="00789-122">**予定表**オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="00789-122">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="00789-123">ユーザーの予定表、または Office 365 のグループの既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="00789-123">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="00789-124">更新する</span><span class="sxs-lookup"><span data-stu-id="00789-124">Update</span></span>](../api/calendar_update.md) | [<span data-ttu-id="00789-125">calendar</span><span class="sxs-lookup"><span data-stu-id="00789-125">calendar</span></span>](calendar.md)  |<span data-ttu-id="00789-126">**予定表**オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="00789-126">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="00789-127">ユーザーの予定表、または Office 365 のグループの既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="00789-127">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="00789-128">削除する</span><span class="sxs-lookup"><span data-stu-id="00789-128">Delete</span></span>](../api/calendar_delete.md) | <span data-ttu-id="00789-129">なし</span><span class="sxs-lookup"><span data-stu-id="00789-129">None</span></span> |<span data-ttu-id="00789-130">予定表オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="00789-130">Delete calendar object.</span></span> |
|[<span data-ttu-id="00789-131">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="00789-131">List calendarView</span></span>](../api/calendar_list_calendarview.md) |<span data-ttu-id="00789-132">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="00789-132">[event](event.md) collection</span></span>| <span data-ttu-id="00789-133">ユーザーの標準として設定されている予定表 `(../me/calendarview)` または特定の予定表から、時間範囲で定義したカレンダー ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="00789-133">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="00789-134">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="00789-134">List events</span></span>](../api/calendar_list_events.md) |<span data-ttu-id="00789-135">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="00789-135">[event](event.md) collection</span></span>| <span data-ttu-id="00789-p106">予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="00789-p106">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="00789-138">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="00789-138">Create event</span></span>](../api/calendar_post_events.md) |[<span data-ttu-id="00789-139">event</span><span class="sxs-lookup"><span data-stu-id="00789-139">event</span></span>](event.md)| <span data-ttu-id="00789-140">既定または指定した予定表で新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="00789-140">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="00789-141">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="00789-141">findMeetingTimes</span></span>](../api/user_findmeetingtimes.md) |[<span data-ttu-id="00789-142">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="00789-142">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="00789-143">会議の時間と開催者と出席者の可用性、および時間や場所の制約に基づいて場所をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="00789-143">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="00789-144">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="00789-144">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="00789-145">calendar</span><span class="sxs-lookup"><span data-stu-id="00789-145">calendar</span></span>](calendar.md)  |<span data-ttu-id="00789-146">新規または既存の予定表に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="00789-146">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="00789-147">単一値の拡張プロパティを持つ予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="00789-147">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="00789-148">calendar</span><span class="sxs-lookup"><span data-stu-id="00789-148">calendar</span></span>](calendar.md) | <span data-ttu-id="00789-149">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="00789-149">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="00789-150">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="00789-150">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="00789-151">calendar</span><span class="sxs-lookup"><span data-stu-id="00789-151">calendar</span></span>](calendar.md) | <span data-ttu-id="00789-152">新規または既存の予定表に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="00789-152">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="00789-153">複数値の拡張プロパティを持つ予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="00789-153">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="00789-154">calendar</span><span class="sxs-lookup"><span data-stu-id="00789-154">calendar</span></span>](calendar.md) | <span data-ttu-id="00789-155">`$expand` を使用して、複数値の拡張プロパティを含む予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="00789-155">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="00789-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00789-156">Properties</span></span>
| <span data-ttu-id="00789-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00789-157">Property</span></span>     | <span data-ttu-id="00789-158">型</span><span class="sxs-lookup"><span data-stu-id="00789-158">Type</span></span>   |<span data-ttu-id="00789-159">説明</span><span class="sxs-lookup"><span data-stu-id="00789-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00789-160">canEdit</span><span class="sxs-lookup"><span data-stu-id="00789-160">canEdit</span></span> |<span data-ttu-id="00789-161">ブール値</span><span class="sxs-lookup"><span data-stu-id="00789-161">Boolean</span></span> |<span data-ttu-id="00789-p107">ユーザーが予定表に書き込むことができる場合は true、それ以外の場合は false です。予定表を作成したユーザーの場合は、このプロパティは true です。予定表を共有していて、書き込みアクセスが付与されているユーザーの場合も、このプロパティは true です。</span><span class="sxs-lookup"><span data-stu-id="00789-p107">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="00789-165">canShare</span><span class="sxs-lookup"><span data-stu-id="00789-165">canShare</span></span> |<span data-ttu-id="00789-166">ブール値</span><span class="sxs-lookup"><span data-stu-id="00789-166">Boolean</span></span> |<span data-ttu-id="00789-p108">ユーザーに予定表を共有するためのアクセス許可がある場合は true、それ以外の場合は false です。予定表を作成したユーザーのみがその予定表を共有できます。</span><span class="sxs-lookup"><span data-stu-id="00789-p108">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="00789-169">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="00789-169">canViewPrivateItems</span></span> |<span data-ttu-id="00789-170">ブール値</span><span class="sxs-lookup"><span data-stu-id="00789-170">Boolean</span></span> |<span data-ttu-id="00789-171">ユーザーがプライベートとしてマークされている予定表アイテムを読み取れることができる場合は true、それ以外の場合は false です。</span><span class="sxs-lookup"><span data-stu-id="00789-171">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="00789-172">changeKey</span><span class="sxs-lookup"><span data-stu-id="00789-172">changeKey</span></span>|<span data-ttu-id="00789-173">文字列</span><span class="sxs-lookup"><span data-stu-id="00789-173">String</span></span>|<span data-ttu-id="00789-p109">予定表オブジェクトのバージョンを識別します。予定表を変更するたびに changeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="00789-p109">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="00789-178">color</span><span class="sxs-lookup"><span data-stu-id="00789-178">color</span></span>|<span data-ttu-id="00789-179">calendarColor</span><span class="sxs-lookup"><span data-stu-id="00789-179">calendarColor</span></span>|<span data-ttu-id="00789-p110">UI で予定表を他の予定表から区別するための配色テーマを指定します。プロパティ値は次のとおりです。薄い青=0、薄い緑=1、薄いオレンジ=2、薄い灰色=3、薄い黄=4、薄い青緑=5、薄いピンク=6、薄い茶色=7、薄い赤=8、最大色=9、自動=-1</span><span class="sxs-lookup"><span data-stu-id="00789-p110">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="00789-182">id</span><span class="sxs-lookup"><span data-stu-id="00789-182">id</span></span>|<span data-ttu-id="00789-183">文字列</span><span class="sxs-lookup"><span data-stu-id="00789-183">String</span></span>|<span data-ttu-id="00789-p111">グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="00789-p111">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="00789-186">name</span><span class="sxs-lookup"><span data-stu-id="00789-186">name</span></span>|<span data-ttu-id="00789-187">String</span><span class="sxs-lookup"><span data-stu-id="00789-187">String</span></span>|<span data-ttu-id="00789-188">予定表の名前。</span><span class="sxs-lookup"><span data-stu-id="00789-188">The calendar name.</span></span>|
|<span data-ttu-id="00789-189">owner</span><span class="sxs-lookup"><span data-stu-id="00789-189">owner</span></span> |[<span data-ttu-id="00789-190">emailAddress</span><span class="sxs-lookup"><span data-stu-id="00789-190">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="00789-p112">設定すると、これは予定表を作成または追加したユーザーを表します。ユーザーが作成または追加した予定表の場合、**owner** プロパティがユーザーに設定されます。ユーザーと共有されている予定表の場合は、**owner** プロパティがその予定表をユーザーと共有した人に設定されます。</span><span class="sxs-lookup"><span data-stu-id="00789-p112">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="00789-194">関係</span><span class="sxs-lookup"><span data-stu-id="00789-194">Relationships</span></span>
| <span data-ttu-id="00789-195">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="00789-195">Relationship</span></span> | <span data-ttu-id="00789-196">型</span><span class="sxs-lookup"><span data-stu-id="00789-196">Type</span></span>   |<span data-ttu-id="00789-197">説明</span><span class="sxs-lookup"><span data-stu-id="00789-197">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00789-198">calendarView</span><span class="sxs-lookup"><span data-stu-id="00789-198">calendarView</span></span>|<span data-ttu-id="00789-199">[Event](event.md) collection</span><span class="sxs-lookup"><span data-stu-id="00789-199">[Event](event.md) collection</span></span>|<span data-ttu-id="00789-p113">予定表のカレンダー ビュー。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="00789-p113">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="00789-203">events</span><span class="sxs-lookup"><span data-stu-id="00789-203">events</span></span>|<span data-ttu-id="00789-204">[Event](event.md) collection</span><span class="sxs-lookup"><span data-stu-id="00789-204">[Event](event.md) collection</span></span>|<span data-ttu-id="00789-p114">予定表内のイベント。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="00789-p114">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="00789-208">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="00789-208">multiValueExtendedProperties</span></span>|<span data-ttu-id="00789-209">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="00789-209">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="00789-p115">予定表に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="00789-p115">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="00789-213">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="00789-213">singleValueExtendedProperties</span></span>|<span data-ttu-id="00789-214">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="00789-214">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="00789-p116">予定表に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="00789-p116">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00789-218">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00789-218">JSON representation</span></span>

<span data-ttu-id="00789-219">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="00789-219">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
