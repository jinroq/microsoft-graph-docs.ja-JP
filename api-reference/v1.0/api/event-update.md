---
title: イベントの更新
description: イベント オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 441a135cf43226927e9a8aee074c2547b9beb23e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972370"
---
# <a name="update-event"></a><span data-ttu-id="f205b-103">イベントの更新</span><span class="sxs-lookup"><span data-stu-id="f205b-103">Update event</span></span>

<span data-ttu-id="f205b-104">[イベント](../resources/event.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f205b-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f205b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f205b-105">Permissions</span></span>
<span data-ttu-id="f205b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f205b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f205b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f205b-108">Permission type</span></span>      | <span data-ttu-id="f205b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f205b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f205b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f205b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f205b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f205b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f205b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f205b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f205b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f205b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f205b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f205b-114">Application</span></span> | <span data-ttu-id="f205b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f205b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f205b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f205b-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f205b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f205b-117">Request headers</span></span>
| <span data-ttu-id="f205b-118">名前</span><span class="sxs-lookup"><span data-stu-id="f205b-118">Name</span></span>       | <span data-ttu-id="f205b-119">種類</span><span class="sxs-lookup"><span data-stu-id="f205b-119">Type</span></span> | <span data-ttu-id="f205b-120">説明</span><span class="sxs-lookup"><span data-stu-id="f205b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f205b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f205b-121">Authorization</span></span>  | <span data-ttu-id="f205b-122">string</span><span class="sxs-lookup"><span data-stu-id="f205b-122">string</span></span>  | <span data-ttu-id="f205b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f205b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f205b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f205b-125">Request body</span></span>
<span data-ttu-id="f205b-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f205b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f205b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f205b-129">Property</span></span>     | <span data-ttu-id="f205b-130">種類</span><span class="sxs-lookup"><span data-stu-id="f205b-130">Type</span></span>   |<span data-ttu-id="f205b-131">説明</span><span class="sxs-lookup"><span data-stu-id="f205b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f205b-132">attendees</span><span class="sxs-lookup"><span data-stu-id="f205b-132">attendees</span></span>|[<span data-ttu-id="f205b-133">Attendee</span><span class="sxs-lookup"><span data-stu-id="f205b-133">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="f205b-134">イベントの参加者のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f205b-134">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="f205b-135">body</span><span class="sxs-lookup"><span data-stu-id="f205b-135">body</span></span>|[<span data-ttu-id="f205b-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="f205b-136">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="f205b-137">イベントに関連付けられたメッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="f205b-137">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="f205b-138">categories</span><span class="sxs-lookup"><span data-stu-id="f205b-138">categories</span></span>|<span data-ttu-id="f205b-139">String</span><span class="sxs-lookup"><span data-stu-id="f205b-139">String</span></span>|<span data-ttu-id="f205b-140">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="f205b-140">The categories associated with the event.</span></span>|
|<span data-ttu-id="f205b-141">end</span><span class="sxs-lookup"><span data-stu-id="f205b-141">end</span></span>|[<span data-ttu-id="f205b-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f205b-142">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="f205b-143">イベントが終了する日時。</span><span class="sxs-lookup"><span data-stu-id="f205b-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="f205b-p104">既定で、終了時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで終了時刻を表現し、UTC からの時間オフセットを含めることができます。EndTimeZone を使用する場合、StartTimeZone の値も指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f205b-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="f205b-147">この例では、太平洋標準時で 2015 年 2 月 25 日午後 9:34 を指定します ("2015-02-25T21:34:00-08:00")。</span><span class="sxs-lookup"><span data-stu-id="f205b-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="f205b-148">importance</span><span class="sxs-lookup"><span data-stu-id="f205b-148">importance</span></span>|<span data-ttu-id="f205b-149">String</span><span class="sxs-lookup"><span data-stu-id="f205b-149">String</span></span>|<span data-ttu-id="f205b-150">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="f205b-150">The importance of the event.</span></span> <span data-ttu-id="f205b-151">可能な値: `low`、 `normal`、 `high`。</span><span class="sxs-lookup"><span data-stu-id="f205b-151">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="f205b-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="f205b-152">isAllDay</span></span>|<span data-ttu-id="f205b-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="f205b-153">Boolean</span></span>|<span data-ttu-id="f205b-154">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="f205b-154">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="f205b-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="f205b-155">isReminderOn</span></span>|<span data-ttu-id="f205b-156">ブール値</span><span class="sxs-lookup"><span data-stu-id="f205b-156">Boolean</span></span>|<span data-ttu-id="f205b-157">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="f205b-157">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="f205b-158">location</span><span class="sxs-lookup"><span data-stu-id="f205b-158">location</span></span>|[<span data-ttu-id="f205b-159">Location</span><span class="sxs-lookup"><span data-stu-id="f205b-159">Location</span></span>](../resources/location.md)|<span data-ttu-id="f205b-160">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="f205b-160">The location of the event.</span></span>|
|<span data-ttu-id="f205b-161">locations</span><span class="sxs-lookup"><span data-stu-id="f205b-161">locations</span></span>|<span data-ttu-id="f205b-162">[location](../resources/location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f205b-162">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="f205b-163">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="f205b-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="f205b-164">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="f205b-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="f205b-165">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="f205b-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="f205b-166">recurrence</span><span class="sxs-lookup"><span data-stu-id="f205b-166">recurrence</span></span>|[<span data-ttu-id="f205b-167">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f205b-167">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="f205b-168">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="f205b-168">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="f205b-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="f205b-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="f205b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f205b-170">Int32</span></span>|<span data-ttu-id="f205b-171">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="f205b-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="f205b-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="f205b-172">responseRequested</span></span>|<span data-ttu-id="f205b-173">ブール値</span><span class="sxs-lookup"><span data-stu-id="f205b-173">Boolean</span></span>|<span data-ttu-id="f205b-174">イベントが承諾または辞退されたときに、送信者が応答を要求する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="f205b-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="f205b-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="f205b-175">sensitivity</span></span>|<span data-ttu-id="f205b-176">String</span><span class="sxs-lookup"><span data-stu-id="f205b-176">String</span></span>| <span data-ttu-id="f205b-177">可能な値: `normal`、 `personal`、 `private`、 `confidential`。</span><span class="sxs-lookup"><span data-stu-id="f205b-177">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="f205b-178">showAs</span><span class="sxs-lookup"><span data-stu-id="f205b-178">showAs</span></span>|<span data-ttu-id="f205b-179">String</span><span class="sxs-lookup"><span data-stu-id="f205b-179">String</span></span>|<span data-ttu-id="f205b-180">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="f205b-180">The status to show.</span></span> <span data-ttu-id="f205b-181">可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="f205b-181">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="f205b-182">開始</span><span class="sxs-lookup"><span data-stu-id="f205b-182">start</span></span>|[<span data-ttu-id="f205b-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f205b-183">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="f205b-184">イベントの開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="f205b-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="f205b-p108">既定で、開始時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで開始時刻を表現し、UTC からの時間オフセットを含めることができます。StartTimeZone を使用する場合、EndTimeZone の値も指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f205b-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="f205b-188">この例では、太平洋標準時で 2015 年 2 月 25 日午後 7:34 を指定します "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="f205b-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="f205b-189">subject</span><span class="sxs-lookup"><span data-stu-id="f205b-189">subject</span></span>|<span data-ttu-id="f205b-190">String</span><span class="sxs-lookup"><span data-stu-id="f205b-190">String</span></span>|<span data-ttu-id="f205b-191">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="f205b-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="f205b-192">**イベント**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、使用して、`PATCH`を追加、更新、または既存の**イベント**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="f205b-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="f205b-193">更新する**イベント**がマスターし、定期的な一連のイベントの場合は、複数の出席者が含まれていて、個別に更新されたインスタンス、複数の通知の電子メールが送信されます: マスターのシリーズとは、インスタンスごとに 1 つのいずれか更新されました。</span><span class="sxs-lookup"><span data-stu-id="f205b-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="f205b-194">応答</span><span class="sxs-lookup"><span data-stu-id="f205b-194">Response</span></span>

<span data-ttu-id="f205b-195">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [event](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f205b-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="f205b-196">**注:** このメソッドは、HTTP 400 正しくない要求を含む応答のエラー コードを返すことができます`ErrorOccurrenceCrossingBoundary`し、次のエラー メッセージ: 変更されたアイテムを越えるまたは隣接するアイテムが重複しています。</span><span class="sxs-lookup"><span data-stu-id="f205b-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="f205b-197">更新プログラムには、定期的なアイテムの例外では、以下の Outlook 制限が違反していることを示します: 発生または日の前の出現箇所では、前日に移動することはできませんし、出現する位置は、次の日の前後に移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="f205b-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="f205b-198">例</span><span class="sxs-lookup"><span data-stu-id="f205b-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f205b-199">要求</span><span class="sxs-lookup"><span data-stu-id="f205b-199">Request</span></span>

<span data-ttu-id="f205b-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f205b-200">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

##### <a name="response"></a><span data-ttu-id="f205b-201">応答</span><span class="sxs-lookup"><span data-stu-id="f205b-201">Response</span></span>

<span data-ttu-id="f205b-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f205b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "time": "datetime-value"
  },
  "recurrence": null,  
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

## <a name="see-also"></a><span data-ttu-id="f205b-205">関連項目</span><span class="sxs-lookup"><span data-stu-id="f205b-205">See also</span></span>

- [<span data-ttu-id="f205b-206">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="f205b-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f205b-207">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="f205b-207">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f205b-208">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="f205b-208">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
