---
title: calendar リソース型
description: イベントのコンテナーである予定表です。 ユーザーの予定表、または Office 365 グループの既定の予定表のいずれかを指定できます。
ms.openlocfilehash: 1c1797897c0efcd7d7196977f93b6a8c611f83f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023585"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="0e74d-104">calendar リソース型</span><span class="sxs-lookup"><span data-stu-id="0e74d-104">calendar resource type</span></span>

<span data-ttu-id="0e74d-105">イベントのコンテナーである予定表です。</span><span class="sxs-lookup"><span data-stu-id="0e74d-105">A calendar which is a container for events.</span></span> <span data-ttu-id="0e74d-106">[ユーザー](user.md)の予定表、または Office 365 [グループ](group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="0e74d-106">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="0e74d-107">**注:** ユーザーの予定表、グループ予定表と対話できるように、いくつかの小さな違いがあります。</span><span class="sxs-lookup"><span data-stu-id="0e74d-107">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

 - <span data-ttu-id="0e74d-108">の[calendarGroup](calendargroup.md)のユーザーの予定表のみを整理することができます。</span><span class="sxs-lookup"><span data-stu-id="0e74d-108">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
 - <span data-ttu-id="0e74d-109">Outlook は、グループのためのすべての会議出席依頼を自動的に受け入れます。</span><span class="sxs-lookup"><span data-stu-id="0e74d-109">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="0e74d-110">ユーザーの予定表のみの[承諾](../api/event-accept.md)、[仮承諾](../api/event-tentativelyaccept.md)、または会議出席依頼を[辞退する](../api/event-decline.md)ことをがします。</span><span class="sxs-lookup"><span data-stu-id="0e74d-110">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
  - <span data-ttu-id="0e74d-111">Outlook は、グループのイベントのアラームをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="0e74d-111">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="0e74d-112">[再通知](../api/event-snoozereminder.md)や[アラーム](reminder.md)を[消す](../api/event-dismissreminder.md)をユーザーの予定表のみにできます。</span><span class="sxs-lookup"><span data-stu-id="0e74d-112">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="0e74d-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e74d-113">Methods</span></span>

| <span data-ttu-id="0e74d-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e74d-114">Method</span></span>       | <span data-ttu-id="0e74d-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0e74d-115">Return Type</span></span>  |<span data-ttu-id="0e74d-116">説明</span><span class="sxs-lookup"><span data-stu-id="0e74d-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e74d-117">予定表を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0e74d-117">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="0e74d-118">[calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e74d-118">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="0e74d-119">ユーザーのすべての予定表を取得するか、既定またはその他の特定の予定表グループの予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-119">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="0e74d-120">予定表を作成する</span><span class="sxs-lookup"><span data-stu-id="0e74d-120">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="0e74d-121">calendar</span><span class="sxs-lookup"><span data-stu-id="0e74d-121">calendar</span></span>](calendar.md)| <span data-ttu-id="0e74d-122">既定の予定表グループまたはユーザーの特定の予定表グループに予定表を作成します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-122">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="0e74d-123">予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="0e74d-123">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="0e74d-124">calendar</span><span class="sxs-lookup"><span data-stu-id="0e74d-124">calendar</span></span>](calendar.md) |<span data-ttu-id="0e74d-125">**予定表**オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-125">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="0e74d-126">ユーザーの予定表、または Office 365 のグループの既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="0e74d-126">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="0e74d-127">更新する</span><span class="sxs-lookup"><span data-stu-id="0e74d-127">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="0e74d-128">calendar</span><span class="sxs-lookup"><span data-stu-id="0e74d-128">calendar</span></span>](calendar.md)  |<span data-ttu-id="0e74d-129">**予定表**オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-129">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="0e74d-130">ユーザーの予定表、または Office 365 のグループの既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="0e74d-130">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="0e74d-131">削除する</span><span class="sxs-lookup"><span data-stu-id="0e74d-131">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="0e74d-132">なし</span><span class="sxs-lookup"><span data-stu-id="0e74d-132">None</span></span> |<span data-ttu-id="0e74d-133">予定表オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-133">Delete calendar object.</span></span> |
|[<span data-ttu-id="0e74d-134">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0e74d-134">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="0e74d-135">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e74d-135">[event](event.md) collection</span></span>| <span data-ttu-id="0e74d-136">ユーザーの標準として設定されている予定表 `(../me/calendarview)` または特定の予定表から、時間範囲で定義したカレンダー ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-136">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="0e74d-137">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0e74d-137">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="0e74d-138">[event](event.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e74d-138">[event](event.md) collection</span></span>| <span data-ttu-id="0e74d-p107">予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="0e74d-141">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="0e74d-141">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="0e74d-142">event</span><span class="sxs-lookup"><span data-stu-id="0e74d-142">event</span></span>](event.md)| <span data-ttu-id="0e74d-143">既定または指定した予定表で新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-143">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="0e74d-144">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="0e74d-144">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="0e74d-145">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="0e74d-145">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="0e74d-146">会議の時間と開催者と出席者の可用性、および時間や場所の制約に基づいて場所をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="0e74d-146">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="0e74d-147">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="0e74d-147">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="0e74d-148">calendar</span><span class="sxs-lookup"><span data-stu-id="0e74d-148">calendar</span></span>](calendar.md)  |<span data-ttu-id="0e74d-149">新規または既存の予定表に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-149">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="0e74d-150">単一値の拡張プロパティを持つ予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="0e74d-150">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="0e74d-151">calendar</span><span class="sxs-lookup"><span data-stu-id="0e74d-151">calendar</span></span>](calendar.md) | <span data-ttu-id="0e74d-152">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-152">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="0e74d-153">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="0e74d-153">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="0e74d-154">calendar</span><span class="sxs-lookup"><span data-stu-id="0e74d-154">calendar</span></span>](calendar.md) | <span data-ttu-id="0e74d-155">新規または既存の予定表に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-155">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="0e74d-156">複数値の拡張プロパティを持つ予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="0e74d-156">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="0e74d-157">calendar</span><span class="sxs-lookup"><span data-stu-id="0e74d-157">calendar</span></span>](calendar.md) | <span data-ttu-id="0e74d-158">`$expand` を使用して、複数値の拡張プロパティを含む予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="0e74d-158">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="0e74d-159">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e74d-159">Properties</span></span>
| <span data-ttu-id="0e74d-160">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e74d-160">Property</span></span>     | <span data-ttu-id="0e74d-161">型</span><span class="sxs-lookup"><span data-stu-id="0e74d-161">Type</span></span>   |<span data-ttu-id="0e74d-162">説明</span><span class="sxs-lookup"><span data-stu-id="0e74d-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e74d-163">canEdit</span><span class="sxs-lookup"><span data-stu-id="0e74d-163">canEdit</span></span> |<span data-ttu-id="0e74d-164">ブール値</span><span class="sxs-lookup"><span data-stu-id="0e74d-164">Boolean</span></span> |<span data-ttu-id="0e74d-p108">ユーザーが予定表に書き込むことができる場合は true、それ以外の場合は false です。予定表を作成したユーザーの場合は、このプロパティは true です。予定表を共有していて、書き込みアクセスが付与されているユーザーの場合も、このプロパティは true です。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p108">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="0e74d-168">canShare</span><span class="sxs-lookup"><span data-stu-id="0e74d-168">canShare</span></span> |<span data-ttu-id="0e74d-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="0e74d-169">Boolean</span></span> |<span data-ttu-id="0e74d-p109">ユーザーに予定表を共有するためのアクセス許可がある場合は true、それ以外の場合は false です。予定表を作成したユーザーのみがその予定表を共有できます。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p109">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="0e74d-172">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="0e74d-172">canViewPrivateItems</span></span> |<span data-ttu-id="0e74d-173">ブール値</span><span class="sxs-lookup"><span data-stu-id="0e74d-173">Boolean</span></span> |<span data-ttu-id="0e74d-174">ユーザーがプライベートとしてマークされている予定表アイテムを読み取れることができる場合は true、それ以外の場合は false です。</span><span class="sxs-lookup"><span data-stu-id="0e74d-174">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="0e74d-175">changeKey</span><span class="sxs-lookup"><span data-stu-id="0e74d-175">changeKey</span></span>|<span data-ttu-id="0e74d-176">String</span><span class="sxs-lookup"><span data-stu-id="0e74d-176">String</span></span>|<span data-ttu-id="0e74d-p110">予定表オブジェクトのバージョンを識別します。予定表を変更するたびに changeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p110">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="0e74d-181">color</span><span class="sxs-lookup"><span data-stu-id="0e74d-181">color</span></span>|<span data-ttu-id="0e74d-182">calendarColor</span><span class="sxs-lookup"><span data-stu-id="0e74d-182">calendarColor</span></span>|<span data-ttu-id="0e74d-p111">UI で予定表を他の予定表から区別するための配色テーマを指定します。プロパティ値は次のとおりです。薄い青=0、薄い緑=1、薄いオレンジ=2、薄い灰色=3、薄い黄=4、薄い青緑=5、薄いピンク=6、薄い茶色=7、薄い赤=8、最大色=9、自動=-1</span><span class="sxs-lookup"><span data-stu-id="0e74d-p111">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="0e74d-185">id</span><span class="sxs-lookup"><span data-stu-id="0e74d-185">id</span></span>|<span data-ttu-id="0e74d-186">String</span><span class="sxs-lookup"><span data-stu-id="0e74d-186">String</span></span>|<span data-ttu-id="0e74d-p112">グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p112">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="0e74d-189">name</span><span class="sxs-lookup"><span data-stu-id="0e74d-189">name</span></span>|<span data-ttu-id="0e74d-190">String</span><span class="sxs-lookup"><span data-stu-id="0e74d-190">String</span></span>|<span data-ttu-id="0e74d-191">予定表の名前。</span><span class="sxs-lookup"><span data-stu-id="0e74d-191">The calendar name.</span></span>|
|<span data-ttu-id="0e74d-192">owner</span><span class="sxs-lookup"><span data-stu-id="0e74d-192">owner</span></span> |[<span data-ttu-id="0e74d-193">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0e74d-193">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="0e74d-p113">設定すると、これは予定表を作成または追加したユーザーを表します。ユーザーが作成または追加した予定表の場合、**owner** プロパティがユーザーに設定されます。ユーザーと共有されている予定表の場合は、**owner** プロパティがその予定表をユーザーと共有した人に設定されます。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p113">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0e74d-197">関係</span><span class="sxs-lookup"><span data-stu-id="0e74d-197">Relationships</span></span>
| <span data-ttu-id="0e74d-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e74d-198">Relationship</span></span> | <span data-ttu-id="0e74d-199">型</span><span class="sxs-lookup"><span data-stu-id="0e74d-199">Type</span></span>   |<span data-ttu-id="0e74d-200">説明</span><span class="sxs-lookup"><span data-stu-id="0e74d-200">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e74d-201">calendarView</span><span class="sxs-lookup"><span data-stu-id="0e74d-201">calendarView</span></span>|<span data-ttu-id="0e74d-202">[Event](event.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e74d-202">[Event](event.md) collection</span></span>|<span data-ttu-id="0e74d-p114">予定表のカレンダー ビュー。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p114">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="0e74d-206">events</span><span class="sxs-lookup"><span data-stu-id="0e74d-206">events</span></span>|<span data-ttu-id="0e74d-207">[Event](event.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e74d-207">[Event](event.md) collection</span></span>|<span data-ttu-id="0e74d-p115">予定表内のイベント。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p115">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="0e74d-211">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="0e74d-211">multiValueExtendedProperties</span></span>|<span data-ttu-id="0e74d-212">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e74d-212">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="0e74d-p116">予定表に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p116">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0e74d-216">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="0e74d-216">singleValueExtendedProperties</span></span>|<span data-ttu-id="0e74d-217">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e74d-217">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="0e74d-p117">予定表に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0e74d-p117">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e74d-221">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e74d-221">JSON representation</span></span>

<span data-ttu-id="0e74d-222">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0e74d-222">Here is a JSON representation of the resource</span></span>

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
