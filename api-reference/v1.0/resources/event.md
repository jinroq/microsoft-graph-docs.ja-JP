---
title: イベント リソースの種類
description: 予定表内のイベントです。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 0be46df98faf4540e221a140daf0ec22355fc24a
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778727"
---
# <a name="event-resource-type"></a><span data-ttu-id="50e37-103">event リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50e37-103">event resource type</span></span>

<span data-ttu-id="50e37-104">[ユーザー](user.md)の予定表か、Office 365 [グループ](group.md)の既定の予定表のイベントです。</span><span class="sxs-lookup"><span data-stu-id="50e37-104">An event in a [user](user.md) calendar, or the default calendar of an Office 365 [group](group.md).</span></span>

<span data-ttu-id="50e37-105">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="50e37-105">This resource supports:</span></span>

- <span data-ttu-id="50e37-106">[拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="50e37-106">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="50e37-107">[変更通知](/graph/webhooks)を受信します。</span><span class="sxs-lookup"><span data-stu-id="50e37-107">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="50e37-108">[デルタ](../api/event-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="50e37-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/event-delta.md) function.</span></span>

> <span data-ttu-id="50e37-109">**注:** ユーザーの予定表とグループの予定表、およびそのイベントの操作方法には、わずかな相違点がいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="50e37-109">**Note:** There are a few minor differences in the way you can interact with user calendars, group calendars, and their events:</span></span>

- <span data-ttu-id="50e37-110">[calendarGroup](calendargroup.md) にはユーザーの予定表のみを整理できます。</span><span class="sxs-lookup"><span data-stu-id="50e37-110">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="50e37-111">Outlook はグループの代わりにすべての会議出席依頼を自動的に受け入れます。</span><span class="sxs-lookup"><span data-stu-id="50e37-111">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="50e37-112">_ユーザー_の予定表の会議出席依頼のみを[承諾](../api/event-accept.md)、[仮承諾](../api/event-tentativelyaccept.md)、または[辞退](../api/event-decline.md)できます。</span><span class="sxs-lookup"><span data-stu-id="50e37-112">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for _user_ calendars only.</span></span>
- <span data-ttu-id="50e37-113">Outlook はグループ イベントのアラームをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="50e37-113">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="50e37-114">_ユーザー_の予定表についてのみ、[リマインダー](reminder.md)を[再起動](../api/event-snoozereminder.md)または[無視](../api/event-dismissreminder.md)できます。</span><span class="sxs-lookup"><span data-stu-id="50e37-114">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for _user_ calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="50e37-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="50e37-115">Methods</span></span>

| <span data-ttu-id="50e37-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="50e37-116">Method</span></span>       | <span data-ttu-id="50e37-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="50e37-117">Return Type</span></span>  |<span data-ttu-id="50e37-118">説明</span><span class="sxs-lookup"><span data-stu-id="50e37-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50e37-119">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="50e37-119">List events</span></span>](../api/user-list-events.md)|<span data-ttu-id="50e37-120">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-120">[event](event.md) collection</span></span> |<span data-ttu-id="50e37-p103">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="50e37-p103">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="50e37-123">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="50e37-123">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="50e37-124">event</span><span class="sxs-lookup"><span data-stu-id="50e37-124">event</span></span>](event.md)| <span data-ttu-id="50e37-125">インスタンス コレクションへの投稿により、新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="50e37-125">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="50e37-126">イベントの取得</span><span class="sxs-lookup"><span data-stu-id="50e37-126">Get event</span></span>](../api/event-get.md) | [<span data-ttu-id="50e37-127">event</span><span class="sxs-lookup"><span data-stu-id="50e37-127">event</span></span>](event.md) |<span data-ttu-id="50e37-128">event オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="50e37-128">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="50e37-129">更新する</span><span class="sxs-lookup"><span data-stu-id="50e37-129">Update</span></span>](../api/event-update.md) | [<span data-ttu-id="50e37-130">event</span><span class="sxs-lookup"><span data-stu-id="50e37-130">event</span></span>](event.md) |<span data-ttu-id="50e37-131">イベント オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="50e37-131">Update event object.</span></span> |
|[<span data-ttu-id="50e37-132">削除</span><span class="sxs-lookup"><span data-stu-id="50e37-132">Delete</span></span>](../api/event-delete.md) | <span data-ttu-id="50e37-133">なし</span><span class="sxs-lookup"><span data-stu-id="50e37-133">None</span></span> |<span data-ttu-id="50e37-134">イベント オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="50e37-134">Delete event object.</span></span> |
|[<span data-ttu-id="50e37-135">承諾</span><span class="sxs-lookup"><span data-stu-id="50e37-135">accept</span></span>](../api/event-accept.md)|<span data-ttu-id="50e37-136">なし</span><span class="sxs-lookup"><span data-stu-id="50e37-136">None</span></span>|<span data-ttu-id="50e37-137">ユーザーの予定表の指定のイベントを承諾します。</span><span class="sxs-lookup"><span data-stu-id="50e37-137">Accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="50e37-138">仮承諾する</span><span class="sxs-lookup"><span data-stu-id="50e37-138">tentativelyAccept</span></span>](../api/event-tentativelyaccept.md)|<span data-ttu-id="50e37-139">なし</span><span class="sxs-lookup"><span data-stu-id="50e37-139">None</span></span>|<span data-ttu-id="50e37-140">ユーザーの予定表の指定のイベントを仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="50e37-140">Tentatively accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="50e37-141">辞退する</span><span class="sxs-lookup"><span data-stu-id="50e37-141">decline</span></span>](../api/event-decline.md)|<span data-ttu-id="50e37-142">なし</span><span class="sxs-lookup"><span data-stu-id="50e37-142">None</span></span>|<span data-ttu-id="50e37-143">ユーザーの予定表の指定のイベントに対する詳細を辞退します。</span><span class="sxs-lookup"><span data-stu-id="50e37-143">Decline invitation to the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="50e37-144">delta</span><span class="sxs-lookup"><span data-stu-id="50e37-144">delta</span></span>](../api/event-delta.md)|<span data-ttu-id="50e37-145">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-145">[event](event.md) collection</span></span>|<span data-ttu-id="50e37-146">ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。</span><span class="sxs-lookup"><span data-stu-id="50e37-146">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="50e37-147">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="50e37-147">dismissReminder</span></span>](../api/event-dismissreminder.md)|<span data-ttu-id="50e37-148">なし</span><span class="sxs-lookup"><span data-stu-id="50e37-148">None</span></span>|<span data-ttu-id="50e37-149">ユーザーの予定表の指定したイベントのリマインダーを無視します。</span><span class="sxs-lookup"><span data-stu-id="50e37-149">Dismiss the reminder for the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="50e37-150">リマインダーを再起動する</span><span class="sxs-lookup"><span data-stu-id="50e37-150">snoozeReminder</span></span>](../api/event-snoozereminder.md)|<span data-ttu-id="50e37-151">なし</span><span class="sxs-lookup"><span data-stu-id="50e37-151">None</span></span>|<span data-ttu-id="50e37-152">ユーザーの予定表の指定したイベントのリマインダーを新しい時刻まで延期します。</span><span class="sxs-lookup"><span data-stu-id="50e37-152">Postpone a reminder for the specified event in a user calendar until a new time.</span></span>|
|[<span data-ttu-id="50e37-153">インスタンスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="50e37-153">List instances</span></span>](../api/event-list-instances.md) |<span data-ttu-id="50e37-154">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-154">[event](event.md) collection</span></span>| <span data-ttu-id="50e37-p104">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが `SeriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="50e37-p104">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="50e37-157">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="50e37-157">**Attachments**</span></span>| | |
|[<span data-ttu-id="50e37-158">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="50e37-158">List attachments</span></span>](../api/event-list-attachments.md) |<span data-ttu-id="50e37-159">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-159">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="50e37-160">イベントのすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="50e37-160">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="50e37-161">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="50e37-161">Add attachment</span></span>](../api/event-post-attachments.md) |[<span data-ttu-id="50e37-162">attachment</span><span class="sxs-lookup"><span data-stu-id="50e37-162">attachment</span></span>](attachment.md)| <span data-ttu-id="50e37-163">添付ファイル コレクションへの投稿により、イベントに新しい添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="50e37-163">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="50e37-164">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="50e37-164">**Open extensions**</span></span>| | |
|[<span data-ttu-id="50e37-165">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="50e37-165">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="50e37-166">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="50e37-166">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="50e37-167">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="50e37-167">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="50e37-168">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="50e37-168">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="50e37-169">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-169">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="50e37-170">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを 1 つまたは複数取得します。</span><span class="sxs-lookup"><span data-stu-id="50e37-170">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="50e37-171">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="50e37-171">**Extended properties**</span></span>| | |
|[<span data-ttu-id="50e37-172">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="50e37-172">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="50e37-173">event</span><span class="sxs-lookup"><span data-stu-id="50e37-173">event</span></span>](event.md)  |<span data-ttu-id="50e37-174">新規または既存のイベントに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="50e37-174">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="50e37-175">単一値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="50e37-175">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="50e37-176">event</span><span class="sxs-lookup"><span data-stu-id="50e37-176">event</span></span>](event.md) | <span data-ttu-id="50e37-177">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含むイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="50e37-177">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="50e37-178">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="50e37-178">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="50e37-179">event</span><span class="sxs-lookup"><span data-stu-id="50e37-179">event</span></span>](event.md) | <span data-ttu-id="50e37-180">新規または既存のイベントに、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="50e37-180">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="50e37-181">複数値の拡張プロパティを持つイベントの取得</span><span class="sxs-lookup"><span data-stu-id="50e37-181">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="50e37-182">event</span><span class="sxs-lookup"><span data-stu-id="50e37-182">event</span></span>](event.md) | <span data-ttu-id="50e37-183">`$expand` を使用して、複数値の拡張プロパティを含むイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="50e37-183">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="50e37-184">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50e37-184">Properties</span></span>
| <span data-ttu-id="50e37-185">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50e37-185">Property</span></span>     | <span data-ttu-id="50e37-186">型</span><span class="sxs-lookup"><span data-stu-id="50e37-186">Type</span></span>   |<span data-ttu-id="50e37-187">説明</span><span class="sxs-lookup"><span data-stu-id="50e37-187">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50e37-188">attendees</span><span class="sxs-lookup"><span data-stu-id="50e37-188">attendees</span></span>|<span data-ttu-id="50e37-189">[attendee](attendee.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-189">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="50e37-190">イベントの出席者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="50e37-190">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="50e37-191">body</span><span class="sxs-lookup"><span data-stu-id="50e37-191">body</span></span>|[<span data-ttu-id="50e37-192">itemBody</span><span class="sxs-lookup"><span data-stu-id="50e37-192">itemBody</span></span>](itembody.md)|<span data-ttu-id="50e37-p105">イベントに関連付けられたメッセージの本文。HTML 形式またはテキスト形式にできます。</span><span class="sxs-lookup"><span data-stu-id="50e37-p105">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="50e37-195">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="50e37-195">bodyPreview</span></span>|<span data-ttu-id="50e37-196">String</span><span class="sxs-lookup"><span data-stu-id="50e37-196">String</span></span>|<span data-ttu-id="50e37-p106">イベントに関連付けられたメッセージのプレビュー。テキスト形式です。</span><span class="sxs-lookup"><span data-stu-id="50e37-p106">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="50e37-199">categories</span><span class="sxs-lookup"><span data-stu-id="50e37-199">categories</span></span>|<span data-ttu-id="50e37-200">String collection</span><span class="sxs-lookup"><span data-stu-id="50e37-200">String collection</span></span>|<span data-ttu-id="50e37-201">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="50e37-201">The categories associated with the event.</span></span>|
|<span data-ttu-id="50e37-202">changeKey</span><span class="sxs-lookup"><span data-stu-id="50e37-202">changeKey</span></span>|<span data-ttu-id="50e37-203">String</span><span class="sxs-lookup"><span data-stu-id="50e37-203">String</span></span>|<span data-ttu-id="50e37-p107">イベント オブジェクトのバージョンを識別します。イベントを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="50e37-p107">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="50e37-207">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50e37-207">createdDateTime</span></span>|<span data-ttu-id="50e37-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50e37-208">DateTimeOffset</span></span>|<span data-ttu-id="50e37-p108">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50e37-p108">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50e37-211">end</span><span class="sxs-lookup"><span data-stu-id="50e37-211">end</span></span>|[<span data-ttu-id="50e37-212">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="50e37-212">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="50e37-213">イベントが終了する日付、時刻、タイムゾーン</span><span class="sxs-lookup"><span data-stu-id="50e37-213">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="50e37-214">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="50e37-214">hasAttachments</span></span>|<span data-ttu-id="50e37-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e37-215">Boolean</span></span>|<span data-ttu-id="50e37-216">イベントに添付ファイルが含まれている場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="50e37-216">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="50e37-217">iCalUId</span><span class="sxs-lookup"><span data-stu-id="50e37-217">iCalUId</span></span>|<span data-ttu-id="50e37-218">String</span><span class="sxs-lookup"><span data-stu-id="50e37-218">String</span></span>|<span data-ttu-id="50e37-219">複数の予定表で 1 つのイベントのすべてのインスタンスによって共有される一意識別子。</span><span class="sxs-lookup"><span data-stu-id="50e37-219">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="50e37-220">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="50e37-220">Read-only.</span></span>|
|<span data-ttu-id="50e37-221">id</span><span class="sxs-lookup"><span data-stu-id="50e37-221">id</span></span>|<span data-ttu-id="50e37-222">String</span><span class="sxs-lookup"><span data-stu-id="50e37-222">String</span></span>| <span data-ttu-id="50e37-223">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="50e37-223">Read-only.</span></span>|
|<span data-ttu-id="50e37-224">重要度</span><span class="sxs-lookup"><span data-stu-id="50e37-224">importance</span></span>|<span data-ttu-id="50e37-225">重要度</span><span class="sxs-lookup"><span data-stu-id="50e37-225">importance</span></span>|<span data-ttu-id="50e37-226">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="50e37-226">The importance of the event.</span></span> <span data-ttu-id="50e37-227">使用可能な値: `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="50e37-227">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="50e37-228">isAllDay</span><span class="sxs-lookup"><span data-stu-id="50e37-228">isAllDay</span></span>|<span data-ttu-id="50e37-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e37-229">Boolean</span></span>|<span data-ttu-id="50e37-230">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="50e37-230">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="50e37-231">isCancelled</span><span class="sxs-lookup"><span data-stu-id="50e37-231">isCancelled</span></span>|<span data-ttu-id="50e37-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e37-232">Boolean</span></span>|<span data-ttu-id="50e37-233">イベントがキャンセルされた場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="50e37-233">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="50e37-234">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="50e37-234">isOrganizer</span></span>|<span data-ttu-id="50e37-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e37-235">Boolean</span></span>|<span data-ttu-id="50e37-236">メッセージの送信者が開催者でもある場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="50e37-236">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="50e37-237">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="50e37-237">isReminderOn</span></span>|<span data-ttu-id="50e37-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e37-238">Boolean</span></span>|<span data-ttu-id="50e37-239">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="50e37-239">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="50e37-240">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50e37-240">lastModifiedDateTime</span></span>|<span data-ttu-id="50e37-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50e37-241">DateTimeOffset</span></span>|<span data-ttu-id="50e37-p111">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50e37-p111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50e37-244">location</span><span class="sxs-lookup"><span data-stu-id="50e37-244">location</span></span>|[<span data-ttu-id="50e37-245">location</span><span class="sxs-lookup"><span data-stu-id="50e37-245">location</span></span>](location.md)|<span data-ttu-id="50e37-246">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="50e37-246">The location of the event.</span></span>|
|<span data-ttu-id="50e37-247">locations</span><span class="sxs-lookup"><span data-stu-id="50e37-247">locations</span></span>|<span data-ttu-id="50e37-248">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-248">[location](location.md) collection</span></span>|<span data-ttu-id="50e37-249">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="50e37-249">The locations where the event is held or attended from.</span></span> <span data-ttu-id="50e37-250">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="50e37-250">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="50e37-251">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="50e37-251">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="50e37-252">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="50e37-252">onlineMeetingUrl</span></span>|<span data-ttu-id="50e37-253">String</span><span class="sxs-lookup"><span data-stu-id="50e37-253">String</span></span>|<span data-ttu-id="50e37-254">オンライン会議の URL。</span><span class="sxs-lookup"><span data-stu-id="50e37-254">A URL for an online meeting.</span></span> <span data-ttu-id="50e37-255">このプロパティは、開催者が Skype 会議などのオンライン会議としてイベントを指定する場合にのみ設定します。</span><span class="sxs-lookup"><span data-stu-id="50e37-255">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="50e37-256">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="50e37-256">Read-only.</span></span>|
|<span data-ttu-id="50e37-257">構成内容変更</span><span class="sxs-lookup"><span data-stu-id="50e37-257">organizer</span></span>|[<span data-ttu-id="50e37-258">recipient</span><span class="sxs-lookup"><span data-stu-id="50e37-258">recipient</span></span>](recipient.md)|<span data-ttu-id="50e37-259">イベントの開催者。</span><span class="sxs-lookup"><span data-stu-id="50e37-259">The organizer of the event.</span></span>|
|<span data-ttu-id="50e37-260">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="50e37-260">originalEndTimeZone</span></span>|<span data-ttu-id="50e37-261">String</span><span class="sxs-lookup"><span data-stu-id="50e37-261">String</span></span>|<span data-ttu-id="50e37-262">イベントの作成時に設定された終了タイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="50e37-262">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="50e37-263">値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="50e37-263">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="50e37-264">originalStart</span><span class="sxs-lookup"><span data-stu-id="50e37-264">originalStart</span></span>|<span data-ttu-id="50e37-265">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50e37-265">DateTimeOffset</span></span>|<span data-ttu-id="50e37-p115">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50e37-p115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50e37-268">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="50e37-268">originalStartTimeZone</span></span>|<span data-ttu-id="50e37-269">String</span><span class="sxs-lookup"><span data-stu-id="50e37-269">String</span></span>|<span data-ttu-id="50e37-p116">イベントが作成されたときに設定された開始タイム ゾーン。値 `tzone://Microsoft/Custom` は、デスクトップの Outlook で、従来のカスタム タイム ゾーンが設定されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="50e37-p116">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="50e37-272">recurrence</span><span class="sxs-lookup"><span data-stu-id="50e37-272">recurrence</span></span>|[<span data-ttu-id="50e37-273">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="50e37-273">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="50e37-274">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="50e37-274">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="50e37-275">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="50e37-275">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="50e37-276">Int32</span><span class="sxs-lookup"><span data-stu-id="50e37-276">Int32</span></span>|<span data-ttu-id="50e37-277">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="50e37-277">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="50e37-278">responseRequested</span><span class="sxs-lookup"><span data-stu-id="50e37-278">responseRequested</span></span>|<span data-ttu-id="50e37-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e37-279">Boolean</span></span>|<span data-ttu-id="50e37-280">イベントが承諾または辞退されたときに、送信者が応答を希望する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="50e37-280">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="50e37-281">responseStatus</span><span class="sxs-lookup"><span data-stu-id="50e37-281">responseStatus</span></span>|[<span data-ttu-id="50e37-282">responseStatus</span><span class="sxs-lookup"><span data-stu-id="50e37-282">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="50e37-283">イベント メッセージへの応答で送信される応答のタイプを識別します。</span><span class="sxs-lookup"><span data-stu-id="50e37-283">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="50e37-284">sensitivity</span><span class="sxs-lookup"><span data-stu-id="50e37-284">sensitivity</span></span>|<span data-ttu-id="50e37-285">sensitivity</span><span class="sxs-lookup"><span data-stu-id="50e37-285">sensitivity</span></span>| <span data-ttu-id="50e37-286">使用可能な値: `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="50e37-286">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="50e37-287">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="50e37-287">seriesMasterId</span></span>|<span data-ttu-id="50e37-288">String</span><span class="sxs-lookup"><span data-stu-id="50e37-288">String</span></span>|<span data-ttu-id="50e37-289">対象イベントが定期的なアイテムの一部である場合、定期的なアイテムのマスター アイテムの ID。</span><span class="sxs-lookup"><span data-stu-id="50e37-289">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="50e37-290">showAs</span><span class="sxs-lookup"><span data-stu-id="50e37-290">showAs</span></span>|<span data-ttu-id="50e37-291">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="50e37-291">freeBusyStatus</span></span>|<span data-ttu-id="50e37-292">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="50e37-292">The status to show.</span></span> <span data-ttu-id="50e37-293">使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="50e37-293">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="50e37-294">開始</span><span class="sxs-lookup"><span data-stu-id="50e37-294">start</span></span>|[<span data-ttu-id="50e37-295">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="50e37-295">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="50e37-296">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="50e37-296">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="50e37-297">subject</span><span class="sxs-lookup"><span data-stu-id="50e37-297">subject</span></span>|<span data-ttu-id="50e37-298">String</span><span class="sxs-lookup"><span data-stu-id="50e37-298">String</span></span>|<span data-ttu-id="50e37-299">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="50e37-299">The text of the event's subject line.</span></span>|
|<span data-ttu-id="50e37-300">type</span><span class="sxs-lookup"><span data-stu-id="50e37-300">type</span></span>|<span data-ttu-id="50e37-301">eventType</span><span class="sxs-lookup"><span data-stu-id="50e37-301">eventType</span></span>|<span data-ttu-id="50e37-302">イベントの種類。</span><span class="sxs-lookup"><span data-stu-id="50e37-302">The event type.</span></span> <span data-ttu-id="50e37-303">使用可能な値: `singleInstance`、`occurrence`、`exception`、`seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="50e37-303">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="50e37-304">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="50e37-304">Read-only.</span></span>|
|<span data-ttu-id="50e37-305">webLink</span><span class="sxs-lookup"><span data-stu-id="50e37-305">webLink</span></span>|<span data-ttu-id="50e37-306">String</span><span class="sxs-lookup"><span data-stu-id="50e37-306">String</span></span>|<span data-ttu-id="50e37-307">Outlook Web App でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="50e37-307">The URL to open the event in Outlook Web App.</span></span><br/><br/><span data-ttu-id="50e37-p119">Outlook Web App のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="50e37-p119">The event will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="50e37-310">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="50e37-310">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50e37-311">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="50e37-311">Relationships</span></span>
| <span data-ttu-id="50e37-312">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="50e37-312">Relationship</span></span> | <span data-ttu-id="50e37-313">型</span><span class="sxs-lookup"><span data-stu-id="50e37-313">Type</span></span>   |<span data-ttu-id="50e37-314">説明</span><span class="sxs-lookup"><span data-stu-id="50e37-314">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50e37-315">attachments</span><span class="sxs-lookup"><span data-stu-id="50e37-315">attachments</span></span>|<span data-ttu-id="50e37-316">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-316">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="50e37-p120">イベントの [fileAttachment](fileattachment.md) 添付ファイルと [itemAttachment](itemattachment.md) 添付ファイルのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="50e37-p120">The collection of [fileAttachment](fileattachment.md) and [itemAttachment](itemattachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50e37-321">予定表</span><span class="sxs-lookup"><span data-stu-id="50e37-321">calendar</span></span>|[<span data-ttu-id="50e37-322">calendar</span><span class="sxs-lookup"><span data-stu-id="50e37-322">calendar</span></span>](calendar.md)|<span data-ttu-id="50e37-p121">イベントを含む予定表。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="50e37-p121">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="50e37-326">extensions</span><span class="sxs-lookup"><span data-stu-id="50e37-326">extensions</span></span>|<span data-ttu-id="50e37-327">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-327">[Extension](extension.md) collection</span></span>|<span data-ttu-id="50e37-p122">イベントに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="50e37-p122">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50e37-331">インスタンス</span><span class="sxs-lookup"><span data-stu-id="50e37-331">instances</span></span>|<span data-ttu-id="50e37-332">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50e37-332">[event](event.md) collection</span></span>|<span data-ttu-id="50e37-p123">イベントのインスタンス。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="50e37-p123">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50e37-337">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="50e37-337">multiValueExtendedProperties</span></span>|<span data-ttu-id="50e37-338">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="50e37-338">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="50e37-p124">イベントに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="50e37-p124">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50e37-342">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="50e37-342">singleValueExtendedProperties</span></span>|<span data-ttu-id="50e37-343">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="50e37-343">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="50e37-p125">イベントに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="50e37-p125">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50e37-347">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50e37-347">JSON representation</span></span>

<span data-ttu-id="50e37-348">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="50e37-348">Here is a JSON representation of the resource</span></span>

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


## <a name="see-also"></a><span data-ttu-id="50e37-349">関連項目</span><span class="sxs-lookup"><span data-stu-id="50e37-349">See also</span></span>

- [<span data-ttu-id="50e37-350">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="50e37-350">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="50e37-351">フォルダー内のイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="50e37-351">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)
- [<span data-ttu-id="50e37-352">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="50e37-352">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="50e37-353">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="50e37-353">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="50e37-354">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="50e37-354">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
