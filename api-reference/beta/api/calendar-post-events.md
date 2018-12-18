---
title: イベントを作成する
description: この API を使用して、既定または指定の予定表に新しいイベントを作成します。
author: angelgolfer-ms
ms.openlocfilehash: 136a4b6ead8789a162403364b5fc2d9d7a4a9997
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336737"
---
# <a name="create-event"></a><span data-ttu-id="9bd46-103">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="9bd46-103">Create Event</span></span>

> <span data-ttu-id="9bd46-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9bd46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bd46-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9bd46-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bd46-106">この API を使用して、既定または指定の予定表に新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="9bd46-106">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="9bd46-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9bd46-107">Permissions</span></span>
<span data-ttu-id="9bd46-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9bd46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bd46-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9bd46-110">Permission type</span></span>      | <span data-ttu-id="9bd46-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9bd46-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bd46-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9bd46-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9bd46-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bd46-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9bd46-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9bd46-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bd46-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bd46-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9bd46-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9bd46-116">Application</span></span> | <span data-ttu-id="9bd46-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bd46-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bd46-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9bd46-118">HTTP request</span></span>
<span data-ttu-id="9bd46-119"><!-- { "blockType": "ignored" } -->ユーザーまたはグループの既定の[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="9bd46-119"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="9bd46-120">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="9bd46-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="9bd46-121">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="9bd46-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="9bd46-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9bd46-122">Request headers</span></span>
| <span data-ttu-id="9bd46-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9bd46-123">Header</span></span>       | <span data-ttu-id="9bd46-124">値</span><span class="sxs-lookup"><span data-stu-id="9bd46-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9bd46-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bd46-125">Authorization</span></span>  | <span data-ttu-id="9bd46-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9bd46-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9bd46-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bd46-128">Content-Type</span></span>  | <span data-ttu-id="9bd46-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9bd46-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9bd46-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="9bd46-131">Request body</span></span>
<span data-ttu-id="9bd46-132">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9bd46-132">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9bd46-133">応答</span><span class="sxs-lookup"><span data-stu-id="9bd46-133">Response</span></span>

<span data-ttu-id="9bd46-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9bd46-134">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bd46-135">例</span><span class="sxs-lookup"><span data-stu-id="9bd46-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bd46-136">要求</span><span class="sxs-lookup"><span data-stu-id="9bd46-136">Request</span></span>
<span data-ttu-id="9bd46-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9bd46-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="9bd46-138">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9bd46-138">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9bd46-139">応答</span><span class="sxs-lookup"><span data-stu-id="9bd46-139">Response</span></span>
<span data-ttu-id="9bd46-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9bd46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
