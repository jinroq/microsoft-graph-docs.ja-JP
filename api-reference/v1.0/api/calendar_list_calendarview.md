# <a name="list-calendarview"></a><span data-ttu-id="2a24c-101">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2a24c-101">List calendarView</span></span>

<span data-ttu-id="2a24c-102">ユーザーまたはグループの既定の予定表 `(../me/calendarview)` またはユーザーが所有する他の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="2a24c-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a24c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a24c-103">Permissions</span></span>
<span data-ttu-id="2a24c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="2a24c-106">ユーザーの予定表のイベント:Calendars.Read または Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a24c-106">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="2a24c-107">グループの予定表のイベント:Group.Read.All または Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a24c-107">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2a24c-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a24c-108">HTTP request</span></span>

<span data-ttu-id="2a24c-109">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2a24c-109">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="2a24c-110">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2a24c-110">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="2a24c-111">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2a24c-111">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="2a24c-112">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a24c-112">Query parameters</span></span>

<span data-ttu-id="2a24c-113">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="2a24c-113">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="2a24c-114">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a24c-114">Parameter</span></span>    | <span data-ttu-id="2a24c-115">型</span><span class="sxs-lookup"><span data-stu-id="2a24c-115">Type</span></span>   |<span data-ttu-id="2a24c-116">説明</span><span class="sxs-lookup"><span data-stu-id="2a24c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a24c-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2a24c-117">startDateTime</span></span>|<span data-ttu-id="2a24c-118">String</span><span class="sxs-lookup"><span data-stu-id="2a24c-118">String</span></span>|<span data-ttu-id="2a24c-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="2a24c-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="2a24c-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2a24c-121">endDateTime</span></span>|<span data-ttu-id="2a24c-122">String</span><span class="sxs-lookup"><span data-stu-id="2a24c-122">String</span></span>|<span data-ttu-id="2a24c-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="2a24c-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="2a24c-125">また、このメソッドは応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="2a24c-125">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2a24c-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a24c-126">Request headers</span></span>
| <span data-ttu-id="2a24c-127">名前</span><span class="sxs-lookup"><span data-stu-id="2a24c-127">Name</span></span>       | <span data-ttu-id="2a24c-128">型</span><span class="sxs-lookup"><span data-stu-id="2a24c-128">Type</span></span> | <span data-ttu-id="2a24c-129">説明</span><span class="sxs-lookup"><span data-stu-id="2a24c-129">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="2a24c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a24c-130">Authorization</span></span>  | <span data-ttu-id="2a24c-131">string</span><span class="sxs-lookup"><span data-stu-id="2a24c-131">string</span></span> | <span data-ttu-id="2a24c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a24c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2a24c-134">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2a24c-134">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="2a24c-135">string</span><span class="sxs-lookup"><span data-stu-id="2a24c-135">string</span></span> | <span data-ttu-id="2a24c-136">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a24c-136">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="2a24c-137">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="2a24c-137">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="2a24c-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2a24c-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a24c-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a24c-139">Request body</span></span>
<span data-ttu-id="2a24c-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a24c-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a24c-141">応答</span><span class="sxs-lookup"><span data-stu-id="2a24c-141">Response</span></span>

<span data-ttu-id="2a24c-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2a24c-142">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2a24c-143">例</span><span class="sxs-lookup"><span data-stu-id="2a24c-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a24c-144">要求</span><span class="sxs-lookup"><span data-stu-id="2a24c-144">Request</span></span>
<span data-ttu-id="2a24c-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a24c-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="2a24c-146">応答</span><span class="sxs-lookup"><span data-stu-id="2a24c-146">Response</span></span>
<span data-ttu-id="2a24c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a24c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
