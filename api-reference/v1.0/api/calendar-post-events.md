---
title: イベントを作成する
description: この API を使用して、既定または指定の予定表に新しいイベントを作成します。
ms.openlocfilehash: da06df89ab4a62a1b767635e3daa928f84f29d9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022557"
---
# <a name="create-event"></a><span data-ttu-id="030ee-103">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="030ee-103">Create Event</span></span>

<span data-ttu-id="030ee-104">この API を使用して、既定または指定の予定表に新しいイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="030ee-104">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="030ee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="030ee-105">Permissions</span></span>
<span data-ttu-id="030ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="030ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="030ee-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="030ee-108">Permission type</span></span>      | <span data-ttu-id="030ee-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="030ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="030ee-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="030ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="030ee-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="030ee-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="030ee-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="030ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="030ee-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="030ee-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="030ee-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="030ee-114">Application</span></span> | <span data-ttu-id="030ee-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="030ee-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="030ee-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="030ee-116">HTTP request</span></span>
<span data-ttu-id="030ee-117"><!-- { "blockType": "ignored" } -->ユーザーまたはグループの既定の[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="030ee-117"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="030ee-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="030ee-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="030ee-119">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="030ee-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="030ee-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="030ee-120">Request headers</span></span>
| <span data-ttu-id="030ee-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="030ee-121">Header</span></span>       | <span data-ttu-id="030ee-122">値</span><span class="sxs-lookup"><span data-stu-id="030ee-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="030ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="030ee-123">Authorization</span></span>  | <span data-ttu-id="030ee-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="030ee-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="030ee-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="030ee-126">Content-Type</span></span>  | <span data-ttu-id="030ee-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="030ee-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="030ee-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="030ee-129">Request body</span></span>
<span data-ttu-id="030ee-130">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="030ee-130">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="030ee-131">応答</span><span class="sxs-lookup"><span data-stu-id="030ee-131">Response</span></span>

<span data-ttu-id="030ee-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="030ee-132">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="030ee-133">例</span><span class="sxs-lookup"><span data-stu-id="030ee-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="030ee-134">要求</span><span class="sxs-lookup"><span data-stu-id="030ee-134">Request</span></span>
<span data-ttu-id="030ee-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="030ee-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="030ee-136">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="030ee-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="030ee-137">応答</span><span class="sxs-lookup"><span data-stu-id="030ee-137">Response</span></span>
<span data-ttu-id="030ee-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="030ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
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