# <a name="event-resource-type"></a><span data-ttu-id="e92bf-101">イベント リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e92bf-101">event resource type</span></span>

<span data-ttu-id="e92bf-102">予定表内のイベントです。</span><span class="sxs-lookup"><span data-stu-id="e92bf-102">An event in a calendar.</span></span>

<span data-ttu-id="e92bf-103">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e92bf-103">This resource supports:</span></span>

- <span data-ttu-id="e92bf-104">[拡張機能](../../../concepts/extensibility_overview.md)として、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-104">Adding your own data to custom properties as [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="e92bf-105">[変更通知](../../../concepts/webhooks.md)にサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="e92bf-105">Subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>
- <span data-ttu-id="e92bf-106">[デルタ](../api/event_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-106">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/event_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="e92bf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e92bf-107">Methods</span></span>

| <span data-ttu-id="e92bf-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e92bf-108">Method</span></span>       | <span data-ttu-id="e92bf-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e92bf-109">Return Type</span></span>  |<span data-ttu-id="e92bf-110">説明</span><span class="sxs-lookup"><span data-stu-id="e92bf-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e92bf-111">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e92bf-111">List events</span></span>](../api/user_list_events.md)|<span data-ttu-id="e92bf-112">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-112">[event](event.md) collection</span></span> |<span data-ttu-id="e92bf-p101">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p101">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="e92bf-115">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="e92bf-115">Create event</span></span>](../api/user_post_events.md) |[<span data-ttu-id="e92bf-116">event</span><span class="sxs-lookup"><span data-stu-id="e92bf-116">event</span></span>](event.md)| <span data-ttu-id="e92bf-117">インスタンス コレクションへの投稿により、新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-117">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="e92bf-118">イベントの取得</span><span class="sxs-lookup"><span data-stu-id="e92bf-118">Get event</span></span>](../api/event_get.md) | [<span data-ttu-id="e92bf-119">event</span><span class="sxs-lookup"><span data-stu-id="e92bf-119">event</span></span>](event.md) |<span data-ttu-id="e92bf-120">event オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e92bf-120">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="e92bf-121">更新する</span><span class="sxs-lookup"><span data-stu-id="e92bf-121">Update</span></span>](../api/event_update.md) | [<span data-ttu-id="e92bf-122">event</span><span class="sxs-lookup"><span data-stu-id="e92bf-122">event</span></span>](event.md) |<span data-ttu-id="e92bf-123">イベント オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-123">Update event object.</span></span> |
|[<span data-ttu-id="e92bf-124">削除</span><span class="sxs-lookup"><span data-stu-id="e92bf-124">Delete</span></span>](../api/event_delete.md) | <span data-ttu-id="e92bf-125">なし</span><span class="sxs-lookup"><span data-stu-id="e92bf-125">None</span></span> |<span data-ttu-id="e92bf-126">イベント オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-126">Delete event object.</span></span> |
|[<span data-ttu-id="e92bf-127">承諾</span><span class="sxs-lookup"><span data-stu-id="e92bf-127">accept</span></span>](../api/event_accept.md)|<span data-ttu-id="e92bf-128">なし</span><span class="sxs-lookup"><span data-stu-id="e92bf-128">None</span></span>|<span data-ttu-id="e92bf-129">指定したイベントを承諾します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-129">Accept the specified event.</span></span>|
|[<span data-ttu-id="e92bf-130">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="e92bf-130">tentativelyAccept</span></span>](../api/event_tentativelyaccept.md)|<span data-ttu-id="e92bf-131">なし</span><span class="sxs-lookup"><span data-stu-id="e92bf-131">None</span></span>|<span data-ttu-id="e92bf-132">指定したイベントを仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-132">Tentatively accept the specified event.</span></span>|
|[<span data-ttu-id="e92bf-133">辞退</span><span class="sxs-lookup"><span data-stu-id="e92bf-133">decline</span></span>](../api/event_decline.md)|<span data-ttu-id="e92bf-134">なし</span><span class="sxs-lookup"><span data-stu-id="e92bf-134">None</span></span>|<span data-ttu-id="e92bf-135">指定したイベントへの招待を辞退します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-135">Decline invitation to the specified event.</span></span>|
|[<span data-ttu-id="e92bf-136">delta</span><span class="sxs-lookup"><span data-stu-id="e92bf-136">delta</span></span>](../api/event_delta.md)|<span data-ttu-id="e92bf-137">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-137">[event](event.md) collection</span></span>|<span data-ttu-id="e92bf-138">ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-138">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="e92bf-139">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="e92bf-139">dismissReminder</span></span>](../api/event_dismissreminder.md)|<span data-ttu-id="e92bf-140">なし</span><span class="sxs-lookup"><span data-stu-id="e92bf-140">None</span></span>|<span data-ttu-id="e92bf-141">指定したイベントのアラームを無視します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-141">Dismiss the reminder for the specified event.</span></span>|
|[<span data-ttu-id="e92bf-142">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="e92bf-142">snoozeReminder</span></span>](../api/event_snoozereminder.md)|<span data-ttu-id="e92bf-143">なし</span><span class="sxs-lookup"><span data-stu-id="e92bf-143">None</span></span>|<span data-ttu-id="e92bf-144">指定したイベントのアラームを再通知します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-144">Snooze the reminder for the specified event.</span></span>|
|[<span data-ttu-id="e92bf-145">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="e92bf-145">List instances</span></span>](../api/event_list_instances.md) |<span data-ttu-id="e92bf-146">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-146">[event](event.md) collection</span></span>| <span data-ttu-id="e92bf-p102">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが `SeriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="e92bf-149">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="e92bf-149">**Attachments**</span></span>| | |
|[<span data-ttu-id="e92bf-150">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e92bf-150">List attachments</span></span>](../api/event_list_attachments.md) |<span data-ttu-id="e92bf-151">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-151">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="e92bf-152">イベントのすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-152">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="e92bf-153">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="e92bf-153">Add attachment</span></span>](../api/event_post_attachments.md) |[<span data-ttu-id="e92bf-154">attachment</span><span class="sxs-lookup"><span data-stu-id="e92bf-154">attachment</span></span>](attachment.md)| <span data-ttu-id="e92bf-155">添付ファイル コレクションへの投稿により、イベントに新しい添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-155">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="e92bf-156">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="e92bf-156">**Open extensions**</span></span>| | |
|[<span data-ttu-id="e92bf-157">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="e92bf-157">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="e92bf-158">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e92bf-158">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="e92bf-159">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-159">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="e92bf-160">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="e92bf-160">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="e92bf-161">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-161">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="e92bf-162">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを 1 つまたは複数取得します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-162">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="e92bf-163">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="e92bf-163">**Extended properties**</span></span>| | |
|[<span data-ttu-id="e92bf-164">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="e92bf-164">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="e92bf-165">event</span><span class="sxs-lookup"><span data-stu-id="e92bf-165">event</span></span>](event.md)  |<span data-ttu-id="e92bf-166">新規または既存のイベントに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-166">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="e92bf-167">単一値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="e92bf-167">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="e92bf-168">event</span><span class="sxs-lookup"><span data-stu-id="e92bf-168">event</span></span>](event.md) | <span data-ttu-id="e92bf-169">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含むイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-169">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="e92bf-170">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="e92bf-170">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="e92bf-171">event</span><span class="sxs-lookup"><span data-stu-id="e92bf-171">event</span></span>](event.md) | <span data-ttu-id="e92bf-172">新規または既存のイベントに、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-172">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="e92bf-173">複数値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="e92bf-173">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="e92bf-174">event</span><span class="sxs-lookup"><span data-stu-id="e92bf-174">event</span></span>](event.md) | <span data-ttu-id="e92bf-175">`$expand` を使用して、複数値の拡張プロパティを含むイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-175">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="e92bf-176">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e92bf-176">Properties</span></span>
| <span data-ttu-id="e92bf-177">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e92bf-177">Property</span></span>     | <span data-ttu-id="e92bf-178">型</span><span class="sxs-lookup"><span data-stu-id="e92bf-178">Type</span></span>   |<span data-ttu-id="e92bf-179">説明</span><span class="sxs-lookup"><span data-stu-id="e92bf-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e92bf-180">attendees</span><span class="sxs-lookup"><span data-stu-id="e92bf-180">attendees</span></span>|<span data-ttu-id="e92bf-181">[attendee](attendee.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-181">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="e92bf-182">イベントの出席者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="e92bf-182">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="e92bf-183">body</span><span class="sxs-lookup"><span data-stu-id="e92bf-183">body</span></span>|[<span data-ttu-id="e92bf-184">itemBody</span><span class="sxs-lookup"><span data-stu-id="e92bf-184">itemBody</span></span>](itembody.md)|<span data-ttu-id="e92bf-p103">イベントに関連付けられたメッセージの本文。HTML 形式またはテキスト形式にできます。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p103">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="e92bf-187">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="e92bf-187">bodyPreview</span></span>|<span data-ttu-id="e92bf-188">String</span><span class="sxs-lookup"><span data-stu-id="e92bf-188">String</span></span>|<span data-ttu-id="e92bf-p104">イベントに関連付けられたメッセージのプレビュー。テキスト形式です。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p104">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="e92bf-191">categories</span><span class="sxs-lookup"><span data-stu-id="e92bf-191">categories</span></span>|<span data-ttu-id="e92bf-192">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-192">String collection</span></span>|<span data-ttu-id="e92bf-193">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="e92bf-193">The categories associated with the event.</span></span>|
|<span data-ttu-id="e92bf-194">changeKey</span><span class="sxs-lookup"><span data-stu-id="e92bf-194">changeKey</span></span>|<span data-ttu-id="e92bf-195">文字列</span><span class="sxs-lookup"><span data-stu-id="e92bf-195">String</span></span>|<span data-ttu-id="e92bf-p105">イベント オブジェクトのバージョンを識別します。イベントを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p105">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="e92bf-199">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e92bf-199">createdDateTime</span></span>|<span data-ttu-id="e92bf-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e92bf-200">DateTimeOffset</span></span>|<span data-ttu-id="e92bf-p106">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e92bf-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e92bf-203">end</span><span class="sxs-lookup"><span data-stu-id="e92bf-203">end</span></span>|[<span data-ttu-id="e92bf-204">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e92bf-204">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e92bf-205">イベントが終了する日付、時刻、タイムゾーン</span><span class="sxs-lookup"><span data-stu-id="e92bf-205">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="e92bf-206">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="e92bf-206">hasAttachments</span></span>|<span data-ttu-id="e92bf-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92bf-207">Boolean</span></span>|<span data-ttu-id="e92bf-208">イベントに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-208">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="e92bf-209">iCalUId</span><span class="sxs-lookup"><span data-stu-id="e92bf-209">iCalUId</span></span>|<span data-ttu-id="e92bf-210">文字列</span><span class="sxs-lookup"><span data-stu-id="e92bf-210">String</span></span>|<span data-ttu-id="e92bf-211">複数の予定表で 1 つのイベントのすべてのインスタンスによって共有される一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e92bf-211">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="e92bf-212">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e92bf-212">Read-only.</span></span>|
|<span data-ttu-id="e92bf-213">id</span><span class="sxs-lookup"><span data-stu-id="e92bf-213">id</span></span>|<span data-ttu-id="e92bf-214">文字列</span><span class="sxs-lookup"><span data-stu-id="e92bf-214">String</span></span>| <span data-ttu-id="e92bf-215">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e92bf-215">Read-only.</span></span>|
|<span data-ttu-id="e92bf-216">importance</span><span class="sxs-lookup"><span data-stu-id="e92bf-216">importance</span></span>|<span data-ttu-id="e92bf-217">importance</span><span class="sxs-lookup"><span data-stu-id="e92bf-217">importance</span></span>|<span data-ttu-id="e92bf-218">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="e92bf-218">The importance of the event.</span></span> <span data-ttu-id="e92bf-219">可能な値: `low`、 `normal`、 `high`。</span><span class="sxs-lookup"><span data-stu-id="e92bf-219">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="e92bf-220">isAllDay</span><span class="sxs-lookup"><span data-stu-id="e92bf-220">isAllDay</span></span>|<span data-ttu-id="e92bf-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92bf-221">Boolean</span></span>|<span data-ttu-id="e92bf-222">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-222">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="e92bf-223">isCancelled</span><span class="sxs-lookup"><span data-stu-id="e92bf-223">isCancelled</span></span>|<span data-ttu-id="e92bf-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92bf-224">Boolean</span></span>|<span data-ttu-id="e92bf-225">イベントがキャンセルされた場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-225">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="e92bf-226">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="e92bf-226">isOrganizer</span></span>|<span data-ttu-id="e92bf-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92bf-227">Boolean</span></span>|<span data-ttu-id="e92bf-228">メッセージの送信者が開催者でもある場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-228">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="e92bf-229">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="e92bf-229">isReminderOn</span></span>|<span data-ttu-id="e92bf-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92bf-230">Boolean</span></span>|<span data-ttu-id="e92bf-231">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-231">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="e92bf-232">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e92bf-232">lastModifiedDateTime</span></span>|<span data-ttu-id="e92bf-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e92bf-233">DateTimeOffset</span></span>|<span data-ttu-id="e92bf-p109">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e92bf-p109">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e92bf-236">location</span><span class="sxs-lookup"><span data-stu-id="e92bf-236">location</span></span>|[<span data-ttu-id="e92bf-237">location</span><span class="sxs-lookup"><span data-stu-id="e92bf-237">location</span></span>](location.md)|<span data-ttu-id="e92bf-238">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="e92bf-238">The location of the event.</span></span>|
|<span data-ttu-id="e92bf-239">locations</span><span class="sxs-lookup"><span data-stu-id="e92bf-239">locations</span></span>|<span data-ttu-id="e92bf-240">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-240">[location](location.md) collection</span></span>|<span data-ttu-id="e92bf-241">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="e92bf-241">The locations where the event is held or attended from.</span></span> <span data-ttu-id="e92bf-242">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-242">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="e92bf-243">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="e92bf-243">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="e92bf-244">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="e92bf-244">onlineMeetingUrl</span></span>|<span data-ttu-id="e92bf-245">文字列</span><span class="sxs-lookup"><span data-stu-id="e92bf-245">String</span></span>|<span data-ttu-id="e92bf-246">オンライン会議の URL。</span><span class="sxs-lookup"><span data-stu-id="e92bf-246">A URL for an online meeting.</span></span> <span data-ttu-id="e92bf-247">会議の開催者が Skype 会議などのオンラインの会議とイベントを指定するときにのみ、プロパティが設定されています。</span><span class="sxs-lookup"><span data-stu-id="e92bf-247">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="e92bf-248">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e92bf-248">Read-only.</span></span>|
|<span data-ttu-id="e92bf-249">organizer</span><span class="sxs-lookup"><span data-stu-id="e92bf-249">organizer</span></span>|[<span data-ttu-id="e92bf-250">recipient</span><span class="sxs-lookup"><span data-stu-id="e92bf-250">recipient</span></span>](recipient.md)|<span data-ttu-id="e92bf-251">イベントの開催者。</span><span class="sxs-lookup"><span data-stu-id="e92bf-251">The organizer of the event.</span></span>|
|<span data-ttu-id="e92bf-252">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="e92bf-252">originalEndTimeZone</span></span>|<span data-ttu-id="e92bf-253">文字列</span><span class="sxs-lookup"><span data-stu-id="e92bf-253">String</span></span>|<span data-ttu-id="e92bf-254">イベントの作成時に設定された終了タイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="e92bf-254">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="e92bf-255">値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-255">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="e92bf-256">originalStart</span><span class="sxs-lookup"><span data-stu-id="e92bf-256">originalStart</span></span>|<span data-ttu-id="e92bf-257">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e92bf-257">DateTimeOffset</span></span>|<span data-ttu-id="e92bf-p113">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e92bf-p113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e92bf-260">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="e92bf-260">originalStartTimeZone</span></span>|<span data-ttu-id="e92bf-261">String</span><span class="sxs-lookup"><span data-stu-id="e92bf-261">String</span></span>|<span data-ttu-id="e92bf-p114">イベントが作成されたときに設定された開始タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p114">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="e92bf-264">recurrence</span><span class="sxs-lookup"><span data-stu-id="e92bf-264">recurrence</span></span>|[<span data-ttu-id="e92bf-265">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e92bf-265">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="e92bf-266">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="e92bf-266">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="e92bf-267">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="e92bf-267">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="e92bf-268">Int32</span><span class="sxs-lookup"><span data-stu-id="e92bf-268">Int32</span></span>|<span data-ttu-id="e92bf-269">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="e92bf-269">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="e92bf-270">responseRequested</span><span class="sxs-lookup"><span data-stu-id="e92bf-270">responseRequested</span></span>|<span data-ttu-id="e92bf-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92bf-271">Boolean</span></span>|<span data-ttu-id="e92bf-272">イベントが承諾または辞退されたときに、送信者が応答を希望する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-272">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="e92bf-273">responseStatus</span><span class="sxs-lookup"><span data-stu-id="e92bf-273">responseStatus</span></span>|[<span data-ttu-id="e92bf-274">responseStatus</span><span class="sxs-lookup"><span data-stu-id="e92bf-274">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="e92bf-275">イベント メッセージへの応答で送信される応答のタイプを識別します。</span><span class="sxs-lookup"><span data-stu-id="e92bf-275">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="e92bf-276">sensitivity</span><span class="sxs-lookup"><span data-stu-id="e92bf-276">sensitivity</span></span>|<span data-ttu-id="e92bf-277">sensitivity</span><span class="sxs-lookup"><span data-stu-id="e92bf-277">sensitivity</span></span>| <span data-ttu-id="e92bf-278">可能な値: `normal`、 `personal`、 `private`、 `confidential`。</span><span class="sxs-lookup"><span data-stu-id="e92bf-278">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="e92bf-279">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="e92bf-279">seriesMasterId</span></span>|<span data-ttu-id="e92bf-280">文字列</span><span class="sxs-lookup"><span data-stu-id="e92bf-280">String</span></span>|<span data-ttu-id="e92bf-281">項目の ID、定期的な系列マスター、このイベントが定期的な一連の一部である場合。</span><span class="sxs-lookup"><span data-stu-id="e92bf-281">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="e92bf-282">showAs</span><span class="sxs-lookup"><span data-stu-id="e92bf-282">showAs</span></span>|<span data-ttu-id="e92bf-283">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="e92bf-283">freeBusyStatus</span></span>|<span data-ttu-id="e92bf-284">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="e92bf-284">The status to show.</span></span> <span data-ttu-id="e92bf-285">可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="e92bf-285">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="e92bf-286">start</span><span class="sxs-lookup"><span data-stu-id="e92bf-286">start</span></span>|[<span data-ttu-id="e92bf-287">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e92bf-287">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e92bf-288">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="e92bf-288">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="e92bf-289">subject</span><span class="sxs-lookup"><span data-stu-id="e92bf-289">subject</span></span>|<span data-ttu-id="e92bf-290">String</span><span class="sxs-lookup"><span data-stu-id="e92bf-290">String</span></span>|<span data-ttu-id="e92bf-291">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="e92bf-291">The text of the event's subject line.</span></span>|
|<span data-ttu-id="e92bf-292">type</span><span class="sxs-lookup"><span data-stu-id="e92bf-292">type</span></span>|<span data-ttu-id="e92bf-293">eventType</span><span class="sxs-lookup"><span data-stu-id="e92bf-293">eventType</span></span>|<span data-ttu-id="e92bf-294">イベントの種類。</span><span class="sxs-lookup"><span data-stu-id="e92bf-294">The event type.</span></span> <span data-ttu-id="e92bf-295">可能な値: `singleInstance`、 `occurrence`、 `exception`、 `seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="e92bf-295">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="e92bf-296">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e92bf-296">Read-only.</span></span>|
|<span data-ttu-id="e92bf-297">webLink</span><span class="sxs-lookup"><span data-stu-id="e92bf-297">webLink</span></span>|<span data-ttu-id="e92bf-298">文字列</span><span class="sxs-lookup"><span data-stu-id="e92bf-298">String</span></span>|<span data-ttu-id="e92bf-299">Outlook Web App でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="e92bf-299">The URL to open the event in Outlook Web App.</span></span><br/><br/><span data-ttu-id="e92bf-p117">Outlook Web App のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p117">The event will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="e92bf-302">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e92bf-302">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e92bf-303">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e92bf-303">Relationships</span></span>
| <span data-ttu-id="e92bf-304">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e92bf-304">Relationship</span></span> | <span data-ttu-id="e92bf-305">型</span><span class="sxs-lookup"><span data-stu-id="e92bf-305">Type</span></span>   |<span data-ttu-id="e92bf-306">説明</span><span class="sxs-lookup"><span data-stu-id="e92bf-306">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e92bf-307">attachments</span><span class="sxs-lookup"><span data-stu-id="e92bf-307">attachments</span></span>|<span data-ttu-id="e92bf-308">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-308">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="e92bf-p118">イベントの [fileAttachment](fileAttachment.md) 添付ファイルと [itemAttachment](itemAttachment.md) 添付ファイルのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p118">The collection of [fileAttachment](fileAttachment.md) and [itemAttachment](itemAttachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e92bf-313">予定表</span><span class="sxs-lookup"><span data-stu-id="e92bf-313">calendar</span></span>|[<span data-ttu-id="e92bf-314">calendar</span><span class="sxs-lookup"><span data-stu-id="e92bf-314">calendar</span></span>](calendar.md)|<span data-ttu-id="e92bf-p119">イベントを含む予定表。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p119">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="e92bf-318">extensions</span><span class="sxs-lookup"><span data-stu-id="e92bf-318">extensions</span></span>|<span data-ttu-id="e92bf-319">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-319">[Extension](extension.md) collection</span></span>|<span data-ttu-id="e92bf-p120">イベントに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p120">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e92bf-323">インスタンス</span><span class="sxs-lookup"><span data-stu-id="e92bf-323">instances</span></span>|<span data-ttu-id="e92bf-324">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e92bf-324">[event](event.md) collection</span></span>|<span data-ttu-id="e92bf-p121">イベントのインスタンス。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p121">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e92bf-329">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e92bf-329">multiValueExtendedProperties</span></span>|<span data-ttu-id="e92bf-330">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="e92bf-330">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e92bf-p122">イベントに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p122">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e92bf-334">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e92bf-334">singleValueExtendedProperties</span></span>|<span data-ttu-id="e92bf-335">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="e92bf-335">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e92bf-p123">イベントに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e92bf-p123">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e92bf-339">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e92bf-339">JSON representation</span></span>

<span data-ttu-id="e92bf-340">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e92bf-340">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.event",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "instances",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "iCalUId": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "type": "String",
  "webLink": "string",

  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]

}

```


## <a name="see-also"></a><span data-ttu-id="e92bf-341">関連項目</span><span class="sxs-lookup"><span data-stu-id="e92bf-341">See also</span></span>

- [<span data-ttu-id="e92bf-342">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="e92bf-342">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="e92bf-343">フォルダー内のイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="e92bf-343">Get incremental changes to events in a folder</span></span>](../../../concepts/delta_query_events.md)
- [<span data-ttu-id="e92bf-344">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="e92bf-344">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e92bf-345">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="e92bf-345">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="e92bf-346">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="e92bf-346">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
