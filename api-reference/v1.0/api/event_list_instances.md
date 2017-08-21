# <a name="list-instances"></a><span data-ttu-id="3b08e-101">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="3b08e-101">List instances</span></span>

<span data-ttu-id="3b08e-p101">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが`SeriesMaster`タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="3b08e-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b08e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="3b08e-104">Prerequisites</span></span>
<span data-ttu-id="3b08e-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Calendars.Read*</span><span class="sxs-lookup"><span data-stu-id="3b08e-105">One of the following **scopes** is required to execute this API: *Calendars.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="3b08e-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b08e-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="3b08e-107">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3b08e-107">Query parameters</span></span>

<span data-ttu-id="3b08e-108">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="3b08e-108">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="3b08e-109">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3b08e-109">Parameter</span></span>    | <span data-ttu-id="3b08e-110">型</span><span class="sxs-lookup"><span data-stu-id="3b08e-110">Type</span></span>   |<span data-ttu-id="3b08e-111">説明</span><span class="sxs-lookup"><span data-stu-id="3b08e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b08e-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3b08e-112">startDateTime</span></span>|<span data-ttu-id="3b08e-113">String</span><span class="sxs-lookup"><span data-stu-id="3b08e-113">String</span></span>|<span data-ttu-id="3b08e-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="3b08e-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="3b08e-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3b08e-116">endDateTime</span></span>|<span data-ttu-id="3b08e-117">文字列</span><span class="sxs-lookup"><span data-stu-id="3b08e-117">String</span></span>|<span data-ttu-id="3b08e-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="3b08e-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="3b08e-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3b08e-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3b08e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b08e-121">Request headers</span></span>
| <span data-ttu-id="3b08e-122">名前</span><span class="sxs-lookup"><span data-stu-id="3b08e-122">Name</span></span>       | <span data-ttu-id="3b08e-123">型</span><span class="sxs-lookup"><span data-stu-id="3b08e-123">Type</span></span> | <span data-ttu-id="3b08e-124">説明</span><span class="sxs-lookup"><span data-stu-id="3b08e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b08e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b08e-125">Authorization</span></span>  | <span data-ttu-id="3b08e-126">string</span><span class="sxs-lookup"><span data-stu-id="3b08e-126">string</span></span>  | <span data-ttu-id="3b08e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b08e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b08e-129">Prefer</span><span class="sxs-lookup"><span data-stu-id="3b08e-129">Prefer</span></span> | <span data-ttu-id="3b08e-130">string</span><span class="sxs-lookup"><span data-stu-id="3b08e-130">string</span></span> | <span data-ttu-id="3b08e-p105">outlook.timezone="Eastern 標準時"です。省略可能。これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。指定されていない場合、応答は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="3b08e-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b08e-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b08e-135">Request body</span></span>
<span data-ttu-id="3b08e-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b08e-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b08e-137">応答</span><span class="sxs-lookup"><span data-stu-id="3b08e-137">Response</span></span>

<span data-ttu-id="3b08e-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3b08e-138">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b08e-139">例</span><span class="sxs-lookup"><span data-stu-id="3b08e-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b08e-140">要求</span><span class="sxs-lookup"><span data-stu-id="3b08e-140">Request</span></span>
<span data-ttu-id="3b08e-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3b08e-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="3b08e-142">応答</span><span class="sxs-lookup"><span data-stu-id="3b08e-142">Response</span></span>
<span data-ttu-id="3b08e-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b08e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
