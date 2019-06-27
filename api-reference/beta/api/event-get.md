---
title: イベントを取得する
description: 指定したイベントオブジェクトのプロパティと関係を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b3c09dbc4ef62609d57ca8f62a7081f58f3fa2df
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259179"
---
# <a name="get-event"></a><span data-ttu-id="d3e2e-103">イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="d3e2e-103">Get event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3e2e-104">指定した[イベント](../resources/event.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-104">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="d3e2e-105">アプリが別のユーザーの予定表のイベントを取得できるシナリオが 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-105">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="d3e2e-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="d3e2e-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d3e2e-107">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーと予定表を共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d3e2e-108">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-108">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="d3e2e-109">**event** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**event** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-109">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="d3e2e-110">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-110">Support various time zones</span></span>

<span data-ttu-id="d3e2e-111">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-111">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="d3e2e-112">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-112">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="d3e2e-p102">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="d3e2e-116">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-116">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3e2e-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d3e2e-117">Permissions</span></span>
<span data-ttu-id="d3e2e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e2e-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3e2e-120">Permission type</span></span>      | <span data-ttu-id="d3e2e-121">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3e2e-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3e2e-122">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3e2e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="d3e2e-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3e2e-123">Calendars.Read</span></span>    |
|<span data-ttu-id="d3e2e-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3e2e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3e2e-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3e2e-125">Calendars.Read</span></span>    |
|<span data-ttu-id="d3e2e-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3e2e-126">Application</span></span> | <span data-ttu-id="d3e2e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3e2e-127">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3e2e-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3e2e-128">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="d3e2e-129">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d3e2e-129">Optional query parameters</span></span>
<span data-ttu-id="d3e2e-130">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d3e2e-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3e2e-131">Request headers</span></span>
| <span data-ttu-id="d3e2e-132">名前</span><span class="sxs-lookup"><span data-stu-id="d3e2e-132">Name</span></span>       | <span data-ttu-id="d3e2e-133">型</span><span class="sxs-lookup"><span data-stu-id="d3e2e-133">Type</span></span> | <span data-ttu-id="d3e2e-134">説明</span><span class="sxs-lookup"><span data-stu-id="d3e2e-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d3e2e-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3e2e-135">Authorization</span></span>  | <span data-ttu-id="d3e2e-136">string</span><span class="sxs-lookup"><span data-stu-id="d3e2e-136">string</span></span>  | <span data-ttu-id="d3e2e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3e2e-139">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d3e2e-139">Prefer: outlook.timezone</span></span> | <span data-ttu-id="d3e2e-140">string</span><span class="sxs-lookup"><span data-stu-id="d3e2e-140">string</span></span> | <span data-ttu-id="d3e2e-141">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d3e2e-142">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d3e2e-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-143">Optional.</span></span> |
| <span data-ttu-id="d3e2e-144">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="d3e2e-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="d3e2e-145">string</span><span class="sxs-lookup"><span data-stu-id="d3e2e-145">string</span></span> | <span data-ttu-id="d3e2e-146">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="d3e2e-147">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-147">Values can be "text" or "html".</span></span> <span data-ttu-id="d3e2e-148">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="d3e2e-149">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="d3e2e-150">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3e2e-151">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3e2e-151">Request body</span></span>
<span data-ttu-id="d3e2e-152">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3e2e-153">応答</span><span class="sxs-lookup"><span data-stu-id="d3e2e-153">Response</span></span>

