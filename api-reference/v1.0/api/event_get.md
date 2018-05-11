# <a name="get-event"></a><span data-ttu-id="de500-101">イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="de500-101">Get event</span></span>

<span data-ttu-id="de500-102">指定した[イベント](../resources/event.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="de500-102">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="de500-103">現在、この操作によって返されるイベントの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="de500-103">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="de500-104">**event** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`GET` 操作を使用して、**event** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="de500-104">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="get-events-in-another-users-calendar"></a><span data-ttu-id="de500-105">別のユーザーの予定表でイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="de500-105">Get events in another user's calendar</span></span>

<span data-ttu-id="de500-106">アプリケーションのアクセス許可がある場合、または 1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合、別のユーザーの予定表からイベントを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="de500-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get events from another user's calendar.</span></span> <span data-ttu-id="de500-107">このセクションでは、委任されたアクセス許可に関連するシナリオに焦点を当てます。</span><span class="sxs-lookup"><span data-stu-id="de500-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="de500-108">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="de500-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="de500-109">別のユーザー Garth は、John と予定表を共有しています。</span><span class="sxs-lookup"><span data-stu-id="de500-109">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="de500-110">その場合、以下に示す例のクエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有の予定表でイベントを取得できます。</span><span class="sxs-lookup"><span data-stu-id="de500-110">You can get an event in that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/events/{id}
```

<span data-ttu-id="de500-111">この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対しサポートされているすべての GET イベント操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="de500-111">This capability applies to all the supported GET events operations for an individual user, as listed in the [HTTP request](#http-request) section below .</span></span> <span data-ttu-id="de500-112">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="de500-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="de500-113">Garth が John と予定表を共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="de500-113">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="de500-114">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身の予定表でイベントを取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="de500-114">In such cases, specifying a user ID or user principal name only works for getting an event in the signed-in user’s own calendars, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
```

<span data-ttu-id="de500-115">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="de500-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="de500-116">共有の連絡先フォルダー、予定表、メッセージ フォルダー</span><span class="sxs-lookup"><span data-stu-id="de500-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="de500-117">連絡先、イベント、共有フォルダー内のメッセージ</span><span class="sxs-lookup"><span data-stu-id="de500-117">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="de500-118">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="de500-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="de500-119">この機能は、連絡先、イベント、メッセージ、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="de500-119">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="de500-120">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="de500-120">Support various time zones</span></span>

<span data-ttu-id="de500-121">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="de500-121">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="de500-122">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="de500-122">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="de500-p105">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="de500-p105">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="de500-126">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="de500-126">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="de500-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de500-127">Permissions</span></span>
<span data-ttu-id="de500-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de500-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="de500-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de500-130">Permission type</span></span>      | <span data-ttu-id="de500-131">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de500-131">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de500-132">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de500-132">Delegated (work or school account)</span></span> | <span data-ttu-id="de500-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de500-133">Calendars.Read</span></span>    |
|<span data-ttu-id="de500-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de500-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de500-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de500-135">Calendars.Read</span></span>    |
|<span data-ttu-id="de500-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de500-136">Application</span></span> | <span data-ttu-id="de500-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de500-137">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="de500-138">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de500-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroup/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="de500-139">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="de500-139">Optional query parameters</span></span>
<span data-ttu-id="de500-140">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="de500-140">This method supports the [OData Query Parameters](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="de500-141">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de500-141">Request headers</span></span>
| <span data-ttu-id="de500-142">名前</span><span class="sxs-lookup"><span data-stu-id="de500-142">Name</span></span>       | <span data-ttu-id="de500-143">型</span><span class="sxs-lookup"><span data-stu-id="de500-143">Type</span></span> | <span data-ttu-id="de500-144">説明</span><span class="sxs-lookup"><span data-stu-id="de500-144">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="de500-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="de500-145">Authorization</span></span>  | <span data-ttu-id="de500-146">string</span><span class="sxs-lookup"><span data-stu-id="de500-146">string</span></span> | <span data-ttu-id="de500-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de500-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="de500-149">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="de500-149">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="de500-150">string</span><span class="sxs-lookup"><span data-stu-id="de500-150">string</span></span> | <span data-ttu-id="de500-151">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="de500-151">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="de500-152">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="de500-152">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="de500-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="de500-153">Optional.</span></span> |
| <span data-ttu-id="de500-154">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="de500-154">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="de500-155">string</span><span class="sxs-lookup"><span data-stu-id="de500-155">string</span></span> | <span data-ttu-id="de500-156">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="de500-156">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="de500-157">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="de500-157">Values can be "text" or "html".</span></span> <span data-ttu-id="de500-158">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="de500-158">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="de500-159">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="de500-159">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="de500-160">省略可能。</span><span class="sxs-lookup"><span data-stu-id="de500-160">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de500-161">要求本文</span><span class="sxs-lookup"><span data-stu-id="de500-161">Request body</span></span>
<span data-ttu-id="de500-162">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="de500-162">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de500-163">応答</span><span class="sxs-lookup"><span data-stu-id="de500-163">Response</span></span>

<span data-ttu-id="de500-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="de500-164">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de500-165">例</span><span class="sxs-lookup"><span data-stu-id="de500-165">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="de500-166">要求 1</span><span class="sxs-lookup"><span data-stu-id="de500-166">Request 1</span></span>
<span data-ttu-id="de500-p110">最初の例では、指定されたイベントを取得します。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="de500-p110">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="de500-169">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="de500-169">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="de500-p111">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターがない場合には、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="de500-p111">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response-1"></a><span data-ttu-id="de500-172">応答 1</span><span class="sxs-lookup"><span data-stu-id="de500-172">Response 1</span></span>

<span data-ttu-id="de500-p112">以下は、応答の例です。**body** プロパティが HTML の既定の形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="de500-p112">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1928

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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
```


##### <a name="request-2"></a><span data-ttu-id="de500-175">要求 2</span><span class="sxs-lookup"><span data-stu-id="de500-175">Request 2</span></span>

<span data-ttu-id="de500-176">2 番目の例では、複数の場所を指定するイベントを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="de500-176">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="de500-177">この要求では、特定のプロパティを返すように `$select` クエリ パラメーターを指定しています。</span><span class="sxs-lookup"><span data-stu-id="de500-177">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkADAGAADDdm4NAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-2"></a><span data-ttu-id="de500-178">応答 2</span><span class="sxs-lookup"><span data-stu-id="de500-178">Response 2</span></span>
<span data-ttu-id="de500-179">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="de500-179">Here is an example of the response.</span></span> <span data-ttu-id="de500-180">**locations** プロパティには、イベントを開催する 3 つの場所の詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de500-180">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="de500-181">要求では `Prefer: outlook.timezone` ヘッダーを指定していないため、**start** および **end** プロパティは既定の UTC タイム ゾーンで表示されます。</span><span class="sxs-lookup"><span data-stu-id="de500-181">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="de500-182">イベントの本文は、既定の HTML 形式になっています。</span><span class="sxs-lookup"><span data-stu-id="de500-182">The event body is in the default HTML format.</span></span>  

<!-- {
  "blockType": "response",
  "name": "get_event_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"UTC"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"UTC"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
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
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```



## <a name="see-also"></a><span data-ttu-id="de500-183">関連項目</span><span class="sxs-lookup"><span data-stu-id="de500-183">See also</span></span>

- [<span data-ttu-id="de500-184">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="de500-184">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="de500-185">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="de500-185">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="de500-186">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="de500-186">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
