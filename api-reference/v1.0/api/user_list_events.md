# <a name="list-events"></a><span data-ttu-id="3527b-101">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3527b-101">List events</span></span>

<span data-ttu-id="3527b-p101">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3527b-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="3527b-104">現在、この操作によって返されるイベントの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="3527b-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="3527b-105">拡張イベントのインスタンスを取得するには、[予定表ビューを取得する](calendar_list_calendarview.md)、または[イベントのインスタンスを取得する](event_list_instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="3527b-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>


### <a name="get-events-in-another-users-calendar"></a><span data-ttu-id="3527b-106">別のユーザーの予定表でイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="3527b-106">Get events in another user's calendar</span></span>

<span data-ttu-id="3527b-107">アプリケーションのアクセス許可がある場合、または 1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合、別のユーザーの予定表からイベントを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="3527b-107">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get events from another user's calendar.</span></span> <span data-ttu-id="3527b-108">このセクションでは、委任されたアクセス許可に関連するシナリオに焦点を当てます。</span><span class="sxs-lookup"><span data-stu-id="3527b-108">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="3527b-109">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="3527b-109">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="3527b-110">別のユーザー Garth は、John と予定表を共有しています。</span><span class="sxs-lookup"><span data-stu-id="3527b-110">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="3527b-111">その場合、以下に示す例のクエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有の予定表でイベントを取得できます。</span><span class="sxs-lookup"><span data-stu-id="3527b-111">You can get the events in that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/events
```

<span data-ttu-id="3527b-112">この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対しサポートされているすべての GET イベント操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3527b-112">This capability applies to all the supported GET events operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="3527b-113">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="3527b-113">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="3527b-114">Garth が John と予定表を共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="3527b-114">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="3527b-115">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身の予定表でイベントを取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="3527b-115">In such cases, specifying a user ID or user principal name only works for getting events in the signed-in user’s own calendars, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/events
```

<span data-ttu-id="3527b-116">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="3527b-116">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="3527b-117">共有の連絡先フォルダー</span><span class="sxs-lookup"><span data-stu-id="3527b-117">Shared contact folders</span></span>
- <span data-ttu-id="3527b-118">共有の予定表</span><span class="sxs-lookup"><span data-stu-id="3527b-118">Shared calendars</span></span>
- <span data-ttu-id="3527b-119">共有フォルダー内の連絡先およびイベント</span><span class="sxs-lookup"><span data-stu-id="3527b-119">Contacts and events in shared folders</span></span>
- <span data-ttu-id="3527b-120">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="3527b-120">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="3527b-121">この機能は、連絡先、イベント、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="3527b-121">This capability is not available in other operations for contacts, events, and their folders.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="3527b-122">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="3527b-122">Support various time zones</span></span>

<span data-ttu-id="3527b-123">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="3527b-123">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="3527b-124">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="3527b-124">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="3527b-p106">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="3527b-p106">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="3527b-128">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="3527b-128">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="3527b-129">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3527b-129">Permissions</span></span>
<span data-ttu-id="3527b-p107">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3527b-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3527b-132">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3527b-132">Permission type</span></span>      | <span data-ttu-id="3527b-133">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3527b-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3527b-134">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3527b-134">Delegated (work or school account)</span></span> | <span data-ttu-id="3527b-135">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3527b-135">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3527b-136">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3527b-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3527b-137">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3527b-137">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3527b-138">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3527b-138">Application</span></span> | <span data-ttu-id="3527b-139">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3527b-139">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3527b-140">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3527b-140">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="3527b-141">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3527b-141">Optional query parameters</span></span>
<span data-ttu-id="3527b-142">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3527b-142">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3527b-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3527b-143">Request headers</span></span>
| <span data-ttu-id="3527b-144">名前</span><span class="sxs-lookup"><span data-stu-id="3527b-144">Name</span></span>       | <span data-ttu-id="3527b-145">型</span><span class="sxs-lookup"><span data-stu-id="3527b-145">Type</span></span> | <span data-ttu-id="3527b-146">説明</span><span class="sxs-lookup"><span data-stu-id="3527b-146">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3527b-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="3527b-147">Authorization</span></span>  | <span data-ttu-id="3527b-148">string</span><span class="sxs-lookup"><span data-stu-id="3527b-148">string</span></span>  | <span data-ttu-id="3527b-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3527b-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3527b-151">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="3527b-151">Prefer: outlook.timezone</span></span> | <span data-ttu-id="3527b-152">string</span><span class="sxs-lookup"><span data-stu-id="3527b-152">string</span></span> | <span data-ttu-id="3527b-p109">応答内のイベントに対する既定のタイム ゾーン。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3527b-p109">The default time zone for events in the response. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3527b-155">要求本文</span><span class="sxs-lookup"><span data-stu-id="3527b-155">Request body</span></span>
<span data-ttu-id="3527b-156">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3527b-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3527b-157">応答</span><span class="sxs-lookup"><span data-stu-id="3527b-157">Response</span></span>

<span data-ttu-id="3527b-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3527b-158">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3527b-159">例</span><span class="sxs-lookup"><span data-stu-id="3527b-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3527b-160">要求</span><span class="sxs-lookup"><span data-stu-id="3527b-160">Request</span></span>
<span data-ttu-id="3527b-p110">以下は、要求の例です。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="3527b-p110">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="3527b-163">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="3527b-163">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="3527b-p111">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターがない場合には、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3527b-p111">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="3527b-166">応答</span><span class="sxs-lookup"><span data-stu-id="3527b-166">Response</span></span>
<span data-ttu-id="3527b-p112">以下は、応答の例です。**body** プロパティが既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="3527b-p112">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
