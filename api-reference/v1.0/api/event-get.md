---
title: イベントを取得する
description: 指定したイベント オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
ms.openlocfilehash: f83591e8315aed80fa650e7518bd7bf77e98882b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311026"
---
# <a name="get-event"></a><span data-ttu-id="b43a8-103">イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="b43a8-103">Get event</span></span>

<span data-ttu-id="b43a8-104">指定した[イベント](../resources/event.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="b43a8-104">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="b43a8-105">現在、この操作によって返されるイベントの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="b43a8-105">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="b43a8-106">2 つシナリオは、アプリケーションが別のユーザーの予定表でイベントを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="b43a8-106">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="b43a8-107">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="b43a8-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b43a8-108">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーとカレンダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="b43a8-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b43a8-109">[詳細と例](/graph/outlook-get-shared-events-calendars)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b43a8-109">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="b43a8-110">**イベント** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**イベント** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-110">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="b43a8-111">さまざまなタイム ゾーンをサポートします。</span><span class="sxs-lookup"><span data-stu-id="b43a8-111">Support various time zones</span></span>

<span data-ttu-id="b43a8-112">イベントを返す GET 操作の場合は、すべての操作で `Prefer: outlook.timezone` ヘッダーを使用して、応答のイベントの開始時刻と終了時刻のタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="b43a8-113">たとえば、次の `Prefer: outlook.timezone` ヘッダーは、応答の開始時刻と終了時刻を東部標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="b43a8-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="b43a8-p102">イベントが別のタイム ゾーンで作成された場合は、開始時刻と終了時刻は `Prefer` ヘッダーで指定したタイム ゾーンに合わせて調整されます。サポートされているタイム ゾーン名については、この[一覧](../resources/datetimetimezone.md)を参照してください。`Prefer: outlook.timezone` ヘッダーを指定しない場合、開始時刻と終了時刻は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="b43a8-117">**イベント**リソース上で **OriginalStartTimeZone** プロパティと **OriginalEndTimeZone** プロパティを使用して、イベント作成時に使用されたタイム ゾーンを検索できます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="b43a8-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b43a8-118">Permissions</span></span>
<span data-ttu-id="b43a8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b43a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b43a8-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b43a8-121">Permission type</span></span>      | <span data-ttu-id="b43a8-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b43a8-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b43a8-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b43a8-123">Delegated (work or school account)</span></span> | <span data-ttu-id="b43a8-124">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b43a8-124">Calendars.Read</span></span>    |
|<span data-ttu-id="b43a8-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b43a8-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b43a8-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b43a8-126">Calendars.Read</span></span>    |
|<span data-ttu-id="b43a8-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b43a8-127">Application</span></span> | <span data-ttu-id="b43a8-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b43a8-128">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b43a8-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b43a8-129">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="b43a8-130">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b43a8-130">Optional query parameters</span></span>
<span data-ttu-id="b43a8-131">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b43a8-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b43a8-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b43a8-132">Request headers</span></span>
| <span data-ttu-id="b43a8-133">名前</span><span class="sxs-lookup"><span data-stu-id="b43a8-133">Name</span></span>       | <span data-ttu-id="b43a8-134">種類</span><span class="sxs-lookup"><span data-stu-id="b43a8-134">Type</span></span> | <span data-ttu-id="b43a8-135">説明</span><span class="sxs-lookup"><span data-stu-id="b43a8-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="b43a8-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="b43a8-136">Authorization</span></span>  | <span data-ttu-id="b43a8-137">string</span><span class="sxs-lookup"><span data-stu-id="b43a8-137">string</span></span> | <span data-ttu-id="b43a8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b43a8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b43a8-140">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b43a8-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="b43a8-141">string</span><span class="sxs-lookup"><span data-stu-id="b43a8-141">string</span></span> | <span data-ttu-id="b43a8-142">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="b43a8-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="b43a8-143">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="b43a8-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b43a8-144">Optional.</span></span> |
| <span data-ttu-id="b43a8-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="b43a8-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="b43a8-146">string</span><span class="sxs-lookup"><span data-stu-id="b43a8-146">string</span></span> | <span data-ttu-id="b43a8-147">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="b43a8-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="b43a8-148">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="b43a8-148">Values can be "text" or "html".</span></span> <span data-ttu-id="b43a8-149">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="b43a8-150">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="b43a8-151">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b43a8-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b43a8-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="b43a8-152">Request body</span></span>
<span data-ttu-id="b43a8-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b43a8-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b43a8-154">応答</span><span class="sxs-lookup"><span data-stu-id="b43a8-154">Response</span></span>

<span data-ttu-id="b43a8-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b43a8-155">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b43a8-156">例</span><span class="sxs-lookup"><span data-stu-id="b43a8-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b43a8-157">要求 1</span><span class="sxs-lookup"><span data-stu-id="b43a8-157">Request 1</span></span>
<span data-ttu-id="b43a8-p107">最初の例では、指定されたイベントを取得します。以下のものを指定します。</span><span class="sxs-lookup"><span data-stu-id="b43a8-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="b43a8-160">太平洋標準時で返される日時の値を取得するための `Prefer: outlook.timezone` ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="b43a8-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="b43a8-p108">特定のプロパティを返すための `$select` クエリ パラメーター。`$select` パラメーターがない場合には、すべてのイベント プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGIAAAoZDOFAAA="],
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGIAAAoZDOFAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response-1"></a><span data-ttu-id="b43a8-163">応答 1</span><span class="sxs-lookup"><span data-stu-id="b43a8-163">Response 1</span></span>

<span data-ttu-id="b43a8-p109">以下は、応答の例です。**body** プロパティが HTML の既定の形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-p109">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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


##### <a name="request-2"></a><span data-ttu-id="b43a8-166">要求 2</span><span class="sxs-lookup"><span data-stu-id="b43a8-166">Request 2</span></span>

<span data-ttu-id="b43a8-167">2 番目の例では、複数の場所を指定するイベントを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b43a8-167">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="b43a8-168">この要求では、特定のプロパティを返すように `$select` クエリ パラメーターを指定しています。</span><span class="sxs-lookup"><span data-stu-id="b43a8-168">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADAGAADDdm4NAAA="],
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGAADDdm4NAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-2"></a><span data-ttu-id="b43a8-169">応答 2</span><span class="sxs-lookup"><span data-stu-id="b43a8-169">Response 2</span></span>
<span data-ttu-id="b43a8-170">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b43a8-170">Here is an example of the response.</span></span> <span data-ttu-id="b43a8-171">**locations** プロパティには、イベントを開催する 3 つの場所の詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b43a8-171">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="b43a8-172">要求では `Prefer: outlook.timezone` ヘッダーを指定していないため、**start** および **end** プロパティは既定の UTC タイム ゾーンで表示されます。</span><span class="sxs-lookup"><span data-stu-id="b43a8-172">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="b43a8-173">イベントの本文は、既定の HTML 形式になっています。</span><span class="sxs-lookup"><span data-stu-id="b43a8-173">The event body is in the default HTML format.</span></span>  

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



## <a name="see-also"></a><span data-ttu-id="b43a8-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="b43a8-174">See also</span></span>

- [<span data-ttu-id="b43a8-175">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="b43a8-175">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b43a8-176">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="b43a8-176">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b43a8-177">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="b43a8-177">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->