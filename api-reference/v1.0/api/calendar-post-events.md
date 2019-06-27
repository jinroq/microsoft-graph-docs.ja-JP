---
title: イベントの作成
description: この API を使用して、既定または指定の予定表に新しいイベントを作成します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 1dec239f6da7a5053ac9cbfb02b761cefb67dcf2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264758"
---
# <a name="create-event"></a><span data-ttu-id="67bcb-103">イベントの作成</span><span class="sxs-lookup"><span data-stu-id="67bcb-103">Create event</span></span>

<span data-ttu-id="67bcb-104">この API を使用して、既定または指定の予定表に新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="67bcb-104">Use this API to create a new event in the default or specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="67bcb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67bcb-105">Permissions</span></span>
<span data-ttu-id="67bcb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67bcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67bcb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67bcb-108">Permission type</span></span>      | <span data-ttu-id="67bcb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67bcb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67bcb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67bcb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67bcb-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67bcb-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="67bcb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67bcb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67bcb-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67bcb-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="67bcb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67bcb-114">Application</span></span> | <span data-ttu-id="67bcb-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67bcb-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="67bcb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67bcb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="67bcb-117">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="67bcb-117">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="67bcb-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="67bcb-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="67bcb-119">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="67bcb-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="67bcb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67bcb-120">Request headers</span></span>
| <span data-ttu-id="67bcb-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67bcb-121">Header</span></span>       | <span data-ttu-id="67bcb-122">値</span><span class="sxs-lookup"><span data-stu-id="67bcb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67bcb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67bcb-123">Authorization</span></span>  | <span data-ttu-id="67bcb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="67bcb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="67bcb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67bcb-126">Content-Type</span></span>  | <span data-ttu-id="67bcb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="67bcb-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67bcb-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="67bcb-129">Request body</span></span>
<span data-ttu-id="67bcb-130">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67bcb-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="67bcb-131">応答</span><span class="sxs-lookup"><span data-stu-id="67bcb-131">Response</span></span>

<span data-ttu-id="67bcb-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="67bcb-132">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67bcb-133">例</span><span class="sxs-lookup"><span data-stu-id="67bcb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67bcb-134">要求</span><span class="sxs-lookup"><span data-stu-id="67bcb-134">Request</span></span>
<span data-ttu-id="67bcb-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67bcb-135">Here is an example of the request.</span></span>
<span data-ttu-id="67bcb-136">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67bcb-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
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

##### <a name="response"></a><span data-ttu-id="67bcb-137">応答</span><span class="sxs-lookup"><span data-stu-id="67bcb-137">Response</span></span>
<span data-ttu-id="67bcb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67bcb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="67bcb-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="67bcb-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="67bcb-142">C#</span><span class="sxs-lookup"><span data-stu-id="67bcb-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_event_from_calendar-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67bcb-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="67bcb-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_event_from_calendar-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="67bcb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67bcb-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_event_from_calendar-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendar-post-events.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendar-post-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendar-post-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
