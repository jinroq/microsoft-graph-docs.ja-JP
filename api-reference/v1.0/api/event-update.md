---
title: イベントを更新する
description: イベント オブジェクトのプロパティを更新する。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 91e91d9f749b0d3ea61e28eae1a1eb4ed7aa1696
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887207"
---
# <a name="update-event"></a><span data-ttu-id="4f355-103">イベントを更新する</span><span class="sxs-lookup"><span data-stu-id="4f355-103">Update event</span></span>

<span data-ttu-id="4f355-104">[イベント](../resources/event.md) オブジェクトのプロパティを更新する。</span><span class="sxs-lookup"><span data-stu-id="4f355-104">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="4f355-105">イベントの開始時刻または終了時刻のタイムゾーンを更新する際に、まず、[サポートされているタイム ゾーンを検索](outlookuser-supportedtimezones.md)して、ユーザーのメールボックス サーバー用に構成されているタイム ゾーンのみ設定されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="4f355-105">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4f355-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f355-106">Permissions</span></span>
<span data-ttu-id="4f355-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f355-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f355-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f355-109">Permission type</span></span>      | <span data-ttu-id="4f355-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f355-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f355-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f355-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f355-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f355-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4f355-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f355-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f355-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f355-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4f355-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f355-115">Application</span></span> | <span data-ttu-id="4f355-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f355-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f355-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f355-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="4f355-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f355-118">Request headers</span></span>
| <span data-ttu-id="4f355-119">名前</span><span class="sxs-lookup"><span data-stu-id="4f355-119">Name</span></span>       | <span data-ttu-id="4f355-120">型</span><span class="sxs-lookup"><span data-stu-id="4f355-120">Type</span></span> | <span data-ttu-id="4f355-121">説明</span><span class="sxs-lookup"><span data-stu-id="4f355-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f355-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f355-122">Authorization</span></span>  | <span data-ttu-id="4f355-123">string</span><span class="sxs-lookup"><span data-stu-id="4f355-123">string</span></span>  | <span data-ttu-id="4f355-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4f355-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f355-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f355-126">Request body</span></span>
<span data-ttu-id="4f355-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4f355-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4f355-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f355-130">Property</span></span>     | <span data-ttu-id="4f355-131">型</span><span class="sxs-lookup"><span data-stu-id="4f355-131">Type</span></span>   |<span data-ttu-id="4f355-132">説明</span><span class="sxs-lookup"><span data-stu-id="4f355-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f355-133">attendees</span><span class="sxs-lookup"><span data-stu-id="4f355-133">attendees</span></span>|[<span data-ttu-id="4f355-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="4f355-134">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="4f355-135">イベントの参加者のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4f355-135">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="4f355-136">body</span><span class="sxs-lookup"><span data-stu-id="4f355-136">body</span></span>|[<span data-ttu-id="4f355-137">ItemBody</span><span class="sxs-lookup"><span data-stu-id="4f355-137">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="4f355-138">イベントに関連付けられたメッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="4f355-138">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="4f355-139">categories</span><span class="sxs-lookup"><span data-stu-id="4f355-139">categories</span></span>|<span data-ttu-id="4f355-140">String</span><span class="sxs-lookup"><span data-stu-id="4f355-140">String</span></span>|<span data-ttu-id="4f355-141">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="4f355-141">The categories associated with the event.</span></span>|
| <span data-ttu-id="4f355-142">end</span><span class="sxs-lookup"><span data-stu-id="4f355-142">end</span></span>|<span data-ttu-id="4f355-143">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4f355-143">DateTimeTimeZone</span></span>|<span data-ttu-id="4f355-144">イベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="4f355-144">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="4f355-145">importance</span><span class="sxs-lookup"><span data-stu-id="4f355-145">importance</span></span>|<span data-ttu-id="4f355-146">String</span><span class="sxs-lookup"><span data-stu-id="4f355-146">String</span></span>|<span data-ttu-id="4f355-147">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="4f355-147">The importance of the event.</span></span> <span data-ttu-id="4f355-148">使用可能な値: `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="4f355-148">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="4f355-149">isAllDay</span><span class="sxs-lookup"><span data-stu-id="4f355-149">isAllDay</span></span>|<span data-ttu-id="4f355-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f355-150">Boolean</span></span>|<span data-ttu-id="4f355-151">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4f355-151">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="4f355-152">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="4f355-152">isReminderOn</span></span>|<span data-ttu-id="4f355-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f355-153">Boolean</span></span>|<span data-ttu-id="4f355-154">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4f355-154">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="4f355-155">location</span><span class="sxs-lookup"><span data-stu-id="4f355-155">location</span></span>|[<span data-ttu-id="4f355-156">Location</span><span class="sxs-lookup"><span data-stu-id="4f355-156">Location</span></span>](../resources/location.md)|<span data-ttu-id="4f355-157">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="4f355-157">The location of the event.</span></span>|
|<span data-ttu-id="4f355-158">locations</span><span class="sxs-lookup"><span data-stu-id="4f355-158">locations</span></span>|<span data-ttu-id="4f355-159">[location](../resources/location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4f355-159">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="4f355-160">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="4f355-160">The locations where the event is held or attended from.</span></span> <span data-ttu-id="4f355-161">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="4f355-161">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="4f355-162">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="4f355-162">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="4f355-163">recurrence</span><span class="sxs-lookup"><span data-stu-id="4f355-163">recurrence</span></span>|[<span data-ttu-id="4f355-164">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="4f355-164">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="4f355-165">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="4f355-165">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="4f355-166">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="4f355-166">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="4f355-167">Int32</span><span class="sxs-lookup"><span data-stu-id="4f355-167">Int32</span></span>|<span data-ttu-id="4f355-168">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="4f355-168">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="4f355-169">responseRequested</span><span class="sxs-lookup"><span data-stu-id="4f355-169">responseRequested</span></span>|<span data-ttu-id="4f355-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f355-170">Boolean</span></span>|<span data-ttu-id="4f355-171">イベントが承諾または辞退されたときに、送信者が応答を要求する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4f355-171">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="4f355-172">sensitivity</span><span class="sxs-lookup"><span data-stu-id="4f355-172">sensitivity</span></span>|<span data-ttu-id="4f355-173">String</span><span class="sxs-lookup"><span data-stu-id="4f355-173">String</span></span>| <span data-ttu-id="4f355-174">使用可能な値: `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="4f355-174">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="4f355-175">showAs</span><span class="sxs-lookup"><span data-stu-id="4f355-175">showAs</span></span>|<span data-ttu-id="4f355-176">String</span><span class="sxs-lookup"><span data-stu-id="4f355-176">String</span></span>|<span data-ttu-id="4f355-177">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="4f355-177">The status to show.</span></span> <span data-ttu-id="4f355-178">使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="4f355-178">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="4f355-179">開始</span><span class="sxs-lookup"><span data-stu-id="4f355-179">start</span></span>|<span data-ttu-id="4f355-180">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4f355-180">DateTimeTimeZone</span></span>|<span data-ttu-id="4f355-181">イベントの開始日、時間、タイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="4f355-181">The date, time, and time zone that the event starts.</span></span> |
|<span data-ttu-id="4f355-182">subject</span><span class="sxs-lookup"><span data-stu-id="4f355-182">subject</span></span>|<span data-ttu-id="4f355-183">String</span><span class="sxs-lookup"><span data-stu-id="4f355-183">String</span></span>|<span data-ttu-id="4f355-184">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="4f355-184">The text of the event's subject line.</span></span>|

<span data-ttu-id="4f355-185">**イベント** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**イベント** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="4f355-185">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="4f355-186">アップデートする**イベント**が複数の出席者が含まれる定期的で主要なイベントである場合、インスタンス別にそれぞれに更新され、主要な系列と更新された各インスタンスごとに複数の通知メールが送信されます。</span><span class="sxs-lookup"><span data-stu-id="4f355-186">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="4f355-187">応答</span><span class="sxs-lookup"><span data-stu-id="4f355-187">Response</span></span>

<span data-ttu-id="4f355-188">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [event](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4f355-188">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="4f355-189">**注:** この方法は、エラー コード`ErrorOccurrenceCrossingBoundary` で HTTP 400 無効な要求の応答を返すことができます。そして、次のエラー メッセージが表示されます: 変更したアイテムが、隣接するアイテムと交差または重複しています。</span><span class="sxs-lookup"><span data-stu-id="4f355-189">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="4f355-190">定期的な予定の例外にある Outlook の制限に更新プログラムが違反していることを次のように示します: 定期的な予定を移動させる、または前回の定期的な予定をその日付より前日または後日に移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="4f355-190">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="4f355-191">例</span><span class="sxs-lookup"><span data-stu-id="4f355-191">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4f355-192">要求</span><span class="sxs-lookup"><span data-stu-id="4f355-192">Request</span></span>

<span data-ttu-id="4f355-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4f355-193">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4f355-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f355-194">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f355-195">C#</span><span class="sxs-lookup"><span data-stu-id="4f355-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f355-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="4f355-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f355-197">Java</span><span class="sxs-lookup"><span data-stu-id="4f355-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f355-198">応答</span><span class="sxs-lookup"><span data-stu-id="4f355-198">Response</span></span>

<span data-ttu-id="4f355-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4f355-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4f355-202">関連項目</span><span class="sxs-lookup"><span data-stu-id="4f355-202">See also</span></span>

- [<span data-ttu-id="4f355-203">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="4f355-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4f355-204">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="4f355-204">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4f355-205">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="4f355-205">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
