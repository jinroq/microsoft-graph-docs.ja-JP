---
title: 'カレンダー ビューのイベントへの増分の変更を取得する '
description: 'カレンダー ビューは、既定のカレンダー (../me/calendarview) からの日付/時刻範囲内にあるイベントのコレクションです。 '
author: piotrci
localization_priority: Priority
ms.openlocfilehash: f63f15fe30ea92e237467ac2d73f50345b3d8379
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881180"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a><span data-ttu-id="bb409-103">カレンダー ビューのイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="bb409-103">Get incremental changes to events in a calendar view</span></span> 

<span data-ttu-id="bb409-p101">カレンダー ビューは、既定のカレンダー (../me/calendarview) またはユーザーの他のカレンダーからの日付/時刻範囲内にあるイベントのコレクションです。デルタ クエリを使用すると、カレンダー ビューで新規、更新済み、または削除済みのイベントを取得できます。返されるイベントには、定期的なアイテムの発生と例外、および単一のインスタンスが含まれている場合があります。デルタ データを使用すると、毎回サーバーからユーザーのイベントのセット全体をフェッチせずに、ユーザーのイベントのローカル ストアの保守と同期が行えます。</span><span class="sxs-lookup"><span data-stu-id="bb409-p101">A calendar view is a collection of events in a date/time range from the default calendar (../me/calendarview) or some other calendar of the user's. By using delta query, you can get new, updated, or deleted events in a calendar view. The returned events may include occurrences and exceptions of a recurring series, and single instances. The delta data enables you to maintain and synchronize a local store of a user's events, without having to fetch the entire set of the user's events from the server every time.</span></span>

<span data-ttu-id="bb409-p102">デルタ クエリでは、指定したカレンダー ビュー内のすべてのイベントを取得する完全な同期と、最後の同期以降にカレンダー ビューで変更されたそれらのイベントを取得する増分同期の両方がサポートされています。通常は、最初の完全同期を実行して、その後、そのカレンダー ビューへの増分の変更を定期的に取得します。</span><span class="sxs-lookup"><span data-stu-id="bb409-p102">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization. Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span> 

## <a name="track-event-changes-in-a-calendar-view"></a><span data-ttu-id="bb409-110">カレンダー ビューのイベントの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="bb409-110">Track event changes in a calendar view</span></span>

<span data-ttu-id="bb409-p103">イベントのデルタ クエリは、指定するカレンダーと日付/時刻範囲 (つまり、カレンダー ビュー) に固有のものです。複数のカレンダー ビューの変更を追跡するには、各カレンダーを個別に追跡する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb409-p103">Delta query for events is specific to a calendar and date/time range that you specify (i.e., a calendar view). To track the changes in multiple calendars, you need to track each calendar individually.</span></span> 

