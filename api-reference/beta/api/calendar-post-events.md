---
title: イベントの作成
description: この API を使用して、既定または指定の予定表に新しいイベントを作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 042f3fba0f916dc709654b2492cc53834ca7c488
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419112"
---
# <a name="create-event"></a><span data-ttu-id="5e42e-103">イベントの作成</span><span class="sxs-lookup"><span data-stu-id="5e42e-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e42e-104">この API を使用して、予定表に新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="5e42e-104">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="5e42e-105">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5e42e-105">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="5e42e-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5e42e-106">Permissions</span></span>
<span data-ttu-id="5e42e-107">イベントが作成されたカレンダーの種類と、要求されたアクセス許可の種類 (委任またはアプリケーション) によっては、この API を呼び出すために次のいずれかのアクセス許可が必要になります。</span><span class="sxs-lookup"><span data-stu-id="5e42e-107">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="5e42e-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e42e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e42e-109">カレンダー</span><span class="sxs-lookup"><span data-stu-id="5e42e-109">Calendar</span></span> | <span data-ttu-id="5e42e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e42e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5e42e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e42e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e42e-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e42e-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="5e42e-113">ユーザーの予定表</span><span class="sxs-lookup"><span data-stu-id="5e42e-113">user calendar</span></span> | <span data-ttu-id="5e42e-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e42e-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="5e42e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e42e-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="5e42e-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e42e-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="5e42e-117">グループ calendar</span><span class="sxs-lookup"><span data-stu-id="5e42e-117">group calendar</span></span> | <span data-ttu-id="5e42e-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e42e-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="5e42e-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e42e-119">Not supported.</span></span> | <span data-ttu-id="5e42e-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e42e-120">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="5e42e-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e42e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="5e42e-122">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5e42e-122">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="5e42e-123">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5e42e-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="5e42e-124">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5e42e-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="5e42e-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e42e-125">Request headers</span></span>
| <span data-ttu-id="5e42e-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e42e-126">Header</span></span>       | <span data-ttu-id="5e42e-127">値</span><span class="sxs-lookup"><span data-stu-id="5e42e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e42e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e42e-128">Authorization</span></span>  | <span data-ttu-id="5e42e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5e42e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e42e-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e42e-131">Content-Type</span></span>  | <span data-ttu-id="5e42e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5e42e-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e42e-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e42e-134">Request body</span></span>
<span data-ttu-id="5e42e-135">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5e42e-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5e42e-136">応答</span><span class="sxs-lookup"><span data-stu-id="5e42e-136">Response</span></span>

<span data-ttu-id="5e42e-137">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5e42e-137">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e42e-138">例</span><span class="sxs-lookup"><span data-stu-id="5e42e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e42e-139">要求</span><span class="sxs-lookup"><span data-stu-id="5e42e-139">Request</span></span>
<span data-ttu-id="5e42e-140">次の例では、サインインしているユーザーの指定された予定表にイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="5e42e-140">The following example creates an event in the specified calendar of the signed-in user's.</span></span>

<span data-ttu-id="5e42e-141">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5e42e-141">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5e42e-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5e42e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does next month work for you?"
  },
  "start": {
      "dateTime": "2019-03-10T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-10T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e42e-143">C#</span><span class="sxs-lookup"><span data-stu-id="5e42e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e42e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e42e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e42e-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="5e42e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5e42e-146">応答</span><span class="sxs-lookup"><span data-stu-id="5e42e-146">Response</span></span>
<span data-ttu-id="5e42e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5e42e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA=",
    "createdDateTime": "2019-02-28T21:36:26.7105485Z",
    "lastModifiedDateTime": "2019-02-28T21:36:26.9577227Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200C780DAE",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does next month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes next month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-10T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-10T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
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
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Megan Bowen",
            "address": "MeganB@contoso.OnMicrosoft.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
