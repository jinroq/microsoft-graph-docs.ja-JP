---
title: イベントの更新
description: イベント オブジェクトのプロパティを更新します。
author: angelgolfer-ms
ms.openlocfilehash: 05612f50b038f491598b98c5661fac17238419df
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330675"
---
# <a name="update-event"></a><span data-ttu-id="bc215-103">イベントの更新</span><span class="sxs-lookup"><span data-stu-id="bc215-103">Update event</span></span>

> <span data-ttu-id="bc215-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc215-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc215-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc215-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc215-106">[イベント](../resources/event.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc215-106">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc215-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bc215-107">Permissions</span></span>
<span data-ttu-id="bc215-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc215-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc215-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc215-110">Permission type</span></span>      | <span data-ttu-id="bc215-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc215-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc215-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc215-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc215-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc215-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bc215-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc215-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc215-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc215-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bc215-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc215-116">Application</span></span> | <span data-ttu-id="bc215-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc215-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc215-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc215-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bc215-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc215-119">Request headers</span></span>
| <span data-ttu-id="bc215-120">名前</span><span class="sxs-lookup"><span data-stu-id="bc215-120">Name</span></span>       | <span data-ttu-id="bc215-121">種類</span><span class="sxs-lookup"><span data-stu-id="bc215-121">Type</span></span> | <span data-ttu-id="bc215-122">説明</span><span class="sxs-lookup"><span data-stu-id="bc215-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc215-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc215-123">Authorization</span></span>  | <span data-ttu-id="bc215-124">string</span><span class="sxs-lookup"><span data-stu-id="bc215-124">string</span></span>  | <span data-ttu-id="bc215-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bc215-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc215-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc215-127">Request body</span></span>
<span data-ttu-id="bc215-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="bc215-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc215-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc215-131">Property</span></span>       | <span data-ttu-id="bc215-132">種類</span><span class="sxs-lookup"><span data-stu-id="bc215-132">Type</span></span>    | <span data-ttu-id="bc215-133">説明</span><span class="sxs-lookup"><span data-stu-id="bc215-133">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="bc215-134">attendees</span><span class="sxs-lookup"><span data-stu-id="bc215-134">attendees</span></span>|<span data-ttu-id="bc215-135">Attendee</span><span class="sxs-lookup"><span data-stu-id="bc215-135">Attendee</span></span>|<span data-ttu-id="bc215-136">イベントの参加者のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="bc215-136">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="bc215-137">body</span><span class="sxs-lookup"><span data-stu-id="bc215-137">body</span></span>|<span data-ttu-id="bc215-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="bc215-138">ItemBody</span></span>|<span data-ttu-id="bc215-139">イベントに関連付けられたメッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="bc215-139">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="bc215-140">categories</span><span class="sxs-lookup"><span data-stu-id="bc215-140">categories</span></span>|<span data-ttu-id="bc215-141">String</span><span class="sxs-lookup"><span data-stu-id="bc215-141">String</span></span>|<span data-ttu-id="bc215-142">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="bc215-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="bc215-143">end</span><span class="sxs-lookup"><span data-stu-id="bc215-143">end</span></span>|<span data-ttu-id="bc215-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc215-144">DateTimeTimeZone</span></span>|<span data-ttu-id="bc215-145">イベントが終了する日時。</span><span class="sxs-lookup"><span data-stu-id="bc215-145">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="bc215-p105">既定で、終了時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで終了時刻を表現し、UTC からの時間オフセットを含めることができます。EndTimeZone を使用する場合、StartTimeZone の値も指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bc215-p105">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="bc215-149">この例では、太平洋標準時で 2015 年 2 月 25 日午後 9:34 を指定します ("2015-02-25T21:34:00-08:00")。</span><span class="sxs-lookup"><span data-stu-id="bc215-149">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="bc215-150">importance</span><span class="sxs-lookup"><span data-stu-id="bc215-150">importance</span></span>|<span data-ttu-id="bc215-151">String</span><span class="sxs-lookup"><span data-stu-id="bc215-151">String</span></span>|<span data-ttu-id="bc215-152">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="bc215-152">The importance of the event.</span></span> <span data-ttu-id="bc215-153">可能な値は `low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="bc215-153">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="bc215-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="bc215-154">isAllDay</span></span>|<span data-ttu-id="bc215-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc215-155">Boolean</span></span>|<span data-ttu-id="bc215-156">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="bc215-156">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="bc215-157">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="bc215-157">isReminderOn</span></span>|<span data-ttu-id="bc215-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc215-158">Boolean</span></span>|<span data-ttu-id="bc215-159">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="bc215-159">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="bc215-160">location</span><span class="sxs-lookup"><span data-stu-id="bc215-160">location</span></span>|<span data-ttu-id="bc215-161">Location</span><span class="sxs-lookup"><span data-stu-id="bc215-161">Location</span></span>|<span data-ttu-id="bc215-162">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="bc215-162">The location of the event.</span></span>|
|<span data-ttu-id="bc215-163">locations</span><span class="sxs-lookup"><span data-stu-id="bc215-163">locations</span></span>|<span data-ttu-id="bc215-164">[場所](../resources/location.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="bc215-164">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="bc215-165">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="bc215-165">The locations where the event is held or attended from.</span></span> <span data-ttu-id="bc215-166">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="bc215-166">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="bc215-167">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="bc215-167">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="bc215-168">recurrence</span><span class="sxs-lookup"><span data-stu-id="bc215-168">recurrence</span></span>|<span data-ttu-id="bc215-169">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="bc215-169">PatternedRecurrence</span></span>|<span data-ttu-id="bc215-170">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="bc215-170">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="bc215-171">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="bc215-171">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="bc215-172">Int32</span><span class="sxs-lookup"><span data-stu-id="bc215-172">Int32</span></span>|<span data-ttu-id="bc215-173">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="bc215-173">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="bc215-174">responseRequested</span><span class="sxs-lookup"><span data-stu-id="bc215-174">responseRequested</span></span>|<span data-ttu-id="bc215-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc215-175">Boolean</span></span>|<span data-ttu-id="bc215-176">イベントが承諾または辞退されたときに、送信者が応答を要求する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="bc215-176">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="bc215-177">sensitivity</span><span class="sxs-lookup"><span data-stu-id="bc215-177">sensitivity</span></span>|<span data-ttu-id="bc215-178">String</span><span class="sxs-lookup"><span data-stu-id="bc215-178">String</span></span>| <span data-ttu-id="bc215-179">可能な値は、`normal`、`personal`、`private`、`confidential` です。</span><span class="sxs-lookup"><span data-stu-id="bc215-179">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="bc215-180">showAs</span><span class="sxs-lookup"><span data-stu-id="bc215-180">showAs</span></span>|<span data-ttu-id="bc215-181">String</span><span class="sxs-lookup"><span data-stu-id="bc215-181">String</span></span>|<span data-ttu-id="bc215-182">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="bc215-182">The status to show.</span></span> <span data-ttu-id="bc215-183">使用可能な値: `free` 、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="bc215-183">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="bc215-184">開始</span><span class="sxs-lookup"><span data-stu-id="bc215-184">start</span></span>|<span data-ttu-id="bc215-185">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc215-185">DateTimeTimeZone</span></span>|<span data-ttu-id="bc215-186">イベントの開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="bc215-186">The start time of the event.</span></span> <br/><br/><span data-ttu-id="bc215-p109">既定で、開始時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで開始時刻を表現し、UTC からの時間オフセットを含めることができます。StartTimeZone を使用する場合、EndTimeZone の値も指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bc215-p109">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="bc215-190">この例では、太平洋標準時で 2015 年 2 月 25 日午後 7:34 を指定します "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="bc215-190">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="bc215-191">subject</span><span class="sxs-lookup"><span data-stu-id="bc215-191">subject</span></span>|<span data-ttu-id="bc215-192">String</span><span class="sxs-lookup"><span data-stu-id="bc215-192">String</span></span>|<span data-ttu-id="bc215-193">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="bc215-193">The text of the event's subject line.</span></span>|

<span data-ttu-id="bc215-194">**イベント**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、使用して、`PATCH`を追加、更新、または既存の**イベント**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="bc215-194">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="bc215-195">更新する**イベント**がマスターし、定期的な一連のイベントの場合は、複数の出席者が含まれていて、個別に更新されたインスタンス、複数の通知の電子メールが送信されます: マスターのシリーズとは、インスタンスごとに 1 つのいずれか更新されました。</span><span class="sxs-lookup"><span data-stu-id="bc215-195">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="bc215-196">応答</span><span class="sxs-lookup"><span data-stu-id="bc215-196">Response</span></span>

<span data-ttu-id="bc215-197">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [event](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bc215-197">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="bc215-198">**注:** このメソッドは、HTTP 400 正しくない要求を含む応答のエラー コードを返すことができます`ErrorOccurrenceCrossingBoundary`し、次のエラー メッセージ: 変更されたアイテムを越えるまたは隣接するアイテムが重複しています。</span><span class="sxs-lookup"><span data-stu-id="bc215-198">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="bc215-199">更新プログラムには、定期的なアイテムの例外では、以下の Outlook 制限が違反していることを示します: 発生または日の前の出現箇所では、前日に移動することはできませんし、出現する位置は、次の日の前後に移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="bc215-199">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="bc215-200">例</span><span class="sxs-lookup"><span data-stu-id="bc215-200">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc215-201">要求</span><span class="sxs-lookup"><span data-stu-id="bc215-201">Request</span></span>

<span data-ttu-id="bc215-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bc215-202">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

##### <a name="response"></a><span data-ttu-id="bc215-203">応答</span><span class="sxs-lookup"><span data-stu-id="bc215-203">Response</span></span>
<span data-ttu-id="bc215-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bc215-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a><span data-ttu-id="bc215-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc215-207">See also</span></span>

- [<span data-ttu-id="bc215-208">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="bc215-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bc215-209">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="bc215-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bc215-210">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="bc215-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
