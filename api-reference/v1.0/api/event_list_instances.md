# <a name="list-instances"></a><span data-ttu-id="ae1c8-101">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="ae1c8-101">List instances</span></span>

<span data-ttu-id="ae1c8-p101">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが`SeriesMaster`タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae1c8-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae1c8-104">Permissions</span></span>
<span data-ttu-id="ae1c8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae1c8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae1c8-107">Permission type</span></span>      | <span data-ttu-id="ae1c8-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae1c8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae1c8-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae1c8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ae1c8-110">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae1c8-110">Calendars.Read</span></span>    |
|<span data-ttu-id="ae1c8-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae1c8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae1c8-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae1c8-112">Calendars.Read</span></span>    |
|<span data-ttu-id="ae1c8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae1c8-113">Application</span></span> | <span data-ttu-id="ae1c8-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae1c8-114">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae1c8-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae1c8-115">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="ae1c8-116">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae1c8-116">Query parameters</span></span>

<span data-ttu-id="ae1c8-117">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ae1c8-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae1c8-118">Parameter</span></span>    | <span data-ttu-id="ae1c8-119">型</span><span class="sxs-lookup"><span data-stu-id="ae1c8-119">Type</span></span>   |<span data-ttu-id="ae1c8-120">説明</span><span class="sxs-lookup"><span data-stu-id="ae1c8-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae1c8-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ae1c8-121">startDateTime</span></span>|<span data-ttu-id="ae1c8-122">String</span><span class="sxs-lookup"><span data-stu-id="ae1c8-122">String</span></span>|<span data-ttu-id="ae1c8-p103">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ae1c8-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ae1c8-125">endDateTime</span></span>|<span data-ttu-id="ae1c8-126">String</span><span class="sxs-lookup"><span data-stu-id="ae1c8-126">String</span></span>|<span data-ttu-id="ae1c8-p104">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ae1c8-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-129">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae1c8-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae1c8-130">Request headers</span></span>
| <span data-ttu-id="ae1c8-131">名前</span><span class="sxs-lookup"><span data-stu-id="ae1c8-131">Name</span></span>       | <span data-ttu-id="ae1c8-132">型</span><span class="sxs-lookup"><span data-stu-id="ae1c8-132">Type</span></span> | <span data-ttu-id="ae1c8-133">説明</span><span class="sxs-lookup"><span data-stu-id="ae1c8-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae1c8-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae1c8-134">Authorization</span></span>  | <span data-ttu-id="ae1c8-135">string</span><span class="sxs-lookup"><span data-stu-id="ae1c8-135">string</span></span>  | <span data-ttu-id="ae1c8-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae1c8-138">Prefer</span><span class="sxs-lookup"><span data-stu-id="ae1c8-138">Prefer</span></span> | <span data-ttu-id="ae1c8-139">string</span><span class="sxs-lookup"><span data-stu-id="ae1c8-139">string</span></span> | <span data-ttu-id="ae1c8-p106">outlook.timezone="Eastern 標準時"です。省略可能。これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。指定されていない場合、応答は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-p106">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae1c8-144">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae1c8-144">Request body</span></span>
<span data-ttu-id="ae1c8-145">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae1c8-146">応答</span><span class="sxs-lookup"><span data-stu-id="ae1c8-146">Response</span></span>

<span data-ttu-id="ae1c8-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae1c8-148">例</span><span class="sxs-lookup"><span data-stu-id="ae1c8-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae1c8-149">要求</span><span class="sxs-lookup"><span data-stu-id="ae1c8-149">Request</span></span>
<span data-ttu-id="ae1c8-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="ae1c8-151">応答</span><span class="sxs-lookup"><span data-stu-id="ae1c8-151">Response</span></span>
<span data-ttu-id="ae1c8-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae1c8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
