# <a name="update-event"></a><span data-ttu-id="fd957-101">イベントの更新</span><span class="sxs-lookup"><span data-stu-id="fd957-101">Update event</span></span>

<span data-ttu-id="fd957-102">イベント オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fd957-102">Update the properties of event object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd957-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd957-103">Permissions</span></span>
<span data-ttu-id="fd957-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd957-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd957-106">Permission type</span></span>      | <span data-ttu-id="fd957-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd957-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd957-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd957-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fd957-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd957-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fd957-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd957-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd957-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd957-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fd957-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd957-112">Application</span></span> | <span data-ttu-id="fd957-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd957-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd957-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd957-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="fd957-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd957-115">Request headers</span></span>
| <span data-ttu-id="fd957-116">名前</span><span class="sxs-lookup"><span data-stu-id="fd957-116">Name</span></span>       | <span data-ttu-id="fd957-117">型</span><span class="sxs-lookup"><span data-stu-id="fd957-117">Type</span></span> | <span data-ttu-id="fd957-118">説明</span><span class="sxs-lookup"><span data-stu-id="fd957-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fd957-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd957-119">Authorization</span></span>  | <span data-ttu-id="fd957-120">string</span><span class="sxs-lookup"><span data-stu-id="fd957-120">string</span></span>  | <span data-ttu-id="fd957-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fd957-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd957-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd957-123">Request body</span></span>
<span data-ttu-id="fd957-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="fd957-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fd957-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd957-127">Property</span></span>     | <span data-ttu-id="fd957-128">型</span><span class="sxs-lookup"><span data-stu-id="fd957-128">Type</span></span>   |<span data-ttu-id="fd957-129">説明</span><span class="sxs-lookup"><span data-stu-id="fd957-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd957-130">attendees</span><span class="sxs-lookup"><span data-stu-id="fd957-130">attendees</span></span>|[<span data-ttu-id="fd957-131">Attendee</span><span class="sxs-lookup"><span data-stu-id="fd957-131">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="fd957-132">イベントの参加者のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="fd957-132">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="fd957-133">body</span><span class="sxs-lookup"><span data-stu-id="fd957-133">body</span></span>|[<span data-ttu-id="fd957-134">ItemBody</span><span class="sxs-lookup"><span data-stu-id="fd957-134">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="fd957-135">イベントに関連付けられたメッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="fd957-135">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="fd957-136">categories</span><span class="sxs-lookup"><span data-stu-id="fd957-136">categories</span></span>|<span data-ttu-id="fd957-137">String</span><span class="sxs-lookup"><span data-stu-id="fd957-137">String</span></span>|<span data-ttu-id="fd957-138">イベントに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="fd957-138">The categories associated with the event.</span></span>|
|<span data-ttu-id="fd957-139">end</span><span class="sxs-lookup"><span data-stu-id="fd957-139">end</span></span>|[<span data-ttu-id="fd957-140">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fd957-140">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="fd957-141">イベントが終了する日時。</span><span class="sxs-lookup"><span data-stu-id="fd957-141">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="fd957-p104">既定で、終了時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで終了時刻を表現し、UTC からの時間オフセットを含めることができます。EndTimeZone を使用する場合、StartTimeZone の値も指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd957-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="fd957-145">この例では、太平洋標準時で 2015 年 2 月 25 日午後 9:34 を指定します ("2015-02-25T21:34:00-08:00")。</span><span class="sxs-lookup"><span data-stu-id="fd957-145">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="fd957-146">importance</span><span class="sxs-lookup"><span data-stu-id="fd957-146">importance</span></span>|<span data-ttu-id="fd957-147">String</span><span class="sxs-lookup"><span data-stu-id="fd957-147">String</span></span>|<span data-ttu-id="fd957-148">イベントの重要度。</span><span class="sxs-lookup"><span data-stu-id="fd957-148">The importance of the event.</span></span> <span data-ttu-id="fd957-149">可能な値は `low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="fd957-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="fd957-150">isAllDay</span><span class="sxs-lookup"><span data-stu-id="fd957-150">isAllDay</span></span>|<span data-ttu-id="fd957-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd957-151">Boolean</span></span>|<span data-ttu-id="fd957-152">イベントが一日中続く場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="fd957-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="fd957-153">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="fd957-153">isReminderOn</span></span>|<span data-ttu-id="fd957-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd957-154">Boolean</span></span>|<span data-ttu-id="fd957-155">ユーザーにイベントを通知するアラートを設定する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="fd957-155">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="fd957-156">location</span><span class="sxs-lookup"><span data-stu-id="fd957-156">location</span></span>|[<span data-ttu-id="fd957-157">Location</span><span class="sxs-lookup"><span data-stu-id="fd957-157">Location</span></span>](../resources/location.md)|<span data-ttu-id="fd957-158">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="fd957-158">The location of the event.</span></span>|
|<span data-ttu-id="fd957-159">locations</span><span class="sxs-lookup"><span data-stu-id="fd957-159">locations</span></span>|<span data-ttu-id="fd957-160">[location](../resources/location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fd957-160">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="fd957-161">イベントを開催する場所、または参加者がいる場所。</span><span class="sxs-lookup"><span data-stu-id="fd957-161">The locations where the event is held or attended from.</span></span> <span data-ttu-id="fd957-162">**location** プロパティと **locations** プロパティは常に互いに一致します。</span><span class="sxs-lookup"><span data-stu-id="fd957-162">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="fd957-163">**location** プロパティを更新すると、**locations** コレクションに含まれる既存のすべての場所が削除されて、**location** の新しい値に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="fd957-163">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="fd957-164">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="fd957-164">onlineMeetingUrl</span></span>|<span data-ttu-id="fd957-165">String</span><span class="sxs-lookup"><span data-stu-id="fd957-165">String</span></span>|<span data-ttu-id="fd957-166">オンライン会議の URL。</span><span class="sxs-lookup"><span data-stu-id="fd957-166">A URL for an online meeting.</span></span>|
|<span data-ttu-id="fd957-167">recurrence</span><span class="sxs-lookup"><span data-stu-id="fd957-167">recurrence</span></span>|[<span data-ttu-id="fd957-168">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="fd957-168">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="fd957-169">イベントの繰り返しパターン。</span><span class="sxs-lookup"><span data-stu-id="fd957-169">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="fd957-170">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="fd957-170">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="fd957-171">Int32</span><span class="sxs-lookup"><span data-stu-id="fd957-171">Int32</span></span>|<span data-ttu-id="fd957-172">アラーム通知を行う、イベント開始時間前の分数。</span><span class="sxs-lookup"><span data-stu-id="fd957-172">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="fd957-173">responseRequested</span><span class="sxs-lookup"><span data-stu-id="fd957-173">responseRequested</span></span>|<span data-ttu-id="fd957-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd957-174">Boolean</span></span>|<span data-ttu-id="fd957-175">イベントが承諾または辞退されたときに、送信者が応答を要求する場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="fd957-175">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="fd957-176">sensitivity</span><span class="sxs-lookup"><span data-stu-id="fd957-176">sensitivity</span></span>|<span data-ttu-id="fd957-177">String</span><span class="sxs-lookup"><span data-stu-id="fd957-177">String</span></span>| <span data-ttu-id="fd957-178">可能な値は、`normal`、`personal`、`private`、`confidential` です。</span><span class="sxs-lookup"><span data-stu-id="fd957-178">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="fd957-179">showAs</span><span class="sxs-lookup"><span data-stu-id="fd957-179">showAs</span></span>|<span data-ttu-id="fd957-180">String</span><span class="sxs-lookup"><span data-stu-id="fd957-180">String</span></span>|<span data-ttu-id="fd957-181">表示するステータス。</span><span class="sxs-lookup"><span data-stu-id="fd957-181">The status to show.</span></span> <span data-ttu-id="fd957-182">使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="fd957-182">Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="fd957-183">開始</span><span class="sxs-lookup"><span data-stu-id="fd957-183">start</span></span>|[<span data-ttu-id="fd957-184">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fd957-184">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="fd957-185">イベントの開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="fd957-185">The start time of the event.</span></span> <br/><br/><span data-ttu-id="fd957-p108">既定で、開始時刻は UTC 単位です。EndTimeZone でオプションのタイム ゾーンを指定して、そのタイム ゾーンで開始時刻を表現し、UTC からの時間オフセットを含めることができます。StartTimeZone を使用する場合、EndTimeZone の値も指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd957-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="fd957-189">この例では、太平洋標準時で 2015 年 2 月 25 日午後 7:34 を指定します "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="fd957-189">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="fd957-190">subject</span><span class="sxs-lookup"><span data-stu-id="fd957-190">subject</span></span>|<span data-ttu-id="fd957-191">String</span><span class="sxs-lookup"><span data-stu-id="fd957-191">String</span></span>|<span data-ttu-id="fd957-192">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="fd957-192">The text of the event's subject line.</span></span>|

<span data-ttu-id="fd957-193">**イベント** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`PATCH` 操作を使用して、既存の**イベント** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="fd957-193">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

## <a name="response"></a><span data-ttu-id="fd957-194">応答</span><span class="sxs-lookup"><span data-stu-id="fd957-194">Response</span></span>

<span data-ttu-id="fd957-195">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [event](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fd957-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd957-196">例</span><span class="sxs-lookup"><span data-stu-id="fd957-196">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fd957-197">要求</span><span class="sxs-lookup"><span data-stu-id="fd957-197">Request</span></span>

<span data-ttu-id="fd957-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fd957-198">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="fd957-199">応答</span><span class="sxs-lookup"><span data-stu-id="fd957-199">Response</span></span>

<span data-ttu-id="fd957-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fd957-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fd957-203">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd957-203">See also</span></span>

- [<span data-ttu-id="fd957-204">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="fd957-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="fd957-205">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="fd957-205">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="fd957-206">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="fd957-206">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
