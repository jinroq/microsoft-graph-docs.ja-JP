---
title: イベントを取得する
description: 指定したイベント オブジェクトのプロパティとリレーションシップを取得します。
ms.openlocfilehash: 3a11b73e4f8c367ca997bf11ca58a4bd90918a0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072276"
---
# <a name="get-event"></a><span data-ttu-id="d162c-103">イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="d162c-103">Get event</span></span>

> <span data-ttu-id="d162c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d162c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d162c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d162c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d162c-106">指定した[イベント](../resources/event.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d162c-106">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="d162c-107">2 つシナリオは、アプリケーションが別のユーザーの予定表でイベントを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="d162c-107">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="d162c-108">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="d162c-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d162c-109">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーとカレンダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="d162c-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d162c-110">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d162c-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="d162c-111">**イベント** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**イベント** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="d162c-111">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="d162c-112">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="d162c-112">Support various time zones</span></span>

<span data-ttu-id="d162c-113">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="d162c-113">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="d162c-114">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="d162c-114">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="d162c-p103">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="d162c-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="d162c-118">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="d162c-118">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="d162c-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d162c-119">Permissions</span></span>
<span data-ttu-id="d162c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d162c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d162c-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d162c-122">Permission type</span></span>      | <span data-ttu-id="d162c-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d162c-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d162c-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d162c-124">Delegated (work or school account)</span></span> | <span data-ttu-id="d162c-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d162c-125">Calendars.Read</span></span>    |
|<span data-ttu-id="d162c-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d162c-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d162c-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d162c-127">Calendars.Read</span></span>    |
|<span data-ttu-id="d162c-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d162c-128">Application</span></span> | <span data-ttu-id="d162c-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d162c-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d162c-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d162c-130">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="d162c-131">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d162c-131">Optional query parameters</span></span>
<span data-ttu-id="d162c-132">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d162c-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d162c-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d162c-133">Request headers</span></span>
| <span data-ttu-id="d162c-134">名前</span><span class="sxs-lookup"><span data-stu-id="d162c-134">Name</span></span>       | <span data-ttu-id="d162c-135">型</span><span class="sxs-lookup"><span data-stu-id="d162c-135">Type</span></span> | <span data-ttu-id="d162c-136">説明</span><span class="sxs-lookup"><span data-stu-id="d162c-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d162c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d162c-137">Authorization</span></span>  | <span data-ttu-id="d162c-138">string</span><span class="sxs-lookup"><span data-stu-id="d162c-138">string</span></span>  | <span data-ttu-id="d162c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d162c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d162c-141">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d162c-141">Prefer: outlook.timezone</span></span> | <span data-ttu-id="d162c-142">文字列</span><span class="sxs-lookup"><span data-stu-id="d162c-142">string</span></span> | <span data-ttu-id="d162c-143">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="d162c-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d162c-144">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="d162c-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d162c-145">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d162c-145">Optional.</span></span> |
| <span data-ttu-id="d162c-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="d162c-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="d162c-147">文字列</span><span class="sxs-lookup"><span data-stu-id="d162c-147">string</span></span> | <span data-ttu-id="d162c-148">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="d162c-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="d162c-149">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="d162c-149">Values can be "text" or "html".</span></span> <span data-ttu-id="d162c-150">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="d162c-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="d162c-151">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d162c-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="d162c-152">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d162c-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d162c-153">要求本文</span><span class="sxs-lookup"><span data-stu-id="d162c-153">Request body</span></span>
<span data-ttu-id="d162c-154">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d162c-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d162c-155">応答</span><span class="sxs-lookup"><span data-stu-id="d162c-155">Response</span></span>

<span data-ttu-id="d162c-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d162c-156">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d162c-157">例</span><span class="sxs-lookup"><span data-stu-id="d162c-157">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d162c-158">要求 1</span><span class="sxs-lookup"><span data-stu-id="d162c-158">Request 1</span></span>
<span data-ttu-id="d162c-p108">最初の例では、指定されたイベントを取得します。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="d162c-p108">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="d162c-161">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="d162c-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="d162c-p109">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターがない場合には、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d162c-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="d162c-164">要求が指定されていません、`Prefer: outlook.body-content-type`ヘッダーが返されたイベントの本文の特定の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d162c-164">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="d162c-165">応答 1</span><span class="sxs-lookup"><span data-stu-id="d162c-165">Response 1</span></span>
<span data-ttu-id="d162c-166">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d162c-166">Here is an example of the response.</span></span> <span data-ttu-id="d162c-167">なし`Prefer: outlook.body-content-type`ヘッダーが指定されている**body**プロパティで返される既定の HTML 形式です。</span><span class="sxs-lookup"><span data-stu-id="d162c-167">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

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

##### <a name="request-2"></a><span data-ttu-id="d162c-168">要求 2</span><span class="sxs-lookup"><span data-stu-id="d162c-168">Request 2</span></span>
<span data-ttu-id="d162c-169">2 番目の例を使用する方法を示しています、`Prefer: outlook.body-content-type="text"`ヘッダーをテキスト形式で指定されたイベントの**body**プロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="d162c-169">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="d162c-170">要求を使用しても、`$select`固有のプロパティを取得するパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="d162c-170">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="d162c-171">なし、`$select`パラメーターでは、すべてのイベント プロパティが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d162c-171">Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAoZDOFAAA=')?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
##### <a name="response-2"></a><span data-ttu-id="d162c-172">応答 2</span><span class="sxs-lookup"><span data-stu-id="d162c-172">Response 2</span></span>
<span data-ttu-id="d162c-173">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d162c-173">Here is an example of the response.</span></span> <span data-ttu-id="d162c-174">**Body**プロパティは、テキスト形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d162c-174">The **body** property is returned in text format.</span></span> 

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


##### <a name="request-3"></a><span data-ttu-id="d162c-175">要求 3</span><span class="sxs-lookup"><span data-stu-id="d162c-175">Request 3</span></span>

<span data-ttu-id="d162c-176">複数の場所を指定するイベントを取得する 3 番目の例を示しています。</span><span class="sxs-lookup"><span data-stu-id="d162c-176">The third example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="d162c-177">この要求では、特定のプロパティを返すように `$select` クエリ パラメーターを指定しています。</span><span class="sxs-lookup"><span data-stu-id="d162c-177">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkADAGAADDdm4NAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-3"></a><span data-ttu-id="d162c-178">応答 3</span><span class="sxs-lookup"><span data-stu-id="d162c-178">Response 3</span></span>
<span data-ttu-id="d162c-179">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d162c-179">Here is an example of the response.</span></span> <span data-ttu-id="d162c-180">**locations** プロパティには、イベントを開催する 3 つの場所の詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d162c-180">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="d162c-181">要求を指定しないため、`Prefer: outlook.timezone`または`Prefer: outlook.body-content-type`デフォルト UTC タイム ゾーンは、ヘッダー、**開始**と**終了**のプロパティが表示され、本文が HTML 形式の既定では。</span><span class="sxs-lookup"><span data-stu-id="d162c-181">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

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

## <a name="see-also"></a><span data-ttu-id="d162c-182">関連項目</span><span class="sxs-lookup"><span data-stu-id="d162c-182">See also</span></span>

- [<span data-ttu-id="d162c-183">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="d162c-183">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d162c-184">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d162c-184">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d162c-185">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d162c-185">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