<span data-ttu-id="d3e2e-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-154">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3e2e-155">例</span><span class="sxs-lookup"><span data-stu-id="d3e2e-155">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d3e2e-156">要求 1</span><span class="sxs-lookup"><span data-stu-id="d3e2e-156">Request 1</span></span>
<span data-ttu-id="d3e2e-p107">最初の例では、指定されたイベントを取得します。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="d3e2e-159">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-159">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="d3e2e-p108">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターを使用しないと、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="d3e2e-162">要求では、返されたイベント本体の具体的な形式を示す `Prefer: outlook.body-content-type` ヘッダーを指定しません。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-162">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGIAAAoZDOFAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="d3e2e-163">応答 1</span><span class="sxs-lookup"><span data-stu-id="d3e2e-163">Response 1</span></span>
<span data-ttu-id="d3e2e-164">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-164">Here is an example of the response.</span></span> <span data-ttu-id="d3e2e-165">`Prefer: outlook.body-content-type` ヘッダーが指定されていないため、**body** プロパティが既定の HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-165">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3e2e-166">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d3e2e-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3e2e-167">C#</span><span class="sxs-lookup"><span data-stu-id="d3e2e-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3e2e-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3e2e-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_event-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3e2e-169">目的-C</span><span class="sxs-lookup"><span data-stu-id="d3e2e-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_event-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="d3e2e-170">要求 2</span><span class="sxs-lookup"><span data-stu-id="d3e2e-170">Request 2</span></span>
<span data-ttu-id="d3e2e-171">2番目の例では、 `Prefer: outlook.body-content-type="text"`ヘッダーを使用して、指定したイベントの**body**プロパティをテキスト形式で取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-171">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="d3e2e-172">この要求も、`$select` クエリ パラメーターを使用して特定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-172">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="d3e2e-173">`$select` パラメーターを使用しないと、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-173">Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGI1AAAoZDOFAAA=/?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
##### <a name="response-2"></a><span data-ttu-id="d3e2e-174">応答 2</span><span class="sxs-lookup"><span data-stu-id="d3e2e-174">Response 2</span></span>
<span data-ttu-id="d3e2e-175">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-175">Here is an example of the response.</span></span> <span data-ttu-id="d3e2e-176">**body** プロパティがテキスト形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-176">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "name": "get_event_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 636

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGI1AAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3e2e-177">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d3e2e-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3e2e-178">C#</span><span class="sxs-lookup"><span data-stu-id="d3e2e-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_event_in_text-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3e2e-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3e2e-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_event_in_text-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3e2e-180">目的-C</span><span class="sxs-lookup"><span data-stu-id="d3e2e-180">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_event_in_text-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-3"></a><span data-ttu-id="d3e2e-181">要求 3</span><span class="sxs-lookup"><span data-stu-id="d3e2e-181">Request 3</span></span>

<span data-ttu-id="d3e2e-182">3つ目の例では、複数の場所を指定するイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-182">The third example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="d3e2e-183">この要求では、特定のプロパティを返すように `$select` クエリ パラメーターを指定しています。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-183">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-3"></a><span data-ttu-id="d3e2e-184">応答 3</span><span class="sxs-lookup"><span data-stu-id="d3e2e-184">Response 3</span></span>
<span data-ttu-id="d3e2e-185">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-185">Here is an example of the response.</span></span> <span data-ttu-id="d3e2e-186">**locations** プロパティには、イベントを開催する 3 つの場所の詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-186">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="d3e2e-187">要求で`Prefer: outlook.timezone`はまたは`Prefer: outlook.body-content-type`ヘッダーが指定されていないため、 **start**および**end**プロパティは既定の UTC タイムゾーンで表示され、本文は既定の HTML 形式になります。</span><span class="sxs-lookup"><span data-stu-id="d3e2e-187">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3e2e-188">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d3e2e-188">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3e2e-189">C#</span><span class="sxs-lookup"><span data-stu-id="d3e2e-189">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_event_multiple_locations-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3e2e-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3e2e-190">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_event_multiple_locations-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3e2e-191">目的-C</span><span class="sxs-lookup"><span data-stu-id="d3e2e-191">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_event_multiple_locations-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="d3e2e-192">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3e2e-192">See also</span></span>

- [<span data-ttu-id="d3e2e-193">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="d3e2e-193">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d3e2e-194">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d3e2e-194">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d3e2e-195">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d3e2e-195">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