<span data-ttu-id="bb409-p104">通常、カレンダー ビュー内のイベント変更の追跡は、[デルタ](/graph/api/event-delta?view=graph-rest-1.0)関数を使用した、1 つ以上の GET 要求のラウンドです。最初の GET 要求は、**デルタ**関数を含めることを除いて、[calendarView の一覧表示](/graph/api/calendar-list-calendarview?view=graph-rest-1.0)方法とほぼ同じです。</span><span class="sxs-lookup"><span data-stu-id="bb409-p104">Tracking event changes in a calendar view typically is a round of one or more GET requests with the [delta](/graph/api/event-delta?view=graph-rest-1.0) function. The initial GET request is very much like the way you [list a calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), except that you include the **delta** function:</span></span>

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="bb409-115">**デルタ**関数を使用した GET 要求は、次のいずれかを返します。</span><span class="sxs-lookup"><span data-stu-id="bb409-115">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="bb409-116">`nextLink` (**デルタ**関数の呼び出しと _skipToken_ を使用した URL を含む)、または</span><span class="sxs-lookup"><span data-stu-id="bb409-116">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="bb409-117">`deltaLink` (**デルタ**関数の呼び出しと _deltaToken_ を使用した URL を含む)。</span><span class="sxs-lookup"><span data-stu-id="bb409-117">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="bb409-118">これらのトークンは、refs/remotes/microsoftgraph/master _startDateTime_ パラメーターと _endDateTime_ パラメーター、最初のデルタ クエリの GET 要求内の他のすべてのクエリ パラメーターをエンコードする[状態トークン](delta-query-overview.md#state-tokens)です。</span><span class="sxs-lookup"><span data-stu-id="bb409-118">These tokens are [state tokens](delta-query-overview.md#state-tokens) which encode the refs/remotes/microsoftgraph/master _startDateTime_ and _endDateTime_ parameters, and any other query parameter in your initial delta query GET request.</span></span> 

<span data-ttu-id="bb409-p105">状態トークンは、クライアントに対して完全に不透明です。変更追跡のラウンドを続行する手順は、最後の GET 要求から返された `nextLink` または `deltaLink` の URL を、その同じカレンダー ビューの次の**デルタ**関数呼び出しにコピーして適用するだけです。応答で返される `deltaLink` は、変更追跡の現在のラウンドが完了したことを示します。`deltaLink` URL を保存して、次のラウンドを開始する際に使用することができます。</span><span class="sxs-lookup"><span data-stu-id="bb409-p105">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next **delta** function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="bb409-123">これらの `nextLink` と `deltaLink` の URL を使用する方法については、以下の[例](#example-to-synchronize-events-in-a-calendar-view)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb409-123">See the [example](#example-to-synchronize-events-in-a-calendar-view) below to learn how to use these `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a><span data-ttu-id="bb409-124">カレンダー ビューのデルタ クエリでクエリ パラメーターを使用する</span><span class="sxs-lookup"><span data-stu-id="bb409-124">Use query parameters in a delta query for calendar view</span></span>

- <span data-ttu-id="bb409-125">_startDateTime_ パラメーターと _endDateTime_ パラメーターを含めて、カレンダー ビューの日付/時刻範囲を定義します。</span><span class="sxs-lookup"><span data-stu-id="bb409-125">Include the _startDateTime_ and _endDateTime_ parameters to define a date/time range for your calendar view.</span></span>
- <span data-ttu-id="bb409-126">`$select` はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb409-126">`$select` is not supported.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="bb409-127">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb409-127">Optional request header</span></span>

<span data-ttu-id="bb409-128">各デルタ クエリの GET 要求は、応答で 1 つ以上のイベントのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bb409-128">Each delta query GET request returns a collection of one or more events in the response.</span></span> <span data-ttu-id="bb409-129">必要に応じて、要求ヘッダー `Prefer: odata.maxpagesize={x}` を指定して、応答内の最大イベント数を設定できます。</span><span class="sxs-lookup"><span data-stu-id="bb409-129">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of events in a response.</span></span>


## <a name="example-to-synchronize-events-in-a-calendar-view"></a><span data-ttu-id="bb409-130">カレンダー ビューでのイベント同期の例</span><span class="sxs-lookup"><span data-stu-id="bb409-130">Example to synchronize events in a calendar view</span></span>

<span data-ttu-id="bb409-p107">次の例では、特定の時間範囲にあるユーザーの既定のカレンダーを同期するための一連の 3 つの要求を示します。そのカレンダー ビューには 5 つのイベントがあります。</span><span class="sxs-lookup"><span data-stu-id="bb409-p107">The following example shows a series of 3 requests to synchronize the user's default calendar in a specific time range. There are 5 events in that calendar view.</span></span>

- <span data-ttu-id="bb409-133">[手順 1: サンプルの最初の要求](#step-1-sample-initial-request)と[応答](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="bb409-133">[Step 1: sample initial request](#step-1-sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="bb409-134">[手順 2: サンプルの 2 番目の要求](#step-2-sample-second-request)と[応答](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="bb409-134">[Step 2: sample second request](#step-2-sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="bb409-135">[手順 3: サンプルの 3 番目の要求](#step-3-sample-third-request)と[最後の応答](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="bb409-135">[Step 3: sample third request](#step-3-sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="bb409-p108">簡潔にするため、サンプルの応答にはイベントのプロパティのサブセットのみを表示します。実際の呼び出しでは、ほとんどのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bb409-p108">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span> 

<span data-ttu-id="bb409-138">[次のラウンド](#the-next-round-sample-first-response)で行う操作も参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb409-138">See also what you'll do in the [next round](#the-next-round-sample-first-response).</span></span>


### <a name="step-1-sample-initial-request"></a><span data-ttu-id="bb409-139">手順 1: 最初の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="bb409-139">Step 1: sample initial request</span></span>

<span data-ttu-id="bb409-p109">この例では、指定されたカレンダー ビューは初めて同期されるため、最初の同期要求には状態トークンは含まれません。このラウンドは、そのカレンダー ビュー内のすべてのイベントを返します。</span><span class="sxs-lookup"><span data-stu-id="bb409-p109">In this example, the specified calendar view is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="bb409-142">最初の要求では、次を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb409-142">The first request specifies the following:</span></span>

- <span data-ttu-id="bb409-143">_startDateTime_ パラメーターと _endDateTime_ パラメーターの日付/時刻の値。</span><span class="sxs-lookup"><span data-stu-id="bb409-143">Date/time values for the _startDateTime_ and _endDateTime_ parameters.</span></span>
- <span data-ttu-id="bb409-144">[オプションの要求ヘッダー](#optional-request-header)である _odata.maxpagesize_ が一度に 2 つのイベントを返します。</span><span class="sxs-lookup"><span data-stu-id="bb409-144">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 events at a time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bb409-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb409-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb409-146">C#</span><span class="sxs-lookup"><span data-stu-id="bb409-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb409-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb409-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb409-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb409-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb409-149">Java</span><span class="sxs-lookup"><span data-stu-id="bb409-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="sample-initial-response"></a><span data-ttu-id="bb409-150">最初の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="bb409-150">Sample initial response</span></span>

<span data-ttu-id="bb409-p110">応答には、2 つのイベントと `skipToken` のある `@odata.nextLink` 応答ヘッダーが含まれています。`nextLink` URL は、取得するカレンダー ビューにさらにイベントがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="bb409-p110">The response includes two events and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more events in the calendar view to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIQ==\"",
            "subject":"Plan shopping list",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-09T20:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-09T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },      
            "id":"AAMkADNVxRAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIg==\"",
            "subject":"Pick up car",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T01:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxSAAA="
        }
    ]
}
```

### <a name="step-2-sample-second-request"></a><span data-ttu-id="bb409-153">手順 2: 2 番目の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="bb409-153">Step 2: sample second request</span></span>

<span data-ttu-id="bb409-p111">2 番目の要求では、前の応答で返された `nextLink` URL を指定します。最初の要求にあるような同じ _startDateTime_ パラメーターと _endDateTime_ パラメーターを指定する必要はなくなりましたのでご注意ください。これは、`nextLink` URL の `skipToken` によってこれらのパラメーターがエンコードされて含まれるためです。</span><span class="sxs-lookup"><span data-stu-id="bb409-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same _startDateTime_ and _endDateTime_ parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bb409-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb409-156">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb409-157">C#</span><span class="sxs-lookup"><span data-stu-id="bb409-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb409-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb409-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb409-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb409-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb409-160">Java</span><span class="sxs-lookup"><span data-stu-id="bb409-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-second-response"></a><span data-ttu-id="bb409-161">2 番目の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="bb409-161">Sample second response</span></span> 

<span data-ttu-id="bb409-162">2 番目の応答は、カレンダー ビューから取得するイベントがまだあることを示す、カレンダー ビュー内の次の 2 つのイベントと別の `nextLink` を返します。</span><span class="sxs-lookup"><span data-stu-id="bb409-162">The second response returns the next 2 events in the calendar view and another `nextLink`, indicating there are more events to get from the calendar view.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIw==\"",
            "subject":"Get food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T19:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T21:30:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxTAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvJA==\"",
            "subject":"Prepare food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-11T00:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxUAAA="
        }
    ]
}
```


### <a name="step-3-sample-third-request"></a><span data-ttu-id="bb409-163">手順 3: 3 番目の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="bb409-163">Step 3: sample third request</span></span>

<span data-ttu-id="bb409-164">3 番目の要求は、最後の同期要求から返された最新の `nextLink` を引き続き使用します。</span><span class="sxs-lookup"><span data-stu-id="bb409-164">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span> 
 


# <a name="httptabhttp"></a>[<span data-ttu-id="bb409-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb409-165">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb409-166">C#</span><span class="sxs-lookup"><span data-stu-id="bb409-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb409-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb409-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb409-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb409-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb409-169">Java</span><span class="sxs-lookup"><span data-stu-id="bb409-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-third-and-final-response"></a><span data-ttu-id="bb409-170">3 番目と最後の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="bb409-170">Sample third and final response</span></span>

<span data-ttu-id="bb409-p112">3 番目の応答では、カレンダー ビューに残っている 1 つだけのイベントと、このカレンダー ビューの同期が完了したことを示す `deltaLink` URL が返されます。`deltaLink` URL を保存して、[次のラウンドでそのカレンダー ビューを同期するために使用します](#the-next-round-sample-first-request)。</span><span class="sxs-lookup"><span data-stu-id="bb409-p112">The third response returns the only remaining event in the calendar view, and a `deltaLink` URL which indicates synchronization is complete for this calendar view. Save and use the `deltaLink` URL to [synchronize that calendar view in the next round](#the-next-round-sample-first-request).</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97g==\"",
            "subject":"Rest!",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-12T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-12T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Home"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HuAAA="
        }
    ]
}
```


### <a name="the-next-round-sample-first-request"></a><span data-ttu-id="bb409-173">次のラウンド: 最初の要求のサンプル</span><span class="sxs-lookup"><span data-stu-id="bb409-173">The next round: sample first request</span></span>

<span data-ttu-id="bb409-p113">最後のラウンドの[最後の応答](#step-3-sample-third-request)からの `deltaLink` を使用すると、それ以降にそのカレンダー ビューで (追加、削除、または更新によって) 変更されたこれらのイベントのみを取得できます。次のラウンドの最初の要求は、同じ最大ページ サイズを維持することを前提とすると、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="bb409-p113">Using the `deltaLink` from the [last request](#step-3-sample-third-request) in the last round, you will be able to get only those events that have changed (by being added, deleted, or updated) in that calendar view since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bb409-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb409-176">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb409-177">C#</span><span class="sxs-lookup"><span data-stu-id="bb409-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-next-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb409-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb409-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-next-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb409-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb409-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-next-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb409-180">Java</span><span class="sxs-lookup"><span data-stu-id="bb409-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-next-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="the-next-round-sample-first-response"></a><span data-ttu-id="bb409-181">次のラウンド: 最初の応答のサンプル</span><span class="sxs-lookup"><span data-stu-id="bb409-181">The next round: sample first response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcFuQtZdtpk4",
    "value":[
        {
            "@odata.type": "#microsoft.graph.event",
            "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS04OGQLkRkXbBznTvAADb6ytyAAA=",
            "@removed": {
                "reason": "deleted"
            }
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97w==\"",
            "subject":"Attend service",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-25T06:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-25T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Chapel of Saint Ignatius",
                "address":{
                    "street":"900 Broadway",
                    "city":"Seattle",
                    "state":"WA",
                    "countryOrRegion":"United States",
                    "postalCode":""
                },
                "coordinates":{
                    "latitude":47.6105,
                    "longitude":-122.321
                }
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HvAAA="
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="bb409-182">関連項目</span><span class="sxs-lookup"><span data-stu-id="bb409-182">See also</span></span>

- [<span data-ttu-id="bb409-183">Microsoft Graph デルタ クエリ</span><span class="sxs-lookup"><span data-stu-id="bb409-183">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="bb409-184">メッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="bb409-184">Get incremental changes to messages</span></span>](delta-query-messages.md)
- [<span data-ttu-id="bb409-185">グループに対する増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="bb409-185">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="bb409-186">ユーザーへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="bb409-186">Get incremental changes to users</span></span>](delta-query-users.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example to synchronize events in a calendar view",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
