# <a name="list-events"></a><span data-ttu-id="eeae6-101">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="eeae6-101">List events</span></span>

<span data-ttu-id="eeae6-p101">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eeae6-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="eeae6-104">拡張イベントのインスタンスを取得するには、[予定表ビューを取得する](calendar_list_calendarview.md)、または[イベントのインスタンスを取得する](event_list_instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

<span data-ttu-id="eeae6-105">現在、この操作によって返されるイベントの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="eeae6-105">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="eeae6-106">2 つシナリオは、アプリケーションが別のユーザーの予定表でイベントを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="eeae6-106">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="eeae6-107">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="eeae6-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="eeae6-108">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーとカレンダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="eeae6-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="eeae6-109">[詳細と例](../../../concepts/outlook-get-shared-events-calendars.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eeae6-109">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="eeae6-110">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="eeae6-110">Support various time zones</span></span>

<span data-ttu-id="eeae6-111">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-111">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="eeae6-112">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="eeae6-112">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="eeae6-p103">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="eeae6-116">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-116">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="eeae6-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eeae6-117">Permissions</span></span>
<span data-ttu-id="eeae6-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eeae6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eeae6-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eeae6-120">Permission type</span></span>      | <span data-ttu-id="eeae6-121">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eeae6-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeae6-122">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eeae6-122">Delegated (work or school account)</span></span> | <span data-ttu-id="eeae6-123">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeae6-123">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="eeae6-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eeae6-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeae6-125">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeae6-125">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="eeae6-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eeae6-126">Application</span></span> | <span data-ttu-id="eeae6-127">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeae6-127">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeae6-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eeae6-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eeae6-129">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eeae6-129">Optional query parameters</span></span>
<span data-ttu-id="eeae6-130">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="eeae6-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eeae6-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeae6-131">Request headers</span></span>
| <span data-ttu-id="eeae6-132">名前</span><span class="sxs-lookup"><span data-stu-id="eeae6-132">Name</span></span>       | <span data-ttu-id="eeae6-133">型</span><span class="sxs-lookup"><span data-stu-id="eeae6-133">Type</span></span> | <span data-ttu-id="eeae6-134">説明</span><span class="sxs-lookup"><span data-stu-id="eeae6-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="eeae6-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="eeae6-135">Authorization</span></span>  | <span data-ttu-id="eeae6-136">string</span><span class="sxs-lookup"><span data-stu-id="eeae6-136">string</span></span> | <span data-ttu-id="eeae6-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eeae6-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eeae6-139">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="eeae6-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="eeae6-140">文字列</span><span class="sxs-lookup"><span data-stu-id="eeae6-140">string</span></span> | <span data-ttu-id="eeae6-141">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="eeae6-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="eeae6-142">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="eeae6-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="eeae6-143">Optional.</span></span> |
| <span data-ttu-id="eeae6-144">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="eeae6-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="eeae6-145">文字列</span><span class="sxs-lookup"><span data-stu-id="eeae6-145">string</span></span> | <span data-ttu-id="eeae6-146">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="eeae6-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="eeae6-147">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="eeae6-147">Values can be "text" or "html".</span></span> <span data-ttu-id="eeae6-148">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="eeae6-149">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="eeae6-150">省略可能。</span><span class="sxs-lookup"><span data-stu-id="eeae6-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eeae6-151">要求本文</span><span class="sxs-lookup"><span data-stu-id="eeae6-151">Request body</span></span>
<span data-ttu-id="eeae6-152">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eeae6-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeae6-153">応答</span><span class="sxs-lookup"><span data-stu-id="eeae6-153">Response</span></span>

<span data-ttu-id="eeae6-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="eeae6-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eeae6-155">例</span><span class="sxs-lookup"><span data-stu-id="eeae6-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeae6-156">要求</span><span class="sxs-lookup"><span data-stu-id="eeae6-156">Request</span></span>
<span data-ttu-id="eeae6-p108">以下は、要求の例です。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="eeae6-p108">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="eeae6-159">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="eeae6-159">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="eeae6-p109">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターがない場合には、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="eeae6-162">応答</span><span class="sxs-lookup"><span data-stu-id="eeae6-162">Response</span></span>
<span data-ttu-id="eeae6-p110">以下は、応答の例です。**body** プロパティが既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="eeae6-p110">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1932

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"html",
                "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
            },
            "start":{
                "dateTime":"2017-04-21T10:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "end":{
                "dateTime":"2017-04-21T12:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "location": {
                "displayName": "Assembly Hall",
                "locationType": "default",
                "uniqueId": "Assembly Hall",
                "uniqueIdType": "private"
            },
            "locations": [
                {
                    "displayName": "Assembly Hall",
                    "locationType": "default",
                    "uniqueIdType": "unknown"
                }
            ],
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Samantha Booth",
                        "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Dana Swope",
                        "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
