---
title: イベントを更新する
description: イベント オブジェクトのプロパティを更新する。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 911f15257ce10e628cb63db2ca4ee9517b5cbe81
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440940"
---
# <a name="update-event"></a><span data-ttu-id="59b61-103">イベントを更新する</span><span class="sxs-lookup"><span data-stu-id="59b61-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59b61-104">[イベント](../resources/event.md) オブジェクトのプロパティを更新する。</span><span class="sxs-lookup"><span data-stu-id="59b61-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="59b61-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59b61-105">Permissions</span></span>
<span data-ttu-id="59b61-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59b61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59b61-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59b61-108">Permission type</span></span>      | <span data-ttu-id="59b61-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59b61-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59b61-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59b61-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59b61-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59b61-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="59b61-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59b61-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59b61-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59b61-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="59b61-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59b61-114">Application</span></span> | <span data-ttu-id="59b61-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59b61-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59b61-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59b61-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="59b61-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59b61-117">Request headers</span></span>
| <span data-ttu-id="59b61-118">名前</span><span class="sxs-lookup"><span data-stu-id="59b61-118">Name</span></span>       | <span data-ttu-id="59b61-119">型</span><span class="sxs-lookup"><span data-stu-id="59b61-119">Type</span></span> | <span data-ttu-id="59b61-120">説明</span><span class="sxs-lookup"><span data-stu-id="59b61-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59b61-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="59b61-121">Authorization</span></span>  | <span data-ttu-id="59b61-122">string</span><span class="sxs-lookup"><span data-stu-id="59b61-122">string</span></span>  | <span data-ttu-id="59b61-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59b61-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59b61-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="59b61-125">Request body</span></span>
<span data-ttu-id="59b61-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="59b61-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59b61-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59b61-129">Property</span></span>       | <span data-ttu-id="59b61-130">型</span><span class="sxs-lookup"><span data-stu-id="59b61-130">Type</span></span>    | <span data-ttu-id="59b61-131">説明</span><span class="sxs-lookup"><span data-stu-id="59b61-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="59b61-132">attendees</span><span class="sxs-lookup"><span data-stu-id="59b61-132">attendees</span></span>|<span data-ttu-id="59b61-133">参加者</span><span class="sxs-lookup"><span data-stu-id="59b61-133">Attendee</span></span>|<span data-ttu-id="59b61-134">イベントの参加者のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="59b61-134">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="59b61-135">body</span><span class="sxs-lookup"><span data-stu-id="59b61-135">body</span></span>|<span data-ttu-id="59b61-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="59b61-136">ItemBody</span></span>|<span data-ttu-id="59b61-137">イベントに関連付けられたメッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="59b61-137">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="59b61-138">categories</span><span class="sxs-lookup"><span data-stu-id="59b61-138">categories</span></span>|<span data-ttu-id="59b61-139">String</span><span class="sxs-lookup"><span data-stu-id="59b61-139">String</span></span>|<span data-ttu-id="59b61-140">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="59b61-140">The categories associated with the event.</span></span>|
| <span data-ttu-id="59b61-141">end</span><span class="sxs-lookup"><span data-stu-id="59b61-141">end</span></span>|<span data-ttu-id="59b61-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="59b61-142">DateTimeTimeZone</span></span>|<span data-ttu-id="59b61-143">イベントが終了する日時。</span><span class="sxs-lookup"><span data-stu-id="59b61-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="59b61-p104">既定で、終了時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで終了時刻を表現し、UTC からの時間オフセットを含めることができます。EndTimeZone を使用する場合、StartTimeZone の値も指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="59b61-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="59b61-147">この例では、太平洋標準時で 2015 年 2 月 25 日午後 9:34 を指定します ("2015-02-25T21:34:00-08:00")。</span><span class="sxs-lookup"><span data-stu-id="59b61-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="59b61-148">importance</span><span class="sxs-lookup"><span data-stu-id="59b61-148">importance</span></span>|<span data-ttu-id="59b61-149">String</span><span class="sxs-lookup"><span data-stu-id="59b61-149">String</span></span>|<span data-ttu-id="59b61-150">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="59b61-150">The importance of the event.</span></span> <span data-ttu-id="59b61-151">可能な値は `low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="59b61-151">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="59b61-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="59b61-152">isAllDay</span></span>|<span data-ttu-id="59b61-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="59b61-153">Boolean</span></span>|<span data-ttu-id="59b61-154">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="59b61-154">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="59b61-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="59b61-155">isReminderOn</span></span>|<span data-ttu-id="59b61-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="59b61-156">Boolean</span></span>|<span data-ttu-id="59b61-157">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="59b61-157">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="59b61-158">location</span><span class="sxs-lookup"><span data-stu-id="59b61-158">location</span></span>|<span data-ttu-id="59b61-159">場所</span><span class="sxs-lookup"><span data-stu-id="59b61-159">Location</span></span>|<span data-ttu-id="59b61-160">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="59b61-160">The location of the event.</span></span>|
|<span data-ttu-id="59b61-161">locations</span><span class="sxs-lookup"><span data-stu-id="59b61-161">locations</span></span>|<span data-ttu-id="59b61-162">[Location](../resources/location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="59b61-162">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="59b61-163">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="59b61-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="59b61-164">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="59b61-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="59b61-165">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="59b61-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="59b61-166">recurrence</span><span class="sxs-lookup"><span data-stu-id="59b61-166">recurrence</span></span>|<span data-ttu-id="59b61-167">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="59b61-167">PatternedRecurrence</span></span>|<span data-ttu-id="59b61-168">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="59b61-168">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="59b61-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="59b61-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="59b61-170">Int32</span><span class="sxs-lookup"><span data-stu-id="59b61-170">Int32</span></span>|<span data-ttu-id="59b61-171">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="59b61-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="59b61-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="59b61-172">responseRequested</span></span>|<span data-ttu-id="59b61-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="59b61-173">Boolean</span></span>|<span data-ttu-id="59b61-174">イベントが承諾または辞退されたときに、送信者が応答を要求する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="59b61-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="59b61-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="59b61-175">sensitivity</span></span>|<span data-ttu-id="59b61-176">String</span><span class="sxs-lookup"><span data-stu-id="59b61-176">String</span></span>| <span data-ttu-id="59b61-177">使用可能な値: `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="59b61-177">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="59b61-178">showAs</span><span class="sxs-lookup"><span data-stu-id="59b61-178">showAs</span></span>|<span data-ttu-id="59b61-179">String</span><span class="sxs-lookup"><span data-stu-id="59b61-179">String</span></span>|<span data-ttu-id="59b61-180">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="59b61-180">The status to show.</span></span> <span data-ttu-id="59b61-181">可能な値は`free` 、 `tentative`、 `busy` `oof` `workingElsewhere`、、、 `unknown`、です。</span><span class="sxs-lookup"><span data-stu-id="59b61-181">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="59b61-182">開始</span><span class="sxs-lookup"><span data-stu-id="59b61-182">start</span></span>|<span data-ttu-id="59b61-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="59b61-183">DateTimeTimeZone</span></span>|<span data-ttu-id="59b61-184">イベントの開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="59b61-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="59b61-p108">既定で、開始時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで開始時刻を表現し、UTC からの時間オフセットを含めることができます。StartTimeZone を使用する場合、EndTimeZone の値も指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="59b61-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="59b61-188">この例では、太平洋標準時で 2015 年 2 月 25 日午後 7:34 を指定します "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="59b61-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="59b61-189">subject</span><span class="sxs-lookup"><span data-stu-id="59b61-189">subject</span></span>|<span data-ttu-id="59b61-190">String</span><span class="sxs-lookup"><span data-stu-id="59b61-190">String</span></span>|<span data-ttu-id="59b61-191">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="59b61-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="59b61-192">**イベント** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**イベント** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="59b61-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="59b61-193">アップデートする**イベント**が複数の出席者が含まれる定期的で主要なイベントである場合、インスタンス別にそれぞれに更新され、主要な系列と更新された各インスタンスごとに複数の通知メールが送信されます。</span><span class="sxs-lookup"><span data-stu-id="59b61-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="59b61-194">応答</span><span class="sxs-lookup"><span data-stu-id="59b61-194">Response</span></span>

