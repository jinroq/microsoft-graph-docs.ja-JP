# <a name="list-calendarview"></a><span data-ttu-id="caea0-101">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="caea0-101">List calendarView</span></span>

<span data-ttu-id="caea0-102">ユーザーの既定の予定表またはユーザーが所有する他の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="caea0-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="caea0-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="caea0-103">Prerequisites</span></span>
<span data-ttu-id="caea0-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Calendars.Read、Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="caea0-104">One of the following **scopes** is required to execute this API: *Calendars.Read; Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="caea0-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="caea0-105">HTTP request</span></span>

<span data-ttu-id="caea0-106">ユーザーの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="caea0-106">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="caea0-107">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="caea0-107">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="caea0-108">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="caea0-108">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="caea0-109">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="caea0-109">Query parameters</span></span>

<span data-ttu-id="caea0-110">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="caea0-110">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="caea0-111">パラメーター</span><span class="sxs-lookup"><span data-stu-id="caea0-111">Parameter</span></span>    | <span data-ttu-id="caea0-112">型</span><span class="sxs-lookup"><span data-stu-id="caea0-112">Type</span></span>   |<span data-ttu-id="caea0-113">説明</span><span class="sxs-lookup"><span data-stu-id="caea0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="caea0-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="caea0-114">startDateTime</span></span>|<span data-ttu-id="caea0-115">String</span><span class="sxs-lookup"><span data-stu-id="caea0-115">String</span></span>|<span data-ttu-id="caea0-p101">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="caea0-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="caea0-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="caea0-118">endDateTime</span></span>|<span data-ttu-id="caea0-119">文字列</span><span class="sxs-lookup"><span data-stu-id="caea0-119">String</span></span>|<span data-ttu-id="caea0-p102">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="caea0-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="caea0-122">また、このメソッドは応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="caea0-122">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="caea0-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="caea0-123">Request headers</span></span>
| <span data-ttu-id="caea0-124">名前</span><span class="sxs-lookup"><span data-stu-id="caea0-124">Name</span></span>       | <span data-ttu-id="caea0-125">型</span><span class="sxs-lookup"><span data-stu-id="caea0-125">Type</span></span> | <span data-ttu-id="caea0-126">説明</span><span class="sxs-lookup"><span data-stu-id="caea0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="caea0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="caea0-127">Authorization</span></span>  | <span data-ttu-id="caea0-128">string</span><span class="sxs-lookup"><span data-stu-id="caea0-128">string</span></span>  | <span data-ttu-id="caea0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="caea0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="caea0-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="caea0-131">Content-Type</span></span>   | <span data-ttu-id="caea0-132">string</span><span class="sxs-lookup"><span data-stu-id="caea0-132">string</span></span>  | <span data-ttu-id="caea0-133">application/json</span><span class="sxs-lookup"><span data-stu-id="caea0-133">application/json</span></span> | 
| <span data-ttu-id="caea0-134">Prefer</span><span class="sxs-lookup"><span data-stu-id="caea0-134">Prefer</span></span> | <span data-ttu-id="caea0-135">string</span><span class="sxs-lookup"><span data-stu-id="caea0-135">string</span></span> | <span data-ttu-id="caea0-p104">outlook.timezone="Eastern 標準時"です。省略可能。これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。指定されていない場合、応答は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="caea0-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="caea0-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="caea0-140">Request body</span></span>
<span data-ttu-id="caea0-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="caea0-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="caea0-142">応答</span><span class="sxs-lookup"><span data-stu-id="caea0-142">Response</span></span>

<span data-ttu-id="caea0-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="caea0-143">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="caea0-144">例</span><span class="sxs-lookup"><span data-stu-id="caea0-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="caea0-145">要求</span><span class="sxs-lookup"><span data-stu-id="caea0-145">Request</span></span>
<span data-ttu-id="caea0-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="caea0-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="caea0-147">応答</span><span class="sxs-lookup"><span data-stu-id="caea0-147">Response</span></span>
<span data-ttu-id="caea0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="caea0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "",
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
