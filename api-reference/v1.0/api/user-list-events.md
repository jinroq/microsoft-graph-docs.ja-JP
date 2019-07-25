---
title: イベントを一覧表示する
description: 'ユーザーのメールボックス内のイベント オブジェクトの一覧を取得します。 単一が含まれているリスト '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6dc8b7cc5109b054bb5b8285770c3cfdff6f381a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888872"
---
# <a name="list-events"></a><span data-ttu-id="7bd78-104">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7bd78-104">List events</span></span>

<span data-ttu-id="7bd78-p102">ユーザーのメールボックス内の[イベント](../resources/event.md) オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7bd78-p102">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="7bd78-107">拡張イベントのインスタンスを取得すると、[予定表ビューを取得する](calendar-list-calendarview.md)または[イベントのインスタンスを取得する](event-list-instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="7bd78-108">現在、この操作によって返されるイベントの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="7bd78-108">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="7bd78-109">アプリが別のユーザーの予定表のイベントを取得できるシナリオが 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="7bd78-109">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="7bd78-110">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="7bd78-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="7bd78-111">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーと予定表を共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="7bd78-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="7bd78-112">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7bd78-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="7bd78-113">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="7bd78-113">Support various time zones</span></span>

<span data-ttu-id="7bd78-114">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-114">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="7bd78-115">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="7bd78-115">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="7bd78-p104">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-p104">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="7bd78-119">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-119">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bd78-120">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7bd78-120">Permissions</span></span>
<span data-ttu-id="7bd78-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7bd78-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bd78-123">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7bd78-123">Permission type</span></span>      | <span data-ttu-id="7bd78-124">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7bd78-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bd78-125">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7bd78-125">Delegated (work or school account)</span></span> | <span data-ttu-id="7bd78-126">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bd78-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7bd78-127">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7bd78-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bd78-128">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bd78-128">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7bd78-129">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7bd78-129">Application</span></span> | <span data-ttu-id="7bd78-130">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bd78-130">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bd78-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7bd78-131">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="7bd78-132">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7bd78-132">Optional query parameters</span></span>
<span data-ttu-id="7bd78-133">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7bd78-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7bd78-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bd78-134">Request headers</span></span>
| <span data-ttu-id="7bd78-135">名前</span><span class="sxs-lookup"><span data-stu-id="7bd78-135">Name</span></span>       | <span data-ttu-id="7bd78-136">型</span><span class="sxs-lookup"><span data-stu-id="7bd78-136">Type</span></span> | <span data-ttu-id="7bd78-137">説明</span><span class="sxs-lookup"><span data-stu-id="7bd78-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="7bd78-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bd78-138">Authorization</span></span>  | <span data-ttu-id="7bd78-139">string</span><span class="sxs-lookup"><span data-stu-id="7bd78-139">string</span></span> | <span data-ttu-id="7bd78-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7bd78-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7bd78-142">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7bd78-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="7bd78-143">string</span><span class="sxs-lookup"><span data-stu-id="7bd78-143">string</span></span> | <span data-ttu-id="7bd78-144">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="7bd78-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="7bd78-145">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="7bd78-146">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7bd78-146">Optional.</span></span> |
| <span data-ttu-id="7bd78-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="7bd78-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="7bd78-148">string</span><span class="sxs-lookup"><span data-stu-id="7bd78-148">string</span></span> | <span data-ttu-id="7bd78-149">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="7bd78-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="7bd78-150">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="7bd78-150">Values can be "text" or "html".</span></span> <span data-ttu-id="7bd78-151">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="7bd78-152">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="7bd78-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7bd78-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bd78-154">要求本文</span><span class="sxs-lookup"><span data-stu-id="7bd78-154">Request body</span></span>
<span data-ttu-id="7bd78-155">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7bd78-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bd78-156">応答</span><span class="sxs-lookup"><span data-stu-id="7bd78-156">Response</span></span>

<span data-ttu-id="7bd78-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7bd78-157">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bd78-158">例</span><span class="sxs-lookup"><span data-stu-id="7bd78-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bd78-159">要求</span><span class="sxs-lookup"><span data-stu-id="7bd78-159">Request</span></span>
<span data-ttu-id="7bd78-p109">以下は、要求の例です。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="7bd78-p109">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="7bd78-162">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="7bd78-162">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="7bd78-p110">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターを使用しないと、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-p110">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7bd78-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bd78-165">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bd78-166">C#</span><span class="sxs-lookup"><span data-stu-id="7bd78-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bd78-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bd78-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bd78-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bd78-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7bd78-169">Java</span><span class="sxs-lookup"><span data-stu-id="7bd78-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7bd78-170">応答</span><span class="sxs-lookup"><span data-stu-id="7bd78-170">Response</span></span>
<span data-ttu-id="7bd78-p111">以下は、応答の例です。**body** プロパティが既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="7bd78-p111">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
