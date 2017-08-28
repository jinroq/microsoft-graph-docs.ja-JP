# <a name="get-event"></a><span data-ttu-id="adaab-101">イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="adaab-101">Get event</span></span>

<span data-ttu-id="adaab-102">指定した[イベント](../resources/event.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="adaab-102">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="adaab-103">現在、この操作によって返されるイベントの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="adaab-103">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="adaab-104">**イベント** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`GET` 操作を使用して、**イベント** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="adaab-104">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="adaab-105">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="adaab-105">Support various time zones</span></span>

<span data-ttu-id="adaab-106">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="adaab-106">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="adaab-107">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="adaab-107">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="adaab-p101">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="adaab-p101">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="adaab-111">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="adaab-111">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="adaab-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="adaab-112">Permissions</span></span>
<span data-ttu-id="adaab-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="adaab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="adaab-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="adaab-115">Permission type</span></span>      | <span data-ttu-id="adaab-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="adaab-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adaab-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="adaab-117">Delegated (work or school account)</span></span> | <span data-ttu-id="adaab-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="adaab-118">Calendars.Read</span></span>    |
|<span data-ttu-id="adaab-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="adaab-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adaab-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="adaab-120">Calendars.Read</span></span>    |
|<span data-ttu-id="adaab-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="adaab-121">Application</span></span> | <span data-ttu-id="adaab-122">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="adaab-122">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="adaab-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="adaab-123">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="adaab-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="adaab-124">Optional query parameters</span></span>
<span data-ttu-id="adaab-125">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="adaab-125">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="adaab-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adaab-126">Request headers</span></span>
| <span data-ttu-id="adaab-127">名前</span><span class="sxs-lookup"><span data-stu-id="adaab-127">Name</span></span>       | <span data-ttu-id="adaab-128">型</span><span class="sxs-lookup"><span data-stu-id="adaab-128">Type</span></span> | <span data-ttu-id="adaab-129">説明</span><span class="sxs-lookup"><span data-stu-id="adaab-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="adaab-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="adaab-130">Authorization</span></span>  | <span data-ttu-id="adaab-131">string</span><span class="sxs-lookup"><span data-stu-id="adaab-131">string</span></span>  | <span data-ttu-id="adaab-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="adaab-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="adaab-134">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="adaab-134">Prefer: outlook.timezone</span></span> | <span data-ttu-id="adaab-135">string</span><span class="sxs-lookup"><span data-stu-id="adaab-135">string</span></span> | <span data-ttu-id="adaab-136">応答内のイベントに対する既定のタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="adaab-136">The default time zone for events in the response.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adaab-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="adaab-137">Request body</span></span>
<span data-ttu-id="adaab-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="adaab-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adaab-139">応答</span><span class="sxs-lookup"><span data-stu-id="adaab-139">Response</span></span>

<span data-ttu-id="adaab-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="adaab-140">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="adaab-141">例</span><span class="sxs-lookup"><span data-stu-id="adaab-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="adaab-142">要求</span><span class="sxs-lookup"><span data-stu-id="adaab-142">Request</span></span>
<span data-ttu-id="adaab-p104">最初の例では、指定されたイベントを取得します。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="adaab-p104">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="adaab-145">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="adaab-145">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="adaab-p105">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターがない場合には、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="adaab-p105">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response"></a><span data-ttu-id="adaab-148">応答</span><span class="sxs-lookup"><span data-stu-id="adaab-148">Response</span></span>

<span data-ttu-id="adaab-p106">以下は、応答の例です。**body** プロパティが HTML の既定の形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="adaab-p106">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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
```

## <a name="see-also"></a><span data-ttu-id="adaab-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="adaab-151">See also</span></span>

- [<span data-ttu-id="adaab-152">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="adaab-152">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="adaab-153">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="adaab-153">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
