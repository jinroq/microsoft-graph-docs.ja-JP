---
title: イベント リソースの種類
description: 予定表内のイベントです。
author: angelgolfer-ms
ms.openlocfilehash: 2caa1cb51da5f9d9ae8808b574e2787fbb63da46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356596"
---
# <a name="event-resource-type"></a><span data-ttu-id="322cd-103">イベント リソースの種類</span><span class="sxs-lookup"><span data-stu-id="322cd-103">event resource type</span></span>

<span data-ttu-id="322cd-104">予定表内のイベントです。</span><span class="sxs-lookup"><span data-stu-id="322cd-104">An event in a calendar.</span></span>

<span data-ttu-id="322cd-105">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="322cd-105">This resource supports:</span></span>

- <span data-ttu-id="322cd-106">[拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="322cd-106">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="322cd-107">[変更通知](/graph/webhooks)にサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="322cd-107">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="322cd-108">[デルタ](../api/event-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="322cd-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/event-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="322cd-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="322cd-109">Methods</span></span>

| <span data-ttu-id="322cd-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="322cd-110">Method</span></span>       | <span data-ttu-id="322cd-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="322cd-111">Return Type</span></span>  |<span data-ttu-id="322cd-112">説明</span><span class="sxs-lookup"><span data-stu-id="322cd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="322cd-113">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="322cd-113">List events</span></span>](../api/user-list-events.md)|<span data-ttu-id="322cd-114">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-114">[event](event.md) collection</span></span> |<span data-ttu-id="322cd-p101">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="322cd-p101">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="322cd-117">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="322cd-117">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="322cd-118">event</span><span class="sxs-lookup"><span data-stu-id="322cd-118">event</span></span>](event.md)| <span data-ttu-id="322cd-119">インスタンス コレクションへの投稿により、新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="322cd-119">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="322cd-120">イベントの取得</span><span class="sxs-lookup"><span data-stu-id="322cd-120">Get event</span></span>](../api/event-get.md) | [<span data-ttu-id="322cd-121">event</span><span class="sxs-lookup"><span data-stu-id="322cd-121">event</span></span>](event.md) |<span data-ttu-id="322cd-122">event オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="322cd-122">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="322cd-123">更新する</span><span class="sxs-lookup"><span data-stu-id="322cd-123">Update</span></span>](../api/event-update.md) | [<span data-ttu-id="322cd-124">event</span><span class="sxs-lookup"><span data-stu-id="322cd-124">event</span></span>](event.md) |<span data-ttu-id="322cd-125">イベント オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="322cd-125">Update event object.</span></span> |
|[<span data-ttu-id="322cd-126">削除</span><span class="sxs-lookup"><span data-stu-id="322cd-126">Delete</span></span>](../api/event-delete.md) | <span data-ttu-id="322cd-127">なし</span><span class="sxs-lookup"><span data-stu-id="322cd-127">None</span></span> |<span data-ttu-id="322cd-128">イベント オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="322cd-128">Delete event object.</span></span> |
|[<span data-ttu-id="322cd-129">承諾</span><span class="sxs-lookup"><span data-stu-id="322cd-129">accept</span></span>](../api/event-accept.md)|<span data-ttu-id="322cd-130">なし</span><span class="sxs-lookup"><span data-stu-id="322cd-130">None</span></span>|<span data-ttu-id="322cd-131">指定したイベントを承諾します。</span><span class="sxs-lookup"><span data-stu-id="322cd-131">Accept the specified event.</span></span>|
|[<span data-ttu-id="322cd-132">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="322cd-132">tentativelyAccept</span></span>](../api/event-tentativelyaccept.md)|<span data-ttu-id="322cd-133">なし</span><span class="sxs-lookup"><span data-stu-id="322cd-133">None</span></span>|<span data-ttu-id="322cd-134">指定したイベントを仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="322cd-134">Tentatively accept the specified event.</span></span>|
|[<span data-ttu-id="322cd-135">辞退</span><span class="sxs-lookup"><span data-stu-id="322cd-135">decline</span></span>](../api/event-decline.md)|<span data-ttu-id="322cd-136">なし</span><span class="sxs-lookup"><span data-stu-id="322cd-136">None</span></span>|<span data-ttu-id="322cd-137">指定したイベントへの招待を辞退します。</span><span class="sxs-lookup"><span data-stu-id="322cd-137">Decline invitation to the specified event.</span></span>|
|[<span data-ttu-id="322cd-138">delta</span><span class="sxs-lookup"><span data-stu-id="322cd-138">delta</span></span>](../api/event-delta.md)|<span data-ttu-id="322cd-139">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-139">[event](event.md) collection</span></span>|<span data-ttu-id="322cd-140">ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。</span><span class="sxs-lookup"><span data-stu-id="322cd-140">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="322cd-141">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="322cd-141">dismissReminder</span></span>](../api/event-dismissreminder.md)|<span data-ttu-id="322cd-142">なし</span><span class="sxs-lookup"><span data-stu-id="322cd-142">None</span></span>|<span data-ttu-id="322cd-143">指定したイベントのアラームを無視します。</span><span class="sxs-lookup"><span data-stu-id="322cd-143">Dismiss the reminder for the specified event.</span></span>|
|[<span data-ttu-id="322cd-144">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="322cd-144">snoozeReminder</span></span>](../api/event-snoozereminder.md)|<span data-ttu-id="322cd-145">なし</span><span class="sxs-lookup"><span data-stu-id="322cd-145">None</span></span>|<span data-ttu-id="322cd-146">指定したイベントのアラームを再通知します。</span><span class="sxs-lookup"><span data-stu-id="322cd-146">Snooze the reminder for the specified event.</span></span>|
|[<span data-ttu-id="322cd-147">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="322cd-147">List instances</span></span>](../api/event-list-instances.md) |<span data-ttu-id="322cd-148">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-148">[event](event.md) collection</span></span>| <span data-ttu-id="322cd-p102">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが `SeriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="322cd-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="322cd-151">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="322cd-151">**Attachments**</span></span>| | |
|[<span data-ttu-id="322cd-152">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="322cd-152">List attachments</span></span>](../api/event-list-attachments.md) |<span data-ttu-id="322cd-153">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-153">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="322cd-154">イベントのすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="322cd-154">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="322cd-155">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="322cd-155">Add attachment</span></span>](../api/event-post-attachments.md) |[<span data-ttu-id="322cd-156">attachment</span><span class="sxs-lookup"><span data-stu-id="322cd-156">attachment</span></span>](attachment.md)| <span data-ttu-id="322cd-157">添付ファイル コレクションへの投稿により、イベントに新しい添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="322cd-157">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="322cd-158">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="322cd-158">**Open extensions**</span></span>| | |
|[<span data-ttu-id="322cd-159">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="322cd-159">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="322cd-160">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="322cd-160">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="322cd-161">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="322cd-161">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="322cd-162">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="322cd-162">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="322cd-163">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-163">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="322cd-164">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを 1 つまたは複数取得します。</span><span class="sxs-lookup"><span data-stu-id="322cd-164">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="322cd-165">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="322cd-165">**Extended properties**</span></span>| | |
|[<span data-ttu-id="322cd-166">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="322cd-166">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="322cd-167">event</span><span class="sxs-lookup"><span data-stu-id="322cd-167">event</span></span>](event.md)  |<span data-ttu-id="322cd-168">新規または既存のイベントに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="322cd-168">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="322cd-169">単一値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="322cd-169">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="322cd-170">event</span><span class="sxs-lookup"><span data-stu-id="322cd-170">event</span></span>](event.md) | <span data-ttu-id="322cd-171">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含むイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="322cd-171">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="322cd-172">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="322cd-172">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="322cd-173">event</span><span class="sxs-lookup"><span data-stu-id="322cd-173">event</span></span>](event.md) | <span data-ttu-id="322cd-174">新規または既存のイベントに、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="322cd-174">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="322cd-175">複数値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="322cd-175">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="322cd-176">event</span><span class="sxs-lookup"><span data-stu-id="322cd-176">event</span></span>](event.md) | <span data-ttu-id="322cd-177">`$expand` を使用して、複数値の拡張プロパティを含むイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="322cd-177">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="322cd-178">プロパティ</span><span class="sxs-lookup"><span data-stu-id="322cd-178">Properties</span></span>
| <span data-ttu-id="322cd-179">プロパティ</span><span class="sxs-lookup"><span data-stu-id="322cd-179">Property</span></span>     | <span data-ttu-id="322cd-180">種類</span><span class="sxs-lookup"><span data-stu-id="322cd-180">Type</span></span>   |<span data-ttu-id="322cd-181">説明</span><span class="sxs-lookup"><span data-stu-id="322cd-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="322cd-182">attendees</span><span class="sxs-lookup"><span data-stu-id="322cd-182">attendees</span></span>|<span data-ttu-id="322cd-183">[attendee](attendee.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-183">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="322cd-184">イベントの出席者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="322cd-184">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="322cd-185">body</span><span class="sxs-lookup"><span data-stu-id="322cd-185">body</span></span>|[<span data-ttu-id="322cd-186">itemBody</span><span class="sxs-lookup"><span data-stu-id="322cd-186">itemBody</span></span>](itembody.md)|<span data-ttu-id="322cd-p103">イベントに関連付けられたメッセージの本文。HTML 形式またはテキスト形式にできます。</span><span class="sxs-lookup"><span data-stu-id="322cd-p103">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="322cd-189">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="322cd-189">bodyPreview</span></span>|<span data-ttu-id="322cd-190">String</span><span class="sxs-lookup"><span data-stu-id="322cd-190">String</span></span>|<span data-ttu-id="322cd-p104">イベントに関連付けられたメッセージのプレビュー。テキスト形式です。</span><span class="sxs-lookup"><span data-stu-id="322cd-p104">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="322cd-193">categories</span><span class="sxs-lookup"><span data-stu-id="322cd-193">categories</span></span>|<span data-ttu-id="322cd-194">String コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-194">String collection</span></span>|<span data-ttu-id="322cd-195">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="322cd-195">The categories associated with the event.</span></span>|
|<span data-ttu-id="322cd-196">changeKey</span><span class="sxs-lookup"><span data-stu-id="322cd-196">changeKey</span></span>|<span data-ttu-id="322cd-197">String</span><span class="sxs-lookup"><span data-stu-id="322cd-197">String</span></span>|<span data-ttu-id="322cd-p105">イベント オブジェクトのバージョンを識別します。イベントを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="322cd-p105">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="322cd-201">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="322cd-201">createdDateTime</span></span>|<span data-ttu-id="322cd-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="322cd-202">DateTimeOffset</span></span>|<span data-ttu-id="322cd-p106">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="322cd-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="322cd-205">end</span><span class="sxs-lookup"><span data-stu-id="322cd-205">end</span></span>|[<span data-ttu-id="322cd-206">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="322cd-206">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="322cd-207">イベントが終了する日付、時刻、タイムゾーン</span><span class="sxs-lookup"><span data-stu-id="322cd-207">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="322cd-208">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="322cd-208">hasAttachments</span></span>|<span data-ttu-id="322cd-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="322cd-209">Boolean</span></span>|<span data-ttu-id="322cd-210">イベントに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="322cd-210">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="322cd-211">iCalUId</span><span class="sxs-lookup"><span data-stu-id="322cd-211">iCalUId</span></span>|<span data-ttu-id="322cd-212">String</span><span class="sxs-lookup"><span data-stu-id="322cd-212">String</span></span>|<span data-ttu-id="322cd-213">複数の予定表で 1 つのイベントのすべてのインスタンスによって共有される一意識別子。</span><span class="sxs-lookup"><span data-stu-id="322cd-213">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="322cd-214">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="322cd-214">Read-only.</span></span>|
|<span data-ttu-id="322cd-215">id</span><span class="sxs-lookup"><span data-stu-id="322cd-215">id</span></span>|<span data-ttu-id="322cd-216">String</span><span class="sxs-lookup"><span data-stu-id="322cd-216">String</span></span>| <span data-ttu-id="322cd-217">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="322cd-217">Read-only.</span></span>|
|<span data-ttu-id="322cd-218">importance</span><span class="sxs-lookup"><span data-stu-id="322cd-218">importance</span></span>|<span data-ttu-id="322cd-219">importance</span><span class="sxs-lookup"><span data-stu-id="322cd-219">importance</span></span>|<span data-ttu-id="322cd-220">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="322cd-220">The importance of the event.</span></span> <span data-ttu-id="322cd-221">可能な値: `low`、 `normal`、 `high`。</span><span class="sxs-lookup"><span data-stu-id="322cd-221">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="322cd-222">isAllDay</span><span class="sxs-lookup"><span data-stu-id="322cd-222">isAllDay</span></span>|<span data-ttu-id="322cd-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="322cd-223">Boolean</span></span>|<span data-ttu-id="322cd-224">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="322cd-224">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="322cd-225">isCancelled</span><span class="sxs-lookup"><span data-stu-id="322cd-225">isCancelled</span></span>|<span data-ttu-id="322cd-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="322cd-226">Boolean</span></span>|<span data-ttu-id="322cd-227">イベントがキャンセルされた場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="322cd-227">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="322cd-228">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="322cd-228">isOrganizer</span></span>|<span data-ttu-id="322cd-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="322cd-229">Boolean</span></span>|<span data-ttu-id="322cd-230">メッセージの送信者が開催者でもある場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="322cd-230">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="322cd-231">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="322cd-231">isReminderOn</span></span>|<span data-ttu-id="322cd-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="322cd-232">Boolean</span></span>|<span data-ttu-id="322cd-233">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="322cd-233">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="322cd-234">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="322cd-234">lastModifiedDateTime</span></span>|<span data-ttu-id="322cd-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="322cd-235">DateTimeOffset</span></span>|<span data-ttu-id="322cd-p109">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="322cd-p109">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="322cd-238">location</span><span class="sxs-lookup"><span data-stu-id="322cd-238">location</span></span>|[<span data-ttu-id="322cd-239">location</span><span class="sxs-lookup"><span data-stu-id="322cd-239">location</span></span>](location.md)|<span data-ttu-id="322cd-240">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="322cd-240">The location of the event.</span></span>|
|<span data-ttu-id="322cd-241">locations</span><span class="sxs-lookup"><span data-stu-id="322cd-241">locations</span></span>|<span data-ttu-id="322cd-242">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-242">[location](location.md) collection</span></span>|<span data-ttu-id="322cd-243">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="322cd-243">The locations where the event is held or attended from.</span></span> <span data-ttu-id="322cd-244">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="322cd-244">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="322cd-245">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="322cd-245">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="322cd-246">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="322cd-246">onlineMeetingUrl</span></span>|<span data-ttu-id="322cd-247">String</span><span class="sxs-lookup"><span data-stu-id="322cd-247">String</span></span>|<span data-ttu-id="322cd-248">オンライン会議の URL。</span><span class="sxs-lookup"><span data-stu-id="322cd-248">A URL for an online meeting.</span></span> <span data-ttu-id="322cd-249">会議の開催者が Skype 会議などのオンラインの会議とイベントを指定するときにのみ、プロパティが設定されています。</span><span class="sxs-lookup"><span data-stu-id="322cd-249">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="322cd-250">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="322cd-250">Read-only.</span></span>|
|<span data-ttu-id="322cd-251">organizer</span><span class="sxs-lookup"><span data-stu-id="322cd-251">organizer</span></span>|[<span data-ttu-id="322cd-252">recipient</span><span class="sxs-lookup"><span data-stu-id="322cd-252">recipient</span></span>](recipient.md)|<span data-ttu-id="322cd-253">イベントの開催者。</span><span class="sxs-lookup"><span data-stu-id="322cd-253">The organizer of the event.</span></span>|
|<span data-ttu-id="322cd-254">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="322cd-254">originalEndTimeZone</span></span>|<span data-ttu-id="322cd-255">String</span><span class="sxs-lookup"><span data-stu-id="322cd-255">String</span></span>|<span data-ttu-id="322cd-256">イベントの作成時に設定された終了タイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="322cd-256">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="322cd-257">値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="322cd-257">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="322cd-258">originalStart</span><span class="sxs-lookup"><span data-stu-id="322cd-258">originalStart</span></span>|<span data-ttu-id="322cd-259">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="322cd-259">DateTimeOffset</span></span>|<span data-ttu-id="322cd-p113">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="322cd-p113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="322cd-262">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="322cd-262">originalStartTimeZone</span></span>|<span data-ttu-id="322cd-263">String</span><span class="sxs-lookup"><span data-stu-id="322cd-263">String</span></span>|<span data-ttu-id="322cd-p114">イベントが作成されたときに設定された開始タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="322cd-p114">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="322cd-266">recurrence</span><span class="sxs-lookup"><span data-stu-id="322cd-266">recurrence</span></span>|[<span data-ttu-id="322cd-267">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="322cd-267">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="322cd-268">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="322cd-268">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="322cd-269">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="322cd-269">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="322cd-270">Int32</span><span class="sxs-lookup"><span data-stu-id="322cd-270">Int32</span></span>|<span data-ttu-id="322cd-271">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="322cd-271">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="322cd-272">responseRequested</span><span class="sxs-lookup"><span data-stu-id="322cd-272">responseRequested</span></span>|<span data-ttu-id="322cd-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="322cd-273">Boolean</span></span>|<span data-ttu-id="322cd-274">イベントが承諾または辞退されたときに、送信者が応答を希望する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="322cd-274">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="322cd-275">responseStatus</span><span class="sxs-lookup"><span data-stu-id="322cd-275">responseStatus</span></span>|[<span data-ttu-id="322cd-276">responseStatus</span><span class="sxs-lookup"><span data-stu-id="322cd-276">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="322cd-277">イベント メッセージへの応答で送信される応答のタイプを識別します。</span><span class="sxs-lookup"><span data-stu-id="322cd-277">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="322cd-278">sensitivity</span><span class="sxs-lookup"><span data-stu-id="322cd-278">sensitivity</span></span>|<span data-ttu-id="322cd-279">sensitivity</span><span class="sxs-lookup"><span data-stu-id="322cd-279">sensitivity</span></span>| <span data-ttu-id="322cd-280">可能な値: `normal`、 `personal`、 `private`、 `confidential`。</span><span class="sxs-lookup"><span data-stu-id="322cd-280">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="322cd-281">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="322cd-281">seriesMasterId</span></span>|<span data-ttu-id="322cd-282">String</span><span class="sxs-lookup"><span data-stu-id="322cd-282">String</span></span>|<span data-ttu-id="322cd-283">項目の ID、定期的な系列マスター、このイベントが定期的な一連の一部である場合。</span><span class="sxs-lookup"><span data-stu-id="322cd-283">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="322cd-284">showAs</span><span class="sxs-lookup"><span data-stu-id="322cd-284">showAs</span></span>|<span data-ttu-id="322cd-285">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="322cd-285">freeBusyStatus</span></span>|<span data-ttu-id="322cd-286">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="322cd-286">The status to show.</span></span> <span data-ttu-id="322cd-287">可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="322cd-287">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="322cd-288">start</span><span class="sxs-lookup"><span data-stu-id="322cd-288">start</span></span>|[<span data-ttu-id="322cd-289">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="322cd-289">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="322cd-290">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="322cd-290">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="322cd-291">subject</span><span class="sxs-lookup"><span data-stu-id="322cd-291">subject</span></span>|<span data-ttu-id="322cd-292">String</span><span class="sxs-lookup"><span data-stu-id="322cd-292">String</span></span>|<span data-ttu-id="322cd-293">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="322cd-293">The text of the event's subject line.</span></span>|
|<span data-ttu-id="322cd-294">type</span><span class="sxs-lookup"><span data-stu-id="322cd-294">type</span></span>|<span data-ttu-id="322cd-295">eventType</span><span class="sxs-lookup"><span data-stu-id="322cd-295">eventType</span></span>|<span data-ttu-id="322cd-296">イベントの種類。</span><span class="sxs-lookup"><span data-stu-id="322cd-296">The event type.</span></span> <span data-ttu-id="322cd-297">可能な値: `singleInstance`、 `occurrence`、 `exception`、 `seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="322cd-297">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="322cd-298">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="322cd-298">Read-only.</span></span>|
|<span data-ttu-id="322cd-299">webLink</span><span class="sxs-lookup"><span data-stu-id="322cd-299">webLink</span></span>|<span data-ttu-id="322cd-300">String</span><span class="sxs-lookup"><span data-stu-id="322cd-300">String</span></span>|<span data-ttu-id="322cd-301">Outlook Web App でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="322cd-301">The URL to open the event in Outlook Web App.</span></span><br/><br/><span data-ttu-id="322cd-p117">Outlook Web App のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="322cd-p117">The event will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="322cd-304">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="322cd-304">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="322cd-305">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="322cd-305">Relationships</span></span>
| <span data-ttu-id="322cd-306">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="322cd-306">Relationship</span></span> | <span data-ttu-id="322cd-307">型</span><span class="sxs-lookup"><span data-stu-id="322cd-307">Type</span></span>   |<span data-ttu-id="322cd-308">説明</span><span class="sxs-lookup"><span data-stu-id="322cd-308">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="322cd-309">attachments</span><span class="sxs-lookup"><span data-stu-id="322cd-309">attachments</span></span>|<span data-ttu-id="322cd-310">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-310">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="322cd-p118">イベントの [fileAttachment](fileattachment.md) 添付ファイルと [itemAttachment](itemattachment.md) 添付ファイルのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="322cd-p118">The collection of [fileAttachment](fileattachment.md) and [itemAttachment](itemattachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="322cd-315">予定表</span><span class="sxs-lookup"><span data-stu-id="322cd-315">calendar</span></span>|[<span data-ttu-id="322cd-316">calendar</span><span class="sxs-lookup"><span data-stu-id="322cd-316">calendar</span></span>](calendar.md)|<span data-ttu-id="322cd-p119">イベントを含む予定表。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="322cd-p119">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="322cd-320">extensions</span><span class="sxs-lookup"><span data-stu-id="322cd-320">extensions</span></span>|<span data-ttu-id="322cd-321">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-321">[Extension](extension.md) collection</span></span>|<span data-ttu-id="322cd-p120">イベントに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="322cd-p120">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="322cd-325">インスタンス</span><span class="sxs-lookup"><span data-stu-id="322cd-325">instances</span></span>|<span data-ttu-id="322cd-326">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="322cd-326">[event](event.md) collection</span></span>|<span data-ttu-id="322cd-p121">イベントのインスタンス。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="322cd-p121">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="322cd-331">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="322cd-331">multiValueExtendedProperties</span></span>|<span data-ttu-id="322cd-332">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="322cd-332">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="322cd-p122">イベントに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="322cd-p122">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="322cd-336">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="322cd-336">singleValueExtendedProperties</span></span>|<span data-ttu-id="322cd-337">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="322cd-337">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="322cd-p123">イベントに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="322cd-p123">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="322cd-341">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="322cd-341">JSON representation</span></span>

<span data-ttu-id="322cd-342">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="322cd-342">Here is a JSON representation of the resource</span></span>

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


## <a name="see-also"></a><span data-ttu-id="322cd-343">関連項目</span><span class="sxs-lookup"><span data-stu-id="322cd-343">See also</span></span>

- [<span data-ttu-id="322cd-344">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="322cd-344">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="322cd-345">フォルダー内のイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="322cd-345">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)
- [<span data-ttu-id="322cd-346">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="322cd-346">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="322cd-347">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="322cd-347">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="322cd-348">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="322cd-348">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
