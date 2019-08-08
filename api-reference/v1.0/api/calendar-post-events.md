---
title: イベントの作成
description: この API を使用して、既定または指定の予定表に新しいイベントを作成します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 559c37348bd2b594e191ba04faf0668198c6e4dc
ms.sourcegitcommit: eb5f63deafcdd6db44e791f2d1f4c46604ab06fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245676"
---
# <a name="create-event"></a><span data-ttu-id="0c914-103">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="0c914-103">Create event</span></span>

<span data-ttu-id="0c914-104">この API を使用して、予定表に新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c914-104">Use this API to create a new Calendar in a calendar group.</span></span> <span data-ttu-id="0c914-105">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="0c914-105">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0c914-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c914-106">Permissions</span></span>
<span data-ttu-id="0c914-107">作成されたイベントが含まれている予定表の種類および要求されたアクセス許可の種類 (委任またはアプリケーション) に応じて、この API を呼び出すには、次のいずれかの権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c914-107">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="0c914-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c914-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c914-109">予定表</span><span class="sxs-lookup"><span data-stu-id="0c914-109">Calendar</span></span> | <span data-ttu-id="0c914-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c914-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c914-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c914-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c914-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c914-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="0c914-113">ユーザーの予定表</span><span class="sxs-lookup"><span data-stu-id="0c914-113">user calendar</span></span> | <span data-ttu-id="0c914-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c914-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="0c914-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c914-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="0c914-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c914-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="0c914-117">グループ予定表</span><span class="sxs-lookup"><span data-stu-id="0c914-117">group calendar</span></span> | <span data-ttu-id="0c914-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c914-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="0c914-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c914-119">Not supported.</span></span> | <span data-ttu-id="0c914-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c914-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c914-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c914-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0c914-122">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0c914-122">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="0c914-123">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0c914-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="0c914-124">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0c914-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="0c914-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c914-125">Request headers</span></span>
| <span data-ttu-id="0c914-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c914-126">Header</span></span>       | <span data-ttu-id="0c914-127">値</span><span class="sxs-lookup"><span data-stu-id="0c914-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c914-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c914-128">Authorization</span></span>  | <span data-ttu-id="0c914-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0c914-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c914-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c914-131">Content-Type</span></span>  | <span data-ttu-id="0c914-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0c914-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c914-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c914-134">Request body</span></span>
<span data-ttu-id="0c914-135">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c914-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0c914-136">応答</span><span class="sxs-lookup"><span data-stu-id="0c914-136">Response</span></span>

<span data-ttu-id="0c914-137">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c914-137">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c914-138">例</span><span class="sxs-lookup"><span data-stu-id="0c914-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c914-139">要求</span><span class="sxs-lookup"><span data-stu-id="0c914-139">Request</span></span>
<span data-ttu-id="0c914-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c914-140">Here is an example of the request.</span></span>
<span data-ttu-id="0c914-141">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c914-141">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c914-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c914-142">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does mid month work for you?"
  },
  "start": {
      "dateTime": "2019-03-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-15T14:00:00",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c914-143">C#</span><span class="sxs-lookup"><span data-stu-id="0c914-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c914-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c914-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c914-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c914-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c914-146">Java</span><span class="sxs-lookup"><span data-stu-id="0c914-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c914-147">応答</span><span class="sxs-lookup"><span data-stu-id="0c914-147">Response</span></span>
<span data-ttu-id="0c914-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c914-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA=",
    "createdDateTime": "2019-02-28T21:17:57.56197Z",
    "lastModifiedDateTime": "2019-02-28T21:17:59.044919Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E641B4C",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does mid month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes mid month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-15T14:00:00.0000000",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
