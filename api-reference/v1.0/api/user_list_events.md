# <a name="list-events"></a><span data-ttu-id="b6f69-101">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b6f69-101">List events</span></span>

<span data-ttu-id="b6f69-p101">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6f69-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="b6f69-104">現在、この操作によって返されるイベントの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="b6f69-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="b6f69-105">拡張イベントのインスタンスを取得するには、[予定表ビューを取得する](calendar_list_calendarview.md)、または[イベントのインスタンスを取得する](event_list_instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="b6f69-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="b6f69-106">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="b6f69-106">Support various time zones</span></span>

<span data-ttu-id="b6f69-107">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="b6f69-107">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="b6f69-108">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="b6f69-108">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="b6f69-p102">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="b6f69-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="b6f69-112">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="b6f69-112">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6f69-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6f69-113">Permissions</span></span>
<span data-ttu-id="b6f69-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6f69-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b6f69-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6f69-116">Permission type</span></span>      | <span data-ttu-id="b6f69-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6f69-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6f69-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6f69-118">Delegated (work or school account)</span></span> | <span data-ttu-id="b6f69-119">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6f69-119">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b6f69-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6f69-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6f69-121">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6f69-121">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b6f69-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6f69-122">Application</span></span> | <span data-ttu-id="b6f69-123">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6f69-123">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6f69-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6f69-124">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="b6f69-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b6f69-125">Optional query parameters</span></span>
<span data-ttu-id="b6f69-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b6f69-126">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b6f69-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6f69-127">Request headers</span></span>
| <span data-ttu-id="b6f69-128">名前</span><span class="sxs-lookup"><span data-stu-id="b6f69-128">Name</span></span>       | <span data-ttu-id="b6f69-129">型</span><span class="sxs-lookup"><span data-stu-id="b6f69-129">Type</span></span> | <span data-ttu-id="b6f69-130">説明</span><span class="sxs-lookup"><span data-stu-id="b6f69-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b6f69-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6f69-131">Authorization</span></span>  | <span data-ttu-id="b6f69-132">string</span><span class="sxs-lookup"><span data-stu-id="b6f69-132">string</span></span>  | <span data-ttu-id="b6f69-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b6f69-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6f69-135">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b6f69-135">Prefer: outlook.timezone</span></span> | <span data-ttu-id="b6f69-136">string</span><span class="sxs-lookup"><span data-stu-id="b6f69-136">string</span></span> | <span data-ttu-id="b6f69-p105">応答内のイベントに対する既定のタイム ゾーン。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b6f69-p105">The default time zone for events in the response. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6f69-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6f69-139">Request body</span></span>
<span data-ttu-id="b6f69-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6f69-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f69-141">応答</span><span class="sxs-lookup"><span data-stu-id="b6f69-141">Response</span></span>

<span data-ttu-id="b6f69-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b6f69-142">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6f69-143">例</span><span class="sxs-lookup"><span data-stu-id="b6f69-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6f69-144">要求</span><span class="sxs-lookup"><span data-stu-id="b6f69-144">Request</span></span>
<span data-ttu-id="b6f69-p106">以下は、要求の例です。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6f69-p106">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="b6f69-147">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="b6f69-147">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="b6f69-p107">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターがない場合には、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b6f69-p107">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="b6f69-150">応答</span><span class="sxs-lookup"><span data-stu-id="b6f69-150">Response</span></span>
<span data-ttu-id="b6f69-p108">以下は、応答の例です。**body** プロパティが既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="b6f69-p108">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
            "location":{
                "displayName":"Assembly Hall"
            },
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Fanny Downs",
                        "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
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
                    "name":"Fanny Downs",
                    "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
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
