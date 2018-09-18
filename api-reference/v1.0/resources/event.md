# <a name="event-resource-type"></a><span data-ttu-id="25033-101">イベント リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25033-101">event resource type</span></span>

<span data-ttu-id="25033-102">予定表内のイベントです。</span><span class="sxs-lookup"><span data-stu-id="25033-102">An event in a calendar.</span></span>

<span data-ttu-id="25033-103">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="25033-103">This resource supports:</span></span>

- <span data-ttu-id="25033-104">[拡張機能](../../../concepts/extensibility_overview.md)を使用して、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="25033-104">Adding your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="25033-105">[通知の変更](../../../concepts/webhooks.md)にサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="25033-105">Subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>
- <span data-ttu-id="25033-106">[デルタ](../api/event_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="25033-106">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/event_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="25033-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="25033-107">Methods</span></span>

| <span data-ttu-id="25033-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="25033-108">Method</span></span>       | <span data-ttu-id="25033-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="25033-109">Return Type</span></span>  |<span data-ttu-id="25033-110">説明</span><span class="sxs-lookup"><span data-stu-id="25033-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25033-111">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="25033-111">List events</span></span>](../api/user_list_events.md)|<span data-ttu-id="25033-112">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-112">[event](event.md) collection</span></span> |<span data-ttu-id="25033-p101">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="25033-p101">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="25033-115">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="25033-115">Create event</span></span>](../api/user_post_events.md) |[<span data-ttu-id="25033-116">event</span><span class="sxs-lookup"><span data-stu-id="25033-116">event</span></span>](event.md)| <span data-ttu-id="25033-117">インスタンス コレクションへの投稿により、新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="25033-117">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="25033-118">イベントの取得</span><span class="sxs-lookup"><span data-stu-id="25033-118">Get event</span></span>](../api/event_get.md) | [<span data-ttu-id="25033-119">event</span><span class="sxs-lookup"><span data-stu-id="25033-119">event</span></span>](event.md) |<span data-ttu-id="25033-120">event オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="25033-120">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="25033-121">更新する</span><span class="sxs-lookup"><span data-stu-id="25033-121">Update</span></span>](../api/event_update.md) | [<span data-ttu-id="25033-122">event</span><span class="sxs-lookup"><span data-stu-id="25033-122">event</span></span>](event.md) |<span data-ttu-id="25033-123">イベント オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="25033-123">Update event object.</span></span> |
|[<span data-ttu-id="25033-124">削除</span><span class="sxs-lookup"><span data-stu-id="25033-124">Delete</span></span>](../api/event_delete.md) | <span data-ttu-id="25033-125">なし</span><span class="sxs-lookup"><span data-stu-id="25033-125">None</span></span> |<span data-ttu-id="25033-126">イベント オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="25033-126">Delete event object.</span></span> |
|[<span data-ttu-id="25033-127">承諾</span><span class="sxs-lookup"><span data-stu-id="25033-127">accept</span></span>](../api/event_accept.md)|<span data-ttu-id="25033-128">なし</span><span class="sxs-lookup"><span data-stu-id="25033-128">None</span></span>|<span data-ttu-id="25033-129">指定したイベントを承諾します。</span><span class="sxs-lookup"><span data-stu-id="25033-129">Accept the specified event.</span></span>|
|[<span data-ttu-id="25033-130">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="25033-130">tentativelyAccept</span></span>](../api/event_tentativelyaccept.md)|<span data-ttu-id="25033-131">なし</span><span class="sxs-lookup"><span data-stu-id="25033-131">None</span></span>|<span data-ttu-id="25033-132">指定したイベントを仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="25033-132">Tentatively accept the specified event.</span></span>|
|[<span data-ttu-id="25033-133">辞退</span><span class="sxs-lookup"><span data-stu-id="25033-133">decline</span></span>](../api/event_decline.md)|<span data-ttu-id="25033-134">なし</span><span class="sxs-lookup"><span data-stu-id="25033-134">None</span></span>|<span data-ttu-id="25033-135">指定したイベントへの招待を辞退します。</span><span class="sxs-lookup"><span data-stu-id="25033-135">Decline invitation to the specified event.</span></span>|
|[<span data-ttu-id="25033-136">delta</span><span class="sxs-lookup"><span data-stu-id="25033-136">delta</span></span>](../api/event_delta.md)|<span data-ttu-id="25033-137">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-137">[event](event.md) collection</span></span>|<span data-ttu-id="25033-138">ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。</span><span class="sxs-lookup"><span data-stu-id="25033-138">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="25033-139">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="25033-139">dismissReminder</span></span>](../api/event_dismissreminder.md)|<span data-ttu-id="25033-140">なし</span><span class="sxs-lookup"><span data-stu-id="25033-140">None</span></span>|<span data-ttu-id="25033-141">指定したイベントのアラームを無視します。</span><span class="sxs-lookup"><span data-stu-id="25033-141">Dismiss the reminder for the specified event.</span></span>|
|[<span data-ttu-id="25033-142">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="25033-142">snoozeReminder</span></span>](../api/event_snoozereminder.md)|<span data-ttu-id="25033-143">なし</span><span class="sxs-lookup"><span data-stu-id="25033-143">None</span></span>|<span data-ttu-id="25033-144">指定したイベントのアラームを再通知します。</span><span class="sxs-lookup"><span data-stu-id="25033-144">Snooze the reminder for the specified event.</span></span>|
|[<span data-ttu-id="25033-145">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="25033-145">List instances</span></span>](../api/event_list_instances.md) |<span data-ttu-id="25033-146">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-146">[event](event.md) collection</span></span>| <span data-ttu-id="25033-p102">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが `SeriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="25033-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="25033-149">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="25033-149">**Attachments**</span></span>| | |
|[<span data-ttu-id="25033-150">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="25033-150">List attachments</span></span>](../api/event_list_attachments.md) |<span data-ttu-id="25033-151">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-151">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="25033-152">イベントのすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="25033-152">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="25033-153">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="25033-153">Add attachment</span></span>](../api/event_post_attachments.md) |[<span data-ttu-id="25033-154">attachment</span><span class="sxs-lookup"><span data-stu-id="25033-154">attachment</span></span>](attachment.md)| <span data-ttu-id="25033-155">添付ファイル コレクションへの投稿により、イベントに新しい添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="25033-155">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="25033-156">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="25033-156">**Open extensions**</span></span>| | |
|[<span data-ttu-id="25033-157">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="25033-157">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="25033-158">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="25033-158">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="25033-159">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="25033-159">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="25033-160">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="25033-160">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="25033-161">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-161">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="25033-162">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを 1 つまたは複数取得します。</span><span class="sxs-lookup"><span data-stu-id="25033-162">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="25033-163">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="25033-163">**Extended properties**</span></span>| | |
|[<span data-ttu-id="25033-164">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="25033-164">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="25033-165">event</span><span class="sxs-lookup"><span data-stu-id="25033-165">event</span></span>](event.md)  |<span data-ttu-id="25033-166">新規または既存のイベントに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="25033-166">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="25033-167">単一値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="25033-167">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="25033-168">event</span><span class="sxs-lookup"><span data-stu-id="25033-168">event</span></span>](event.md) | <span data-ttu-id="25033-169">または `$filter` を使用して、単一値の拡張プロパティを含むイベントを取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="25033-169">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="25033-170">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="25033-170">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="25033-171">event</span><span class="sxs-lookup"><span data-stu-id="25033-171">event</span></span>](event.md) | <span data-ttu-id="25033-172">新規または既存のイベントに、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="25033-172">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="25033-173">複数値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="25033-173">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="25033-174">event</span><span class="sxs-lookup"><span data-stu-id="25033-174">event</span></span>](event.md) | <span data-ttu-id="25033-175">を使用して、複数値の拡張プロパティを含むイベントを取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="25033-175">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="25033-176">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25033-176">Properties</span></span>
| <span data-ttu-id="25033-177">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25033-177">Property</span></span>     | <span data-ttu-id="25033-178">型</span><span class="sxs-lookup"><span data-stu-id="25033-178">Type</span></span>   |<span data-ttu-id="25033-179">説明</span><span class="sxs-lookup"><span data-stu-id="25033-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25033-180">attendees</span><span class="sxs-lookup"><span data-stu-id="25033-180">attendees</span></span>|<span data-ttu-id="25033-181">[attendee](attendee.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-181">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="25033-182">イベントの出席者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="25033-182">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="25033-183">本文</span><span class="sxs-lookup"><span data-stu-id="25033-183">body</span></span>|[<span data-ttu-id="25033-184">itemBody</span><span class="sxs-lookup"><span data-stu-id="25033-184">itemBody</span></span>](itembody.md)|<span data-ttu-id="25033-p103">イベントに関連付けられたメッセージの本文。HTML 形式またはテキスト形式にできます。</span><span class="sxs-lookup"><span data-stu-id="25033-p103">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="25033-187">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="25033-187">bodyPreview</span></span>|<span data-ttu-id="25033-188">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-188">String</span></span>|<span data-ttu-id="25033-p104">イベントに関連付けられたメッセージのプレビュー。テキスト形式です。</span><span class="sxs-lookup"><span data-stu-id="25033-p104">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="25033-191">categories</span><span class="sxs-lookup"><span data-stu-id="25033-191">categories</span></span>|<span data-ttu-id="25033-192">String コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-192">String collection</span></span>|<span data-ttu-id="25033-193">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="25033-193">The categories associated with the event.</span></span>|
|<span data-ttu-id="25033-194">changeKey</span><span class="sxs-lookup"><span data-stu-id="25033-194">changeKey</span></span>|<span data-ttu-id="25033-195">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-195">String</span></span>|<span data-ttu-id="25033-p105">イベント オブジェクトのバージョンを識別します。イベントを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="25033-p105">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="25033-199">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25033-199">createdDateTime</span></span>|<span data-ttu-id="25033-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25033-200">DateTimeOffset</span></span>|<span data-ttu-id="25033-p106">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="25033-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="25033-203">end</span><span class="sxs-lookup"><span data-stu-id="25033-203">end</span></span>|[<span data-ttu-id="25033-204">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="25033-204">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="25033-205">イベントが終了する日付、時刻、タイムゾーン</span><span class="sxs-lookup"><span data-stu-id="25033-205">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="25033-206">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="25033-206">hasAttachments</span></span>|<span data-ttu-id="25033-207">ブール値</span><span class="sxs-lookup"><span data-stu-id="25033-207">Boolean</span></span>|<span data-ttu-id="25033-208">イベントに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="25033-208">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="25033-209">iCalUId</span><span class="sxs-lookup"><span data-stu-id="25033-209">iCalUId</span></span>|<span data-ttu-id="25033-210">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-210">String</span></span>|<span data-ttu-id="25033-211">複数の予定表で 1 つのイベントのすべてのインスタンスによって共有される一意識別子。</span><span class="sxs-lookup"><span data-stu-id="25033-211">A unique identifier that is shared by all instances of an event across different calendars.</span></span>|
|<span data-ttu-id="25033-212">ID</span><span class="sxs-lookup"><span data-stu-id="25033-212">id</span></span>|<span data-ttu-id="25033-213">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-213">String</span></span>| <span data-ttu-id="25033-214">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25033-214">Read-only.</span></span>|
|<span data-ttu-id="25033-215">重要性</span><span class="sxs-lookup"><span data-stu-id="25033-215">importance</span></span>|<span data-ttu-id="25033-216">重要性</span><span class="sxs-lookup"><span data-stu-id="25033-216">importance</span></span>|<span data-ttu-id="25033-217">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="25033-217">The importance of the event.</span></span> <span data-ttu-id="25033-218">使用可能な値は`low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="25033-218">The possible values are `low`, `normal`, or `high`.</span></span>|
|<span data-ttu-id="25033-219">isAllDay</span><span class="sxs-lookup"><span data-stu-id="25033-219">isAllDay</span></span>|<span data-ttu-id="25033-220">ブール値</span><span class="sxs-lookup"><span data-stu-id="25033-220">Boolean</span></span>|<span data-ttu-id="25033-221">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="25033-221">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="25033-222">isCancelled</span><span class="sxs-lookup"><span data-stu-id="25033-222">isCancelled</span></span>|<span data-ttu-id="25033-223">ブール値</span><span class="sxs-lookup"><span data-stu-id="25033-223">Boolean</span></span>|<span data-ttu-id="25033-224">イベントがキャンセルされた場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="25033-224">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="25033-225">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="25033-225">isOrganizer</span></span>|<span data-ttu-id="25033-226">ブール値</span><span class="sxs-lookup"><span data-stu-id="25033-226">Boolean</span></span>|<span data-ttu-id="25033-227">メッセージの送信者が開催者でもある場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="25033-227">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="25033-228">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="25033-228">isReminderOn</span></span>|<span data-ttu-id="25033-229">ブール値</span><span class="sxs-lookup"><span data-stu-id="25033-229">Boolean</span></span>|<span data-ttu-id="25033-230">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="25033-230">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="25033-231">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25033-231">lastModifiedDateTime</span></span>|<span data-ttu-id="25033-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25033-232">DateTimeOffset</span></span>|<span data-ttu-id="25033-p108">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="25033-p108">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="25033-235">location</span><span class="sxs-lookup"><span data-stu-id="25033-235">location</span></span>|[<span data-ttu-id="25033-236">location</span><span class="sxs-lookup"><span data-stu-id="25033-236">location</span></span>](location.md)|<span data-ttu-id="25033-237">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="25033-237">The location of the event.</span></span>|
|<span data-ttu-id="25033-238">位置</span><span class="sxs-lookup"><span data-stu-id="25033-238">locations</span></span>|<span data-ttu-id="25033-239">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-239">[location](location.md) collection</span></span>|<span data-ttu-id="25033-240">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="25033-240">The locations where the event is held or attended from.</span></span> <span data-ttu-id="25033-241">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="25033-241">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="25033-242">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="25033-242">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="25033-243">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="25033-243">onlineMeetingUrl</span></span>|<span data-ttu-id="25033-244">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-244">String</span></span>|<span data-ttu-id="25033-245">オンライン会議の URL。</span><span class="sxs-lookup"><span data-stu-id="25033-245">A URL for an online meeting.</span></span> <span data-ttu-id="25033-246">会議の開催者が Skype 会議などのオンライン会議としてイベントを指定するときにのみ、プロパティが設定されます。</span><span class="sxs-lookup"><span data-stu-id="25033-246">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="25033-247">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25033-247">Read-only.</span></span>|
|<span data-ttu-id="25033-248">organizer</span><span class="sxs-lookup"><span data-stu-id="25033-248">organizer</span></span>|[<span data-ttu-id="25033-249">recipient</span><span class="sxs-lookup"><span data-stu-id="25033-249">recipient</span></span>](recipient.md)|<span data-ttu-id="25033-250">イベントの開催者。</span><span class="sxs-lookup"><span data-stu-id="25033-250">The organizer of the event.</span></span>|
|<span data-ttu-id="25033-251">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="25033-251">originalEndTimeZone</span></span>|<span data-ttu-id="25033-252">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-252">String</span></span>|<span data-ttu-id="25033-253">イベントの作成時に設定された終了タイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="25033-253">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="25033-254">値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="25033-254">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="25033-255">originalStart</span><span class="sxs-lookup"><span data-stu-id="25033-255">originalStart</span></span>|<span data-ttu-id="25033-256">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25033-256">DateTimeOffset</span></span>|<span data-ttu-id="25033-p112">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="25033-p112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="25033-259">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="25033-259">originalStartTimeZone</span></span>|<span data-ttu-id="25033-260">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-260">String</span></span>|<span data-ttu-id="25033-p113">イベントが作成されたときに設定された開始タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="25033-p113">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="25033-263">recurrence</span><span class="sxs-lookup"><span data-stu-id="25033-263">recurrence</span></span>|[<span data-ttu-id="25033-264">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="25033-264">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="25033-265">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="25033-265">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="25033-266">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="25033-266">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="25033-267">Int32</span><span class="sxs-lookup"><span data-stu-id="25033-267">Int32</span></span>|<span data-ttu-id="25033-268">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="25033-268">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="25033-269">responseRequested</span><span class="sxs-lookup"><span data-stu-id="25033-269">responseRequested</span></span>|<span data-ttu-id="25033-270">ブール値</span><span class="sxs-lookup"><span data-stu-id="25033-270">Boolean</span></span>|<span data-ttu-id="25033-271">イベントが承諾または辞退されたときに、送信者が応答を希望する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="25033-271">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="25033-272">responseStatus</span><span class="sxs-lookup"><span data-stu-id="25033-272">responseStatus</span></span>|[<span data-ttu-id="25033-273">responseStatus</span><span class="sxs-lookup"><span data-stu-id="25033-273">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="25033-274">イベント メッセージへの応答で送信される応答のタイプを識別します。</span><span class="sxs-lookup"><span data-stu-id="25033-274">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="25033-275">秘密度</span><span class="sxs-lookup"><span data-stu-id="25033-275">sensitivity</span></span>|<span data-ttu-id="25033-276">秘密度</span><span class="sxs-lookup"><span data-stu-id="25033-276">sensitivity</span></span>| <span data-ttu-id="25033-277">使用可能な値は`normal`、`personal`、`private`、`confidential` です。</span><span class="sxs-lookup"><span data-stu-id="25033-277">The possible values are  `normal`,  `personal`,  `private`, or  `confidential`.</span></span>|
|<span data-ttu-id="25033-278">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="25033-278">seriesMasterId</span></span>|<span data-ttu-id="25033-279">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-279">String</span></span>|<span data-ttu-id="25033-280">このイベントが定期的なイベントの一部である場合、定期的な一連のイベントのマスター アイテムの ID。</span><span class="sxs-lookup"><span data-stu-id="25033-280">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="25033-281">showAs</span><span class="sxs-lookup"><span data-stu-id="25033-281">showAs</span></span>|<span data-ttu-id="25033-282">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="25033-282">FreeBusyStatus</span></span>|<span data-ttu-id="25033-283">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="25033-283">The status to show.</span></span> <span data-ttu-id="25033-284">使用可能な値は `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown` です。</span><span class="sxs-lookup"><span data-stu-id="25033-284">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , , , , , .</span></span>|
|<span data-ttu-id="25033-285">start</span><span class="sxs-lookup"><span data-stu-id="25033-285">start</span></span>|[<span data-ttu-id="25033-286">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="25033-286">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="25033-287">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="25033-287">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="25033-288">subject</span><span class="sxs-lookup"><span data-stu-id="25033-288">subject</span></span>|<span data-ttu-id="25033-289">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-289">String</span></span>|<span data-ttu-id="25033-290">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="25033-290">The text of the event's subject line.</span></span>|
|<span data-ttu-id="25033-291">型</span><span class="sxs-lookup"><span data-stu-id="25033-291">type</span></span>|<span data-ttu-id="25033-292">eventType</span><span class="sxs-lookup"><span data-stu-id="25033-292">eventType</span></span>|<span data-ttu-id="25033-293">イベントの種類。</span><span class="sxs-lookup"><span data-stu-id="25033-293">The event type.</span></span> <span data-ttu-id="25033-294">使用可能な値は`singleInstance`、`occurrence`、`exception`、`seriesMaster` です。</span><span class="sxs-lookup"><span data-stu-id="25033-294">The possible values are  `singleInstance`,  `occurrence`,  `exception`, or  `seriesMaster`.</span></span> <span data-ttu-id="25033-295">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25033-295">Read-only.</span></span>|
|<span data-ttu-id="25033-296">webLink</span><span class="sxs-lookup"><span data-stu-id="25033-296">webLink</span></span>|<span data-ttu-id="25033-297">文字列</span><span class="sxs-lookup"><span data-stu-id="25033-297">String</span></span>|<span data-ttu-id="25033-298">Outlook Web App でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="25033-298">The URL to open the event in Outlook Web App.</span></span><br/><br/><span data-ttu-id="25033-p116">Outlook Web App のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="25033-p116">The event will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="25033-301">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="25033-301">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25033-302">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25033-302">Relationships</span></span>
| <span data-ttu-id="25033-303">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25033-303">Relationship</span></span> | <span data-ttu-id="25033-304">型</span><span class="sxs-lookup"><span data-stu-id="25033-304">Type</span></span>   |<span data-ttu-id="25033-305">説明</span><span class="sxs-lookup"><span data-stu-id="25033-305">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25033-306">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="25033-306">attachments</span></span>|<span data-ttu-id="25033-307">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-307">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="25033-p117">イベントの [fileAttachment](fileAttachment.md) 添付ファイルと [itemAttachment](itemAttachment.md) 添付ファイルのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="25033-p117">The collection of [fileAttachment](fileAttachment.md) and [itemAttachment](itemAttachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="25033-312">calendar</span><span class="sxs-lookup"><span data-stu-id="25033-312">calendar</span></span>|[<span data-ttu-id="25033-313">calendar</span><span class="sxs-lookup"><span data-stu-id="25033-313">calendar</span></span>](calendar.md)|<span data-ttu-id="25033-p118">イベントを含む予定表。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="25033-p118">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="25033-317">extensions</span><span class="sxs-lookup"><span data-stu-id="25033-317">extensions</span></span>|<span data-ttu-id="25033-318">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-318">[Extension](extension.md) collection</span></span>|<span data-ttu-id="25033-p119">イベントに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="25033-p119">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="25033-322">インスタンス</span><span class="sxs-lookup"><span data-stu-id="25033-322">instances</span></span>|<span data-ttu-id="25033-323">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-323">[event](event.md) collection</span></span>|<span data-ttu-id="25033-p120">イベントのインスタンス。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="25033-p120">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="25033-328">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="25033-328">multiValueExtendedProperties</span></span>|<span data-ttu-id="25033-329">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-329">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="25033-p121">イベントに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="25033-p121">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="25033-333">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="25033-333">singleValueExtendedProperties</span></span>|<span data-ttu-id="25033-334">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="25033-334">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="25033-p122">イベントに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="25033-p122">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25033-338">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25033-338">JSON representation</span></span>

<span data-ttu-id="25033-339">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="25033-339">Here is a JSON representation of the resource</span></span>

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


## <a name="see-also"></a><span data-ttu-id="25033-340">関連項目</span><span class="sxs-lookup"><span data-stu-id="25033-340">See also</span></span>

- [<span data-ttu-id="25033-341">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="25033-341">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="25033-342">フォルダー内のイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="25033-342">Get incremental changes to events in a folder</span></span>](../../../concepts/delta_query_events.md)
- [<span data-ttu-id="25033-343">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="25033-343">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="25033-344">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="25033-344">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="25033-345">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="25033-345">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
