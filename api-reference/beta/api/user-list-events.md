---
title: イベントを一覧表示する
description: 'ユーザーの既定の予定表、または指定された予定表からイベント オブジェクトの一覧を取得する '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3da827e8110f45df59213ec1549b6cc351ccfb1e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421044"
---
# <a name="list-events"></a><span data-ttu-id="e559f-103">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e559f-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e559f-104">ユーザーの既定の予定表、または指定された予定表から[イベント](../resources/event.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e559f-104">Get a list of [event](../resources/event.md) objects from the user's default calendar or from a specified calendar.</span></span> <span data-ttu-id="e559f-105">一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e559f-105">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="e559f-106">拡張イベントのインスタンスを取得すると、[予定表ビューを取得する](calendar-list-calendarview.md)または[イベントのインスタンスを取得する](event-list-instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="e559f-106">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="e559f-107">アプリが別のユーザーの予定表のイベントを取得できるシナリオが 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="e559f-107">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="e559f-108">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="e559f-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="e559f-109">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーと予定表を共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="e559f-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="e559f-110">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e559f-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="e559f-111">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="e559f-111">Support various time zones</span></span>

<span data-ttu-id="e559f-112">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="e559f-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="e559f-113">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="e559f-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="e559f-p103">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="e559f-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="e559f-117">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="e559f-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="e559f-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e559f-118">Permissions</span></span>
<span data-ttu-id="e559f-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e559f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e559f-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e559f-121">Permission type</span></span>      | <span data-ttu-id="e559f-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e559f-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e559f-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e559f-123">Delegated (work or school account)</span></span> | <span data-ttu-id="e559f-124">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e559f-124">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e559f-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e559f-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e559f-126">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e559f-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e559f-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e559f-127">Application</span></span> | <span data-ttu-id="e559f-128">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e559f-128">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e559f-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e559f-129">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="e559f-130">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e559f-130">Optional query parameters</span></span>
<span data-ttu-id="e559f-131">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e559f-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e559f-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e559f-132">Request headers</span></span>
| <span data-ttu-id="e559f-133">名前</span><span class="sxs-lookup"><span data-stu-id="e559f-133">Name</span></span>       | <span data-ttu-id="e559f-134">種類</span><span class="sxs-lookup"><span data-stu-id="e559f-134">Type</span></span> | <span data-ttu-id="e559f-135">説明</span><span class="sxs-lookup"><span data-stu-id="e559f-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e559f-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="e559f-136">Authorization</span></span>  | <span data-ttu-id="e559f-137">string</span><span class="sxs-lookup"><span data-stu-id="e559f-137">string</span></span>  | <span data-ttu-id="e559f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e559f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e559f-140">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e559f-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="e559f-141">string</span><span class="sxs-lookup"><span data-stu-id="e559f-141">string</span></span> | <span data-ttu-id="e559f-142">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="e559f-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e559f-143">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="e559f-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e559f-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e559f-144">Optional.</span></span> |
| <span data-ttu-id="e559f-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="e559f-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="e559f-146">string</span><span class="sxs-lookup"><span data-stu-id="e559f-146">string</span></span> | <span data-ttu-id="e559f-147">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="e559f-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="e559f-148">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="e559f-148">Values can be "text" or "html".</span></span> <span data-ttu-id="e559f-149">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="e559f-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="e559f-150">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="e559f-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="e559f-151">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e559f-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e559f-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="e559f-152">Request body</span></span>
<span data-ttu-id="e559f-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e559f-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e559f-154">応答</span><span class="sxs-lookup"><span data-stu-id="e559f-154">Response</span></span>

<span data-ttu-id="e559f-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e559f-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e559f-156">例</span><span class="sxs-lookup"><span data-stu-id="e559f-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e559f-157">要求 1</span><span class="sxs-lookup"><span data-stu-id="e559f-157">Request 1</span></span>
<span data-ttu-id="e559f-158">最初の例は、ユーザーのイベントをすべて取得します。</span><span class="sxs-lookup"><span data-stu-id="e559f-158">The first example gets all the user's events.</span></span> <span data-ttu-id="e559f-159">以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="e559f-159">It specifies the following:</span></span>

- <span data-ttu-id="e559f-160">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="e559f-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="e559f-p109">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターを使用しないと、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e559f-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="e559f-163">要求では、返されたイベント本体の具体的な形式を示す `Prefer: outlook.body-content-type` ヘッダーを指定しません。</span><span class="sxs-lookup"><span data-stu-id="e559f-163">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="e559f-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="e559f-164">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e559f-165">C#</span><span class="sxs-lookup"><span data-stu-id="e559f-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e559f-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e559f-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e559f-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e559f-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="e559f-168">応答 1</span><span class="sxs-lookup"><span data-stu-id="e559f-168">Response 1</span></span>
<span data-ttu-id="e559f-169">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e559f-169">Here is an example of the response.</span></span> <span data-ttu-id="e559f-170">`Prefer: outlook.body-content-type` ヘッダーが指定されていないため、**body** プロパティが既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="e559f-170">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_events",
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
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

##### <a name="request-2"></a><span data-ttu-id="e559f-171">要求 2</span><span class="sxs-lookup"><span data-stu-id="e559f-171">Request 2</span></span>
<span data-ttu-id="e559f-172">2 番目の例は、`Prefer: outlook.body-content-type="text"` ヘッダーを使用して指定されたメッセージの **body** プロパティをテキスト形式で取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e559f-172">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>

<span data-ttu-id="e559f-173">この要求も、`$select` クエリ パラメーターを使用して特定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="e559f-173">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="e559f-174">`$select` パラメーターを使用しないと、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e559f-174">Without a `$select` parameter, all of the event properties will be returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e559f-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="e559f-175">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text" 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e559f-176">C#</span><span class="sxs-lookup"><span data-stu-id="e559f-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e559f-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e559f-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e559f-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e559f-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="e559f-179">応答 2</span><span class="sxs-lookup"><span data-stu-id="e559f-179">Response 2</span></span>
<span data-ttu-id="e559f-180">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e559f-180">Here is an example of the response.</span></span> <span data-ttu-id="e559f-181">**body** プロパティがテキスト形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="e559f-181">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 640

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