<span data-ttu-id="59b61-195">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [event](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="59b61-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="59b61-196">**注:** この方法は、エラー コード`ErrorOccurrenceCrossingBoundary` で HTTP 400 無効な要求の応答を返すことができます。そして、次のエラー メッセージが表示されます: 変更したアイテムが、隣接するアイテムと交差または重複しています。</span><span class="sxs-lookup"><span data-stu-id="59b61-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="59b61-197">定期的な予定の例外にある Outlook の制限に更新プログラムが違反していることを次のように示します: 定期的な予定を移動させる、または前回の定期的な予定をその日付より前日または後日に移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="59b61-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="59b61-198">例</span><span class="sxs-lookup"><span data-stu-id="59b61-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="59b61-199">要求</span><span class="sxs-lookup"><span data-stu-id="59b61-199">Request</span></span>

<span data-ttu-id="59b61-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="59b61-200">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59b61-201">プロトコル</span><span class="sxs-lookup"><span data-stu-id="59b61-201">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="59b61-202">C#</span><span class="sxs-lookup"><span data-stu-id="59b61-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59b61-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="59b61-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59b61-204">応答</span><span class="sxs-lookup"><span data-stu-id="59b61-204">Response</span></span>
<span data-ttu-id="59b61-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="59b61-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="59b61-208">関連項目</span><span class="sxs-lookup"><span data-stu-id="59b61-208">See also</span></span>

- [<span data-ttu-id="59b61-209">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="59b61-209">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="59b61-210">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="59b61-210">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="59b61-211">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="59b61-211">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
