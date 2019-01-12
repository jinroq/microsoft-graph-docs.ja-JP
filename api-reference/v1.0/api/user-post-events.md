---
title: イベントを作成する
description: ユーザーの既定の予定表または指定した予定表でイベントを作成します。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef3ac07ba64115a10862cbdfb98dfbd63d2023ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978614"
---
# <a name="create-event"></a><span data-ttu-id="6778a-103">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="6778a-103">Create Event</span></span>

<span data-ttu-id="6778a-104">ユーザーの既定の予定表または指定した予定表で[イベント](../resources/event.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="6778a-104">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="6778a-105">**start** と **end** プロパティの型が [dateTimeTimeZone](../resources/datetimetimezone.md) であるため、これらの値の一部としてイベントの開始時刻と終了時刻のそれぞれにタイム ゾーンを指定できます。</span><span class="sxs-lookup"><span data-stu-id="6778a-105">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> 

<span data-ttu-id="6778a-106">イベントが送信されるとき、サーバーは出席者全員に招待状を送信します。</span><span class="sxs-lookup"><span data-stu-id="6778a-106">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="6778a-107">**イベントでの場所を設定する**</span><span class="sxs-lookup"><span data-stu-id="6778a-107">**Setting the location in an event**</span></span>

<span data-ttu-id="6778a-108">Exchange 管理者は、会議室などのリソースや、プロジェクターなどの機器用のメールボックスと電子メール アドレスを設定できます。</span><span class="sxs-lookup"><span data-stu-id="6778a-108">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="6778a-109">そうすると、ユーザーはリソースを参加者として会議に招待できます。</span><span class="sxs-lookup"><span data-stu-id="6778a-109">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="6778a-110">サーバーは、リソースに代わって、リソースの空き時間スケジュールに基づいて会議出席依頼を受諾あるいは拒否します。</span><span class="sxs-lookup"><span data-stu-id="6778a-110">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span> <span data-ttu-id="6778a-111">サーバーがリソースの会議参加を受諾すると、リソースの予定表に会議のイベントが作成されます。</span><span class="sxs-lookup"><span data-stu-id="6778a-111">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="6778a-112">会議の予定が変更されると、サーバーはリソースの予定表内のイベントを自動的に更新します。</span><span class="sxs-lookup"><span data-stu-id="6778a-112">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="6778a-113">リソースにメールボックスを設定するするもう 1 つの利点は、リソースのスケジュールを管理できることで、たとえば、あるプライベート会議用会議室は役員かその代理人しか予約できないようにできます。</span><span class="sxs-lookup"><span data-stu-id="6778a-113">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="6778a-114">会議する場所が必要になるイベントを開催する場合:</span><span class="sxs-lookup"><span data-stu-id="6778a-114">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="6778a-115">**event** の **location** プロパティを適宜設定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-115">Set the **location** property of the **event** accordingly.</span></span> 
2. <span data-ttu-id="6778a-116">会議場所にメール アドレスがある場合、オプションの **locationEmailAddress** プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-116">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="6778a-117">さらに、会議の開催場所がリソースとして設定されている場合、あるいはリソースとして設定されている装置がイベントに関わってくる場合は、以下のようにします。</span><span class="sxs-lookup"><span data-stu-id="6778a-117">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="6778a-118">リソースを[出席者](../resources/attendee.md)として招待します。</span><span class="sxs-lookup"><span data-stu-id="6778a-118">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="6778a-119">出席者の **type** プロパティを `resource` に設定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-119">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="6778a-120">出席者の **emailAddress** をリソースのメール アドレスとして設定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-120">Set the attendee **emailAddress** as the resource email address.</span></span>



## <a name="permissions"></a><span data-ttu-id="6778a-121">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6778a-121">Permissions</span></span>
<span data-ttu-id="6778a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6778a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6778a-124">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6778a-124">Permission type</span></span>      | <span data-ttu-id="6778a-125">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6778a-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6778a-126">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6778a-126">Delegated (work or school account)</span></span> | <span data-ttu-id="6778a-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6778a-127">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6778a-128">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6778a-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6778a-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6778a-129">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6778a-130">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6778a-130">Application</span></span> | <span data-ttu-id="6778a-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6778a-131">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6778a-132">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6778a-132">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="6778a-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6778a-133">Request headers</span></span>
| <span data-ttu-id="6778a-134">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6778a-134">Header</span></span>       | <span data-ttu-id="6778a-135">値</span><span class="sxs-lookup"><span data-stu-id="6778a-135">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="6778a-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="6778a-136">Authorization</span></span>  | <span data-ttu-id="6778a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6778a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6778a-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6778a-139">Content-Type</span></span>  | <span data-ttu-id="6778a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6778a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6778a-142">要求本文</span><span class="sxs-lookup"><span data-stu-id="6778a-142">Request body</span></span>
<span data-ttu-id="6778a-143">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-143">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="6778a-144">**イベント** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにイベントに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="6778a-144">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="6778a-145">応答</span><span class="sxs-lookup"><span data-stu-id="6778a-145">Response</span></span>

<span data-ttu-id="6778a-146">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6778a-146">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6778a-147">例</span><span class="sxs-lookup"><span data-stu-id="6778a-147">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6778a-148">要求 1</span><span class="sxs-lookup"><span data-stu-id="6778a-148">Request 1</span></span>
<span data-ttu-id="6778a-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6778a-149">Here is an example of the request.</span></span> <span data-ttu-id="6778a-150">`Prefer: outlook.timezone` 要求ヘッダーを使用して、応答の**開始**時刻と**終了**時刻に対するタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-150">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="6778a-151">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-151">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="6778a-152">応答 1</span><span class="sxs-lookup"><span data-stu-id="6778a-152">Response 1</span></span>
<span data-ttu-id="6778a-153">この応答の例には、`Prefer: outlook.timezone` ヘッダーに指定されているタイム ゾーンを使用した **start** および **end** プロパティが示されています。</span><span class="sxs-lookup"><span data-stu-id="6778a-153">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="6778a-154">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6778a-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6778a-155">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6778a-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="6778a-156">要求 2</span><span class="sxs-lookup"><span data-stu-id="6778a-156">Request 2</span></span>
<span data-ttu-id="6778a-157">次の要求の例では、3 つの場所を指定して、開催者と出席者がこれらの場所から会議に参加できるようにします。</span><span class="sxs-lookup"><span data-stu-id="6778a-157">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="6778a-158">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-158">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_multiple_locations"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 1390

{
  "subject": "Plan summer company picnic",
  "body": {
    "contentType": "HTML",
    "content": "Let's kick-start this event planning!"
  },
  "start": {
      "dateTime": "2017-08-30T11:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-08-30T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "DanaS@contoso.onmicrosoft.com",
        "name": "Dana Swope"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "AlexW@contoso.onmicrosoft.com",
        "name": "Alex Wilber"
      },
      "type": "Required"
    }
  ],
  "location": {
    "displayName": "Conf Room 3; Fourth Coffee; Home Office",
    "locationType": "Default"
  },
  "locations": [
    {
      "displayName": "Conf Room 3"
    },
    {
      "displayName": "Fourth Coffee",
      "address": {
        "street": "4567 Main St",
        "city": "Redmond",
        "state": "WA",
        "countryOrRegion": "US",
        "postalCode": "32008"
      },
      "coordinates": {
        "latitude": 47.672,
        "longitude": -102.103
      }
    },
    {
      "displayName": "Home Office"
    }
  ]

}
```

##### <a name="response-2"></a><span data-ttu-id="6778a-159">応答 2</span><span class="sxs-lookup"><span data-stu-id="6778a-159">Response 2</span></span>
<span data-ttu-id="6778a-160">次の応答の例には、会議の 3 つの場所に関する情報を指定する、作成されたイベントが示されています。</span><span class="sxs-lookup"><span data-stu-id="6778a-160">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="6778a-161">`Prefer: outlook.timezone="Pacific Standard Time"` 要求ヘッダーにより、**start** および **end** プロパティは PST で表記されています。</span><span class="sxs-lookup"><span data-stu-id="6778a-161">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="6778a-162">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6778a-162">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6778a-163">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6778a-163">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2985

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "createdDateTime":"2017-08-30T07:06:33.8673345Z",
  "lastModifiedDateTime":"2017-08-30T07:06:34.5079772Z",
  "changeKey":"y53lbKh6jkaxHzFwGhgyxgAAz3IKMA==",
  "categories":[

  ],
  "originalStartTimeZone":"Pacific Standard Time",
  "originalEndTimeZone":"Pacific Standard Time",
  "iCalUId":"04000000820089190544",
  "reminderMinutesBeforeStart":15,
  "isReminderOn":true,
  "hasAttachments":false,
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "importance":"normal",
  "sensitivity":"normal",
  "isAllDay":false,
  "isCancelled":false,
  "isOrganizer":true,
  "responseRequested":true,
  "seriesMasterId":null,
  "showAs":"busy",
  "type":"singleInstance",
  "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADAGAADDdm4NAAA%3D&exvsurl=1&path=/calendar/item",
  "onlineMeetingUrl":null,
  "responseStatus":{
    "response":"organizer",
    "time":"0001-01-01T00:00:00Z"
  },
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"Pacific Standard Time"
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
  "recurrence":null,
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


##### <a name="request-3"></a><span data-ttu-id="6778a-164">要求 3</span><span class="sxs-lookup"><span data-stu-id="6778a-164">Request 3</span></span>
<span data-ttu-id="6778a-165">3 つ目の例は、定期的なイベントを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6778a-165">The third example shows how to create a recurring event.</span></span> <span data-ttu-id="6778a-166">このイベントは、2017 年 9 月 4 日から年末まで、毎週月曜日の午後 0:00 から午後 2:00 に発生します。</span><span class="sxs-lookup"><span data-stu-id="6778a-166">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon time work for you?"
  },
  "start": {
      "dateTime": "2017-09-04T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-09-04T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "recurrence": {
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Monday" ]
    },
    "range": {
      "type": "endDate",
      "startDate": "2017-09-04",
      "endDate": "2017-12-31"
    }
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="6778a-167">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6778a-167">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="6778a-168">応答 3</span><span class="sxs-lookup"><span data-stu-id="6778a-168">Response 3</span></span>
<span data-ttu-id="6778a-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6778a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==\"",
    "id":"AAMkADQwMD",
    "createdDateTime":"2017-10-07T04:59:12.9698856Z",
    "lastModifiedDateTime":"2017-10-07T04:59:13.8136423Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E0080000000028CEBE04293FD3010000000000000000100000009F85AB8AF8ED4D4FAC777FA89954BDB7",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go for lunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMD&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start":{
        "dateTime":"2017-09-04T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-09-04T14:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar",
        "locationType":"default",
        "uniqueId":"Harry's Bar",
        "uniqueIdType":"private"
    },
    "locations":[
        {
            "displayName":"Harry's Bar",
            "locationType":"default",
            "uniqueIdType":"unknown"
        }
    ],
    "recurrence":{
        "pattern":{
            "type":"weekly",
            "interval":1,
            "month":0,
            "dayOfMonth":0,
            "daysOfWeek":[
                "monday"
            ],
            "firstDayOfWeek":"sunday",
            "index":"first"
        },
        "range":{
            "type":"endDate",
            "startDate":"2017-09-04",
            "endDate":"2017-12-31",
            "recurrenceTimeZone":"Pacific Standard Time",
            "numberOfOccurrences":0
        }
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
        }
    },
    "OnlineMeeting":null
}
```


## <a name="see-also"></a><span data-ttu-id="6778a-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="6778a-172">See also</span></span>

- [<span data-ttu-id="6778a-173">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="6778a-173">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6778a-174">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="6778a-174">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="6778a-175">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="6778a-175">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
