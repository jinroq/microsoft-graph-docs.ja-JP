# <a name="list-instances"></a><span data-ttu-id="ca0e9-101">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="ca0e9-101">List instances</span></span>

<span data-ttu-id="ca0e9-p101">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが`SeriesMaster`タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca0e9-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ca0e9-104">Permissions</span></span>
<span data-ttu-id="ca0e9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ca0e9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca0e9-107">Permission type</span></span>      | <span data-ttu-id="ca0e9-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca0e9-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca0e9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca0e9-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ca0e9-110">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca0e9-110">Calendars.Read</span></span>    |
|<span data-ttu-id="ca0e9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca0e9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca0e9-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca0e9-112">Calendars.Read</span></span>    |
|<span data-ttu-id="ca0e9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca0e9-113">Application</span></span> | <span data-ttu-id="ca0e9-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca0e9-114">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca0e9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca0e9-115">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="ca0e9-116">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ca0e9-116">Query parameters</span></span>

<span data-ttu-id="ca0e9-117">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ca0e9-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ca0e9-118">Parameter</span></span>    | <span data-ttu-id="ca0e9-119">型</span><span class="sxs-lookup"><span data-stu-id="ca0e9-119">Type</span></span>   |<span data-ttu-id="ca0e9-120">説明</span><span class="sxs-lookup"><span data-stu-id="ca0e9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca0e9-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ca0e9-121">startDateTime</span></span>|<span data-ttu-id="ca0e9-122">String</span><span class="sxs-lookup"><span data-stu-id="ca0e9-122">String</span></span>|<span data-ttu-id="ca0e9-p103">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ca0e9-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ca0e9-125">endDateTime</span></span>|<span data-ttu-id="ca0e9-126">String</span><span class="sxs-lookup"><span data-stu-id="ca0e9-126">String</span></span>|<span data-ttu-id="ca0e9-p104">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ca0e9-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ca0e9-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca0e9-130">Request headers</span></span>
| <span data-ttu-id="ca0e9-131">名前</span><span class="sxs-lookup"><span data-stu-id="ca0e9-131">Name</span></span>       | <span data-ttu-id="ca0e9-132">型</span><span class="sxs-lookup"><span data-stu-id="ca0e9-132">Type</span></span> | <span data-ttu-id="ca0e9-133">説明</span><span class="sxs-lookup"><span data-stu-id="ca0e9-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ca0e9-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca0e9-134">Authorization</span></span>  | <span data-ttu-id="ca0e9-135">string</span><span class="sxs-lookup"><span data-stu-id="ca0e9-135">string</span></span> | <span data-ttu-id="ca0e9-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ca0e9-138">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ca0e9-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ca0e9-139">string</span><span class="sxs-lookup"><span data-stu-id="ca0e9-139">string</span></span> | <span data-ttu-id="ca0e9-140">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ca0e9-141">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ca0e9-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca0e9-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca0e9-143">Request body</span></span>
<span data-ttu-id="ca0e9-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca0e9-145">応答</span><span class="sxs-lookup"><span data-stu-id="ca0e9-145">Response</span></span>

<span data-ttu-id="ca0e9-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca0e9-147">例</span><span class="sxs-lookup"><span data-stu-id="ca0e9-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca0e9-148">要求</span><span class="sxs-lookup"><span data-stu-id="ca0e9-148">Request</span></span>
<span data-ttu-id="ca0e9-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="ca0e9-150">応答</span><span class="sxs-lookup"><span data-stu-id="ca0e9-150">Response</span></span>
<span data-ttu-id="ca0e9-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca0e9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
