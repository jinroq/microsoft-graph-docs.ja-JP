---
title: イベントを一覧表示する
description: 予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 198c31d4778a7c84e0ca32dc549d2012c3b40dfc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419128"
---
# <a name="list-events"></a><span data-ttu-id="b0a07-104">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b0a07-104">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0a07-105">予定表のイベント一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b0a07-105">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="b0a07-106">[ユーザー](../resources/user.md)の予定表、または Office 365 [グループ](../resources/group.md)の既定の予定表のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="b0a07-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> <span data-ttu-id="b0a07-107">イベントの一覧には、単一のインスタンスの会議とシリーズのマスターシェイプが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b0a07-107">The list of events contains single instance meetings and series masters.</span></span>

<span data-ttu-id="b0a07-108">拡張イベントのインスタンスを取得すると、[予定表ビューを取得する](calendar-list-calendarview.md)または[イベントのインスタンスを取得する](event-list-instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="b0a07-108">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0a07-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0a07-109">Permissions</span></span>
<span data-ttu-id="b0a07-110">この API を呼び出すには、イベントが含まれる予定表の種類と、要求されたアクセス許可の種類 (委任またはアプリケーション) に応じて、次のいずれかのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0a07-110">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="b0a07-111">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0a07-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0a07-112">カレンダー</span><span class="sxs-lookup"><span data-stu-id="b0a07-112">Calendar</span></span> | <span data-ttu-id="b0a07-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0a07-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b0a07-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0a07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0a07-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0a07-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="b0a07-116">ユーザーの予定表</span><span class="sxs-lookup"><span data-stu-id="b0a07-116">user calendar</span></span> | <span data-ttu-id="b0a07-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0a07-117">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="b0a07-118">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0a07-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="b0a07-119">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0a07-119">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="b0a07-120">グループ calendar</span><span class="sxs-lookup"><span data-stu-id="b0a07-120">group calendar</span></span> | <span data-ttu-id="b0a07-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a07-121">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="b0a07-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0a07-122">Not supported.</span></span> | <span data-ttu-id="b0a07-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0a07-123">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="b0a07-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0a07-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b0a07-125">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b0a07-125">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="b0a07-126">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b0a07-126">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="b0a07-127">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b0a07-127">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0a07-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0a07-128">Optional query parameters</span></span>
<span data-ttu-id="b0a07-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b0a07-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b0a07-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0a07-130">Request headers</span></span>
| <span data-ttu-id="b0a07-131">名前</span><span class="sxs-lookup"><span data-stu-id="b0a07-131">Name</span></span>       | <span data-ttu-id="b0a07-132">型</span><span class="sxs-lookup"><span data-stu-id="b0a07-132">Type</span></span> | <span data-ttu-id="b0a07-133">説明</span><span class="sxs-lookup"><span data-stu-id="b0a07-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="b0a07-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0a07-134">Authorization</span></span>  | <span data-ttu-id="b0a07-135">string</span><span class="sxs-lookup"><span data-stu-id="b0a07-135">string</span></span> | <span data-ttu-id="b0a07-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0a07-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b0a07-138">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b0a07-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="b0a07-139">string</span><span class="sxs-lookup"><span data-stu-id="b0a07-139">string</span></span> | <span data-ttu-id="b0a07-140">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="b0a07-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="b0a07-141">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="b0a07-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="b0a07-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b0a07-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0a07-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0a07-143">Request body</span></span>
<span data-ttu-id="b0a07-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0a07-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0a07-145">応答</span><span class="sxs-lookup"><span data-stu-id="b0a07-145">Response</span></span>

<span data-ttu-id="b0a07-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b0a07-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0a07-147">例</span><span class="sxs-lookup"><span data-stu-id="b0a07-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0a07-148">要求</span><span class="sxs-lookup"><span data-stu-id="b0a07-148">Request</span></span>
<span data-ttu-id="b0a07-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0a07-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0a07-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b0a07-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0a07-151">C#</span><span class="sxs-lookup"><span data-stu-id="b0a07-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0a07-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0a07-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0a07-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="b0a07-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0a07-154">応答</span><span class="sxs-lookup"><span data-stu-id="b0a07-154">Response</span></span>
<span data-ttu-id="b0a07-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0a07-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
