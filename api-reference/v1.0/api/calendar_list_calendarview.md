# <a name="list-calendarview"></a><span data-ttu-id="7dc8e-101">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7dc8e-101">List calendarView</span></span>

<span data-ttu-id="7dc8e-102">ユーザーまたはグループの既定の予定表 `(../me/calendarview)` またはユーザーが所有する他の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dc8e-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="7dc8e-103">Prerequisites</span></span>
<span data-ttu-id="7dc8e-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="7dc8e-105">ユーザーの予定表のイベント:_Calendars.Read_ または _Calendars.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="7dc8e-105">Events in a user's calendar: _Calendars.Read_ or _Calendars.ReadWrite_</span></span>
* <span data-ttu-id="7dc8e-106">グループの予定表のイベント:_Group.Read.All_ または _Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="7dc8e-106">Events in a group calendar: _Group.Read.All_ or _Group.ReadWrite.All_</span></span>

## <a name="http-request"></a><span data-ttu-id="7dc8e-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7dc8e-107">HTTP request</span></span>

<span data-ttu-id="7dc8e-108">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-108">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="7dc8e-109">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-109">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="7dc8e-110">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-110">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="7dc8e-111">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7dc8e-111">Query parameters</span></span>

<span data-ttu-id="7dc8e-112">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-112">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="7dc8e-113">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7dc8e-113">Parameter</span></span>    | <span data-ttu-id="7dc8e-114">型</span><span class="sxs-lookup"><span data-stu-id="7dc8e-114">Type</span></span>   |<span data-ttu-id="7dc8e-115">説明</span><span class="sxs-lookup"><span data-stu-id="7dc8e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7dc8e-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7dc8e-116">startDateTime</span></span>|<span data-ttu-id="7dc8e-117">String</span><span class="sxs-lookup"><span data-stu-id="7dc8e-117">String</span></span>|<span data-ttu-id="7dc8e-p101">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="7dc8e-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7dc8e-120">endDateTime</span></span>|<span data-ttu-id="7dc8e-121">文字列</span><span class="sxs-lookup"><span data-stu-id="7dc8e-121">String</span></span>|<span data-ttu-id="7dc8e-p102">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="7dc8e-124">また、このメソッドは応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-124">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7dc8e-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dc8e-125">Request headers</span></span>
| <span data-ttu-id="7dc8e-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dc8e-126">Header</span></span>       | <span data-ttu-id="7dc8e-127">値</span><span class="sxs-lookup"><span data-stu-id="7dc8e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7dc8e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dc8e-128">Authorization</span></span>  | <span data-ttu-id="7dc8e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7dc8e-131">Prefer</span><span class="sxs-lookup"><span data-stu-id="7dc8e-131">Prefer</span></span>  | <span data-ttu-id="7dc8e-p104">outlook.timezone="Eastern 標準時"です。省略可能。これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。指定されていない場合、応答は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dc8e-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="7dc8e-136">Request body</span></span>
<span data-ttu-id="7dc8e-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dc8e-138">応答</span><span class="sxs-lookup"><span data-stu-id="7dc8e-138">Response</span></span>

<span data-ttu-id="7dc8e-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-139">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7dc8e-140">例</span><span class="sxs-lookup"><span data-stu-id="7dc8e-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7dc8e-141">要求</span><span class="sxs-lookup"><span data-stu-id="7dc8e-141">Request</span></span>
<span data-ttu-id="7dc8e-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="7dc8e-143">応答</span><span class="sxs-lookup"><span data-stu-id="7dc8e-143">Response</span></span>
<span data-ttu-id="7dc8e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7dc8e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
