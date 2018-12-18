---
title: イベントを一覧表示する
description: 予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。
author: angelgolfer-ms
ms.openlocfilehash: 3cf431d600f36350d8654e9624b596222fcbff8b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341882"
---
# <a name="list-events"></a><span data-ttu-id="78c35-104">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="78c35-104">List events</span></span>

> <span data-ttu-id="78c35-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78c35-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78c35-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78c35-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78c35-p103">予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78c35-p103">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="78c35-109">拡張イベントのインスタンスを取得すると、[予定表ビューを取得する](calendar-list-calendarview.md)または[イベントのインスタンスを取得する](event-list-instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="78c35-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="78c35-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="78c35-110">Permissions</span></span>
<span data-ttu-id="78c35-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78c35-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78c35-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78c35-113">Permission type</span></span>      | <span data-ttu-id="78c35-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="78c35-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78c35-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78c35-115">Delegated (work or school account)</span></span> | <span data-ttu-id="78c35-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="78c35-116">Calendars.Read</span></span>    |
|<span data-ttu-id="78c35-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78c35-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78c35-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="78c35-118">Calendars.Read</span></span>    |
|<span data-ttu-id="78c35-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78c35-119">Application</span></span> | <span data-ttu-id="78c35-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="78c35-120">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="78c35-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78c35-121">HTTP request</span></span>
<span data-ttu-id="78c35-122"><!-- { "blockType": "ignored" } -->ユーザーまたはグループの既定の[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="78c35-122"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="78c35-123">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="78c35-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="78c35-124">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="78c35-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78c35-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="78c35-125">Optional query parameters</span></span>
<span data-ttu-id="78c35-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="78c35-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="78c35-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78c35-127">Request headers</span></span>
| <span data-ttu-id="78c35-128">名前</span><span class="sxs-lookup"><span data-stu-id="78c35-128">Name</span></span>       | <span data-ttu-id="78c35-129">種類</span><span class="sxs-lookup"><span data-stu-id="78c35-129">Type</span></span> | <span data-ttu-id="78c35-130">説明</span><span class="sxs-lookup"><span data-stu-id="78c35-130">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="78c35-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="78c35-131">Authorization</span></span>  | <span data-ttu-id="78c35-132">string</span><span class="sxs-lookup"><span data-stu-id="78c35-132">string</span></span> | <span data-ttu-id="78c35-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="78c35-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="78c35-135">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="78c35-135">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="78c35-136">string</span><span class="sxs-lookup"><span data-stu-id="78c35-136">string</span></span> | <span data-ttu-id="78c35-137">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="78c35-137">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="78c35-138">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="78c35-138">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="78c35-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="78c35-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78c35-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="78c35-140">Request body</span></span>
<span data-ttu-id="78c35-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="78c35-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78c35-142">応答</span><span class="sxs-lookup"><span data-stu-id="78c35-142">Response</span></span>

<span data-ttu-id="78c35-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="78c35-143">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78c35-144">例</span><span class="sxs-lookup"><span data-stu-id="78c35-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78c35-145">要求</span><span class="sxs-lookup"><span data-stu-id="78c35-145">Request</span></span>
<span data-ttu-id="78c35-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78c35-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="78c35-147">応答</span><span class="sxs-lookup"><span data-stu-id="78c35-147">Response</span></span>
<span data-ttu-id="78c35-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="78c35-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
