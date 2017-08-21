# <a name="list-calendarview"></a><span data-ttu-id="5bce7-101">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5bce7-101">List calendarView</span></span>

<span data-ttu-id="5bce7-102">グループの既定の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="5bce7-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5bce7-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="5bce7-103">Prerequisites</span></span>
<span data-ttu-id="5bce7-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All* または *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="5bce7-104">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="5bce7-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bce7-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="5bce7-106">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5bce7-106">Query parameters</span></span>

<span data-ttu-id="5bce7-107">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="5bce7-107">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="5bce7-108">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5bce7-108">Parameter</span></span>    | <span data-ttu-id="5bce7-109">型</span><span class="sxs-lookup"><span data-stu-id="5bce7-109">Type</span></span>   |<span data-ttu-id="5bce7-110">説明</span><span class="sxs-lookup"><span data-stu-id="5bce7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bce7-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5bce7-111">startDateTime</span></span>|<span data-ttu-id="5bce7-112">String</span><span class="sxs-lookup"><span data-stu-id="5bce7-112">String</span></span>|<span data-ttu-id="5bce7-p101">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="5bce7-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="5bce7-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5bce7-115">endDateTime</span></span>|<span data-ttu-id="5bce7-116">文字列</span><span class="sxs-lookup"><span data-stu-id="5bce7-116">String</span></span>|<span data-ttu-id="5bce7-p102">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="5bce7-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="5bce7-119">また、このメソッドは応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="5bce7-119">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5bce7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bce7-120">Request headers</span></span>
| <span data-ttu-id="5bce7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bce7-121">Header</span></span>       | <span data-ttu-id="5bce7-122">値</span><span class="sxs-lookup"><span data-stu-id="5bce7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5bce7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bce7-123">Authorization</span></span>  | <span data-ttu-id="5bce7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5bce7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5bce7-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="5bce7-126">Prefer</span></span> | <span data-ttu-id="5bce7-127">string</span><span class="sxs-lookup"><span data-stu-id="5bce7-127">string</span></span> | <span data-ttu-id="5bce7-p104">outlook.timezone="Eastern 標準時"です。省略可能。これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。指定されていない場合、応答は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="5bce7-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bce7-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bce7-132">Request body</span></span>
<span data-ttu-id="5bce7-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5bce7-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bce7-134">応答</span><span class="sxs-lookup"><span data-stu-id="5bce7-134">Response</span></span>

<span data-ttu-id="5bce7-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5bce7-135">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5bce7-136">例</span><span class="sxs-lookup"><span data-stu-id="5bce7-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bce7-137">要求</span><span class="sxs-lookup"><span data-stu-id="5bce7-137">Request</span></span>
<span data-ttu-id="5bce7-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5bce7-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="5bce7-139">応答</span><span class="sxs-lookup"><span data-stu-id="5bce7-139">Response</span></span>
<span data-ttu-id="5bce7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5bce7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
