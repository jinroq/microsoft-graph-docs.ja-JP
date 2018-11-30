---
title: イベント リソースの種類
description: 予定表内のイベントです。
ms.openlocfilehash: 33226ac04bcf0dc8365ee56bf70bfa1a381b5ebc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020471"
---
# <a name="event-resource-type"></a><span data-ttu-id="a2ca1-103">イベント リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2ca1-103">event resource type</span></span>

<span data-ttu-id="a2ca1-104">予定表内のイベントです。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-104">An event in a calendar.</span></span>

<span data-ttu-id="a2ca1-105">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-105">This resource supports:</span></span>

- <span data-ttu-id="a2ca1-106">[拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-106">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="a2ca1-107">[変更通知](/graph/webhooks)にサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-107">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="a2ca1-108">[デルタ](../api/event-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/event-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="a2ca1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2ca1-109">Methods</span></span>

| <span data-ttu-id="a2ca1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2ca1-110">Method</span></span>       | <span data-ttu-id="a2ca1-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a2ca1-111">Return Type</span></span>  |<span data-ttu-id="a2ca1-112">説明</span><span class="sxs-lookup"><span data-stu-id="a2ca1-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2ca1-113">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-113">List events</span></span>](../api/user-list-events.md)|<span data-ttu-id="a2ca1-114">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-114">[event](event.md) collection</span></span> |<span data-ttu-id="a2ca1-p101">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p101">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="a2ca1-117">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-117">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="a2ca1-118">event</span><span class="sxs-lookup"><span data-stu-id="a2ca1-118">event</span></span>](event.md)| <span data-ttu-id="a2ca1-119">インスタンス コレクションへの投稿により、新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-119">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="a2ca1-120">イベントの取得</span><span class="sxs-lookup"><span data-stu-id="a2ca1-120">Get event</span></span>](../api/event-get.md) | [<span data-ttu-id="a2ca1-121">event</span><span class="sxs-lookup"><span data-stu-id="a2ca1-121">event</span></span>](event.md) |<span data-ttu-id="a2ca1-122">event オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-122">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="a2ca1-123">更新する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-123">Update</span></span>](../api/event-update.md) | [<span data-ttu-id="a2ca1-124">event</span><span class="sxs-lookup"><span data-stu-id="a2ca1-124">event</span></span>](event.md) |<span data-ttu-id="a2ca1-125">イベント オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-125">Update event object.</span></span> |
|[<span data-ttu-id="a2ca1-126">削除</span><span class="sxs-lookup"><span data-stu-id="a2ca1-126">Delete</span></span>](../api/event-delete.md) | <span data-ttu-id="a2ca1-127">なし</span><span class="sxs-lookup"><span data-stu-id="a2ca1-127">None</span></span> |<span data-ttu-id="a2ca1-128">イベント オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-128">Delete event object.</span></span> |
|[<span data-ttu-id="a2ca1-129">承諾</span><span class="sxs-lookup"><span data-stu-id="a2ca1-129">accept</span></span>](../api/event-accept.md)|<span data-ttu-id="a2ca1-130">なし</span><span class="sxs-lookup"><span data-stu-id="a2ca1-130">None</span></span>|<span data-ttu-id="a2ca1-131">指定したイベントを承諾します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-131">Accept the specified event.</span></span>|
|[<span data-ttu-id="a2ca1-132">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="a2ca1-132">tentativelyAccept</span></span>](../api/event-tentativelyaccept.md)|<span data-ttu-id="a2ca1-133">なし</span><span class="sxs-lookup"><span data-stu-id="a2ca1-133">None</span></span>|<span data-ttu-id="a2ca1-134">指定したイベントを仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-134">Tentatively accept the specified event.</span></span>|
|[<span data-ttu-id="a2ca1-135">辞退</span><span class="sxs-lookup"><span data-stu-id="a2ca1-135">decline</span></span>](../api/event-decline.md)|<span data-ttu-id="a2ca1-136">なし</span><span class="sxs-lookup"><span data-stu-id="a2ca1-136">None</span></span>|<span data-ttu-id="a2ca1-137">指定したイベントへの招待を辞退します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-137">Decline invitation to the specified event.</span></span>|
|[<span data-ttu-id="a2ca1-138">delta</span><span class="sxs-lookup"><span data-stu-id="a2ca1-138">delta</span></span>](../api/event-delta.md)|<span data-ttu-id="a2ca1-139">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-139">[event](event.md) collection</span></span>|<span data-ttu-id="a2ca1-140">ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-140">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="a2ca1-141">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="a2ca1-141">dismissReminder</span></span>](../api/event-dismissreminder.md)|<span data-ttu-id="a2ca1-142">なし</span><span class="sxs-lookup"><span data-stu-id="a2ca1-142">None</span></span>|<span data-ttu-id="a2ca1-143">指定したイベントのアラームを無視します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-143">Dismiss the reminder for the specified event.</span></span>|
|[<span data-ttu-id="a2ca1-144">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="a2ca1-144">snoozeReminder</span></span>](../api/event-snoozereminder.md)|<span data-ttu-id="a2ca1-145">なし</span><span class="sxs-lookup"><span data-stu-id="a2ca1-145">None</span></span>|<span data-ttu-id="a2ca1-146">指定したイベントのアラームを再通知します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-146">Snooze the reminder for the specified event.</span></span>|
|[<span data-ttu-id="a2ca1-147">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="a2ca1-147">List instances</span></span>](../api/event-list-instances.md) |<span data-ttu-id="a2ca1-148">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-148">[event](event.md) collection</span></span>| <span data-ttu-id="a2ca1-p102">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが `SeriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="a2ca1-151">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="a2ca1-151">**Attachments**</span></span>| | |
|[<span data-ttu-id="a2ca1-152">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-152">List attachments</span></span>](../api/event-list-attachments.md) |<span data-ttu-id="a2ca1-153">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-153">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="a2ca1-154">イベントのすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-154">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="a2ca1-155">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-155">Add attachment</span></span>](../api/event-post-attachments.md) |[<span data-ttu-id="a2ca1-156">attachment</span><span class="sxs-lookup"><span data-stu-id="a2ca1-156">attachment</span></span>](attachment.md)| <span data-ttu-id="a2ca1-157">添付ファイル コレクションへの投稿により、イベントに新しい添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-157">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="a2ca1-158">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="a2ca1-158">**Open extensions**</span></span>| | |
|[<span data-ttu-id="a2ca1-159">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-159">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="a2ca1-160">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a2ca1-160">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="a2ca1-161">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-161">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="a2ca1-162">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-162">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="a2ca1-163">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-163">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="a2ca1-164">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを 1 つまたは複数取得します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-164">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="a2ca1-165">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="a2ca1-165">**Extended properties**</span></span>| | |
|[<span data-ttu-id="a2ca1-166">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-166">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="a2ca1-167">event</span><span class="sxs-lookup"><span data-stu-id="a2ca1-167">event</span></span>](event.md)  |<span data-ttu-id="a2ca1-168">新規または既存のイベントに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-168">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="a2ca1-169">単一値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="a2ca1-169">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="a2ca1-170">event</span><span class="sxs-lookup"><span data-stu-id="a2ca1-170">event</span></span>](event.md) | <span data-ttu-id="a2ca1-171">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含むイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-171">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="a2ca1-172">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-172">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="a2ca1-173">event</span><span class="sxs-lookup"><span data-stu-id="a2ca1-173">event</span></span>](event.md) | <span data-ttu-id="a2ca1-174">新規または既存のイベントに、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-174">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="a2ca1-175">複数値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="a2ca1-175">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="a2ca1-176">event</span><span class="sxs-lookup"><span data-stu-id="a2ca1-176">event</span></span>](event.md) | <span data-ttu-id="a2ca1-177">`$expand` を使用して、複数値の拡張プロパティを含むイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-177">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="a2ca1-178">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2ca1-178">Properties</span></span>
| <span data-ttu-id="a2ca1-179">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2ca1-179">Property</span></span>     | <span data-ttu-id="a2ca1-180">型</span><span class="sxs-lookup"><span data-stu-id="a2ca1-180">Type</span></span>   |<span data-ttu-id="a2ca1-181">説明</span><span class="sxs-lookup"><span data-stu-id="a2ca1-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2ca1-182">attendees</span><span class="sxs-lookup"><span data-stu-id="a2ca1-182">attendees</span></span>|<span data-ttu-id="a2ca1-183">[attendee](attendee.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-183">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="a2ca1-184">イベントの出席者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-184">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="a2ca1-185">body</span><span class="sxs-lookup"><span data-stu-id="a2ca1-185">body</span></span>|[<span data-ttu-id="a2ca1-186">itemBody</span><span class="sxs-lookup"><span data-stu-id="a2ca1-186">itemBody</span></span>](itembody.md)|<span data-ttu-id="a2ca1-p103">イベントに関連付けられたメッセージの本文。HTML 形式またはテキスト形式にできます。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p103">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="a2ca1-189">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="a2ca1-189">bodyPreview</span></span>|<span data-ttu-id="a2ca1-190">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-190">String</span></span>|<span data-ttu-id="a2ca1-p104">イベントに関連付けられたメッセージのプレビュー。テキスト形式です。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p104">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="a2ca1-193">categories</span><span class="sxs-lookup"><span data-stu-id="a2ca1-193">categories</span></span>|<span data-ttu-id="a2ca1-194">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-194">String collection</span></span>|<span data-ttu-id="a2ca1-195">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-195">The categories associated with the event.</span></span>|
|<span data-ttu-id="a2ca1-196">changeKey</span><span class="sxs-lookup"><span data-stu-id="a2ca1-196">changeKey</span></span>|<span data-ttu-id="a2ca1-197">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-197">String</span></span>|<span data-ttu-id="a2ca1-p105">イベント オブジェクトのバージョンを識別します。イベントを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p105">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="a2ca1-201">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ca1-201">createdDateTime</span></span>|<span data-ttu-id="a2ca1-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ca1-202">DateTimeOffset</span></span>|<span data-ttu-id="a2ca1-p106">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a2ca1-205">end</span><span class="sxs-lookup"><span data-stu-id="a2ca1-205">end</span></span>|[<span data-ttu-id="a2ca1-206">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a2ca1-206">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a2ca1-207">イベントが終了する日付、時刻、タイムゾーン</span><span class="sxs-lookup"><span data-stu-id="a2ca1-207">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="a2ca1-208">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="a2ca1-208">hasAttachments</span></span>|<span data-ttu-id="a2ca1-209">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2ca1-209">Boolean</span></span>|<span data-ttu-id="a2ca1-210">イベントに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-210">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="a2ca1-211">iCalUId</span><span class="sxs-lookup"><span data-stu-id="a2ca1-211">iCalUId</span></span>|<span data-ttu-id="a2ca1-212">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-212">String</span></span>|<span data-ttu-id="a2ca1-213">複数の予定表で 1 つのイベントのすべてのインスタンスによって共有される一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-213">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="a2ca1-214">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-214">Read-only.</span></span>|
|<span data-ttu-id="a2ca1-215">id</span><span class="sxs-lookup"><span data-stu-id="a2ca1-215">id</span></span>|<span data-ttu-id="a2ca1-216">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-216">String</span></span>| <span data-ttu-id="a2ca1-217">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-217">Read-only.</span></span>|
|<span data-ttu-id="a2ca1-218">importance</span><span class="sxs-lookup"><span data-stu-id="a2ca1-218">importance</span></span>|<span data-ttu-id="a2ca1-219">importance</span><span class="sxs-lookup"><span data-stu-id="a2ca1-219">importance</span></span>|<span data-ttu-id="a2ca1-220">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-220">The importance of the event.</span></span> <span data-ttu-id="a2ca1-221">可能な値: `low`、 `normal`、 `high`。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-221">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="a2ca1-222">isAllDay</span><span class="sxs-lookup"><span data-stu-id="a2ca1-222">isAllDay</span></span>|<span data-ttu-id="a2ca1-223">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2ca1-223">Boolean</span></span>|<span data-ttu-id="a2ca1-224">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-224">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="a2ca1-225">isCancelled</span><span class="sxs-lookup"><span data-stu-id="a2ca1-225">isCancelled</span></span>|<span data-ttu-id="a2ca1-226">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2ca1-226">Boolean</span></span>|<span data-ttu-id="a2ca1-227">イベントがキャンセルされた場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-227">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="a2ca1-228">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="a2ca1-228">isOrganizer</span></span>|<span data-ttu-id="a2ca1-229">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2ca1-229">Boolean</span></span>|<span data-ttu-id="a2ca1-230">メッセージの送信者が開催者でもある場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-230">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="a2ca1-231">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="a2ca1-231">isReminderOn</span></span>|<span data-ttu-id="a2ca1-232">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2ca1-232">Boolean</span></span>|<span data-ttu-id="a2ca1-233">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-233">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="a2ca1-234">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ca1-234">lastModifiedDateTime</span></span>|<span data-ttu-id="a2ca1-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ca1-235">DateTimeOffset</span></span>|<span data-ttu-id="a2ca1-p109">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p109">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a2ca1-238">location</span><span class="sxs-lookup"><span data-stu-id="a2ca1-238">location</span></span>|[<span data-ttu-id="a2ca1-239">location</span><span class="sxs-lookup"><span data-stu-id="a2ca1-239">location</span></span>](location.md)|<span data-ttu-id="a2ca1-240">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-240">The location of the event.</span></span>|
|<span data-ttu-id="a2ca1-241">locations</span><span class="sxs-lookup"><span data-stu-id="a2ca1-241">locations</span></span>|<span data-ttu-id="a2ca1-242">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-242">[location](location.md) collection</span></span>|<span data-ttu-id="a2ca1-243">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-243">The locations where the event is held or attended from.</span></span> <span data-ttu-id="a2ca1-244">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-244">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="a2ca1-245">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-245">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="a2ca1-246">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="a2ca1-246">onlineMeetingUrl</span></span>|<span data-ttu-id="a2ca1-247">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-247">String</span></span>|<span data-ttu-id="a2ca1-248">オンライン会議の URL。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-248">A URL for an online meeting.</span></span> <span data-ttu-id="a2ca1-249">会議の開催者が Skype 会議などのオンラインの会議とイベントを指定するときにのみ、プロパティが設定されています。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-249">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="a2ca1-250">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-250">Read-only.</span></span>|
|<span data-ttu-id="a2ca1-251">organizer</span><span class="sxs-lookup"><span data-stu-id="a2ca1-251">organizer</span></span>|[<span data-ttu-id="a2ca1-252">recipient</span><span class="sxs-lookup"><span data-stu-id="a2ca1-252">recipient</span></span>](recipient.md)|<span data-ttu-id="a2ca1-253">イベントの開催者。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-253">The organizer of the event.</span></span>|
|<span data-ttu-id="a2ca1-254">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="a2ca1-254">originalEndTimeZone</span></span>|<span data-ttu-id="a2ca1-255">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-255">String</span></span>|<span data-ttu-id="a2ca1-256">イベントの作成時に設定された終了タイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-256">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="a2ca1-257">値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-257">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="a2ca1-258">originalStart</span><span class="sxs-lookup"><span data-stu-id="a2ca1-258">originalStart</span></span>|<span data-ttu-id="a2ca1-259">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ca1-259">DateTimeOffset</span></span>|<span data-ttu-id="a2ca1-p113">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a2ca1-262">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="a2ca1-262">originalStartTimeZone</span></span>|<span data-ttu-id="a2ca1-263">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-263">String</span></span>|<span data-ttu-id="a2ca1-p114">イベントが作成されたときに設定された開始タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p114">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="a2ca1-266">recurrence</span><span class="sxs-lookup"><span data-stu-id="a2ca1-266">recurrence</span></span>|[<span data-ttu-id="a2ca1-267">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="a2ca1-267">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="a2ca1-268">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-268">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="a2ca1-269">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="a2ca1-269">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="a2ca1-270">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ca1-270">Int32</span></span>|<span data-ttu-id="a2ca1-271">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-271">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="a2ca1-272">responseRequested</span><span class="sxs-lookup"><span data-stu-id="a2ca1-272">responseRequested</span></span>|<span data-ttu-id="a2ca1-273">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2ca1-273">Boolean</span></span>|<span data-ttu-id="a2ca1-274">イベントが承諾または辞退されたときに、送信者が応答を希望する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-274">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="a2ca1-275">responseStatus</span><span class="sxs-lookup"><span data-stu-id="a2ca1-275">responseStatus</span></span>|[<span data-ttu-id="a2ca1-276">responseStatus</span><span class="sxs-lookup"><span data-stu-id="a2ca1-276">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="a2ca1-277">イベント メッセージへの応答で送信される応答のタイプを識別します。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-277">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="a2ca1-278">sensitivity</span><span class="sxs-lookup"><span data-stu-id="a2ca1-278">sensitivity</span></span>|<span data-ttu-id="a2ca1-279">sensitivity</span><span class="sxs-lookup"><span data-stu-id="a2ca1-279">sensitivity</span></span>| <span data-ttu-id="a2ca1-280">可能な値: `normal`、 `personal`、 `private`、 `confidential`。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-280">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="a2ca1-281">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="a2ca1-281">seriesMasterId</span></span>|<span data-ttu-id="a2ca1-282">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-282">String</span></span>|<span data-ttu-id="a2ca1-283">項目の ID、定期的な系列マスター、このイベントが定期的な一連の一部である場合。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-283">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="a2ca1-284">showAs</span><span class="sxs-lookup"><span data-stu-id="a2ca1-284">showAs</span></span>|<span data-ttu-id="a2ca1-285">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="a2ca1-285">freeBusyStatus</span></span>|<span data-ttu-id="a2ca1-286">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-286">The status to show.</span></span> <span data-ttu-id="a2ca1-287">可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-287">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="a2ca1-288">start</span><span class="sxs-lookup"><span data-stu-id="a2ca1-288">start</span></span>|[<span data-ttu-id="a2ca1-289">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a2ca1-289">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a2ca1-290">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-290">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="a2ca1-291">subject</span><span class="sxs-lookup"><span data-stu-id="a2ca1-291">subject</span></span>|<span data-ttu-id="a2ca1-292">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-292">String</span></span>|<span data-ttu-id="a2ca1-293">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-293">The text of the event's subject line.</span></span>|
|<span data-ttu-id="a2ca1-294">type</span><span class="sxs-lookup"><span data-stu-id="a2ca1-294">type</span></span>|<span data-ttu-id="a2ca1-295">eventType</span><span class="sxs-lookup"><span data-stu-id="a2ca1-295">eventType</span></span>|<span data-ttu-id="a2ca1-296">イベントの種類。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-296">The event type.</span></span> <span data-ttu-id="a2ca1-297">可能な値: `singleInstance`、 `occurrence`、 `exception`、 `seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-297">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="a2ca1-298">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-298">Read-only.</span></span>|
|<span data-ttu-id="a2ca1-299">webLink</span><span class="sxs-lookup"><span data-stu-id="a2ca1-299">webLink</span></span>|<span data-ttu-id="a2ca1-300">String</span><span class="sxs-lookup"><span data-stu-id="a2ca1-300">String</span></span>|<span data-ttu-id="a2ca1-301">Outlook Web App でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-301">The URL to open the event in Outlook Web App.</span></span><br/><br/><span data-ttu-id="a2ca1-p117">Outlook Web App のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p117">The event will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="a2ca1-304">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-304">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2ca1-305">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2ca1-305">Relationships</span></span>
| <span data-ttu-id="a2ca1-306">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2ca1-306">Relationship</span></span> | <span data-ttu-id="a2ca1-307">型</span><span class="sxs-lookup"><span data-stu-id="a2ca1-307">Type</span></span>   |<span data-ttu-id="a2ca1-308">説明</span><span class="sxs-lookup"><span data-stu-id="a2ca1-308">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2ca1-309">attachments</span><span class="sxs-lookup"><span data-stu-id="a2ca1-309">attachments</span></span>|<span data-ttu-id="a2ca1-310">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-310">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="a2ca1-p118">イベントの [fileAttachment](fileattachment.md) 添付ファイルと [itemAttachment](itemattachment.md) 添付ファイルのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p118">The collection of [fileAttachment](fileattachment.md) and [itemAttachment](itemattachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a2ca1-315">予定表</span><span class="sxs-lookup"><span data-stu-id="a2ca1-315">calendar</span></span>|[<span data-ttu-id="a2ca1-316">calendar</span><span class="sxs-lookup"><span data-stu-id="a2ca1-316">calendar</span></span>](calendar.md)|<span data-ttu-id="a2ca1-p119">イベントを含む予定表。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p119">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="a2ca1-320">extensions</span><span class="sxs-lookup"><span data-stu-id="a2ca1-320">extensions</span></span>|<span data-ttu-id="a2ca1-321">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-321">[Extension](extension.md) collection</span></span>|<span data-ttu-id="a2ca1-p120">イベントに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p120">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a2ca1-325">インスタンス</span><span class="sxs-lookup"><span data-stu-id="a2ca1-325">instances</span></span>|<span data-ttu-id="a2ca1-326">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ca1-326">[event](event.md) collection</span></span>|<span data-ttu-id="a2ca1-p121">イベントのインスタンス。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p121">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a2ca1-331">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a2ca1-331">multiValueExtendedProperties</span></span>|<span data-ttu-id="a2ca1-332">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="a2ca1-332">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="a2ca1-p122">イベントに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p122">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a2ca1-336">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a2ca1-336">singleValueExtendedProperties</span></span>|<span data-ttu-id="a2ca1-337">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="a2ca1-337">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="a2ca1-p123">イベントに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a2ca1-p123">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2ca1-341">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2ca1-341">JSON representation</span></span>

<span data-ttu-id="a2ca1-342">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a2ca1-342">Here is a JSON representation of the resource</span></span>

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


## <a name="see-also"></a><span data-ttu-id="a2ca1-343">関連項目</span><span class="sxs-lookup"><span data-stu-id="a2ca1-343">See also</span></span>

- [<span data-ttu-id="a2ca1-344">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-344">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="a2ca1-345">フォルダー内のイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-345">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)
- [<span data-ttu-id="a2ca1-346">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-346">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a2ca1-347">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="a2ca1-347">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a2ca1-348">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="a2ca1-348">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
