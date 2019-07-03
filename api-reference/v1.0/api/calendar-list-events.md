---
title: イベントを一覧表示する
description: 予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: a8fbac941f4eb045d46572716242c03425b152c4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443814"
---
# <a name="list-events"></a><span data-ttu-id="d0e76-104">イベントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d0e76-104">List events</span></span>

<span data-ttu-id="d0e76-p102">予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d0e76-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="d0e76-107">拡張イベントのインスタンスを取得すると、[予定表ビューを取得する](calendar-list-calendarview.md)または[イベントのインスタンスを取得する](event-list-instances.md)ことができます。</span><span class="sxs-lookup"><span data-stu-id="d0e76-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0e76-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d0e76-108">Permissions</span></span>
<span data-ttu-id="d0e76-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0e76-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0e76-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0e76-111">Permission type</span></span>      | <span data-ttu-id="d0e76-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0e76-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0e76-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0e76-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d0e76-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d0e76-114">Calendars.Read</span></span>    |
|<span data-ttu-id="d0e76-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0e76-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0e76-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d0e76-116">Calendars.Read</span></span>    |
|<span data-ttu-id="d0e76-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0e76-117">Application</span></span> | <span data-ttu-id="d0e76-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d0e76-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0e76-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0e76-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d0e76-120">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d0e76-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="d0e76-121">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d0e76-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="d0e76-122">指定の [calendarGroup](../resources/calendargroup.md) のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d0e76-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d0e76-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d0e76-123">Optional query parameters</span></span>
<span data-ttu-id="d0e76-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d0e76-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d0e76-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0e76-125">Request headers</span></span>
| <span data-ttu-id="d0e76-126">名前</span><span class="sxs-lookup"><span data-stu-id="d0e76-126">Name</span></span>       | <span data-ttu-id="d0e76-127">型</span><span class="sxs-lookup"><span data-stu-id="d0e76-127">Type</span></span> | <span data-ttu-id="d0e76-128">説明</span><span class="sxs-lookup"><span data-stu-id="d0e76-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d0e76-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0e76-129">Authorization</span></span>  | <span data-ttu-id="d0e76-130">string</span><span class="sxs-lookup"><span data-stu-id="d0e76-130">string</span></span> | <span data-ttu-id="d0e76-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d0e76-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d0e76-133">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d0e76-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d0e76-134">string</span><span class="sxs-lookup"><span data-stu-id="d0e76-134">string</span></span> | <span data-ttu-id="d0e76-135">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="d0e76-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d0e76-136">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="d0e76-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d0e76-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d0e76-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0e76-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0e76-138">Request body</span></span>
<span data-ttu-id="d0e76-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d0e76-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0e76-140">応答</span><span class="sxs-lookup"><span data-stu-id="d0e76-140">Response</span></span>

<span data-ttu-id="d0e76-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d0e76-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0e76-142">例</span><span class="sxs-lookup"><span data-stu-id="d0e76-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0e76-143">要求</span><span class="sxs-lookup"><span data-stu-id="d0e76-143">Request</span></span>
<span data-ttu-id="d0e76-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0e76-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d0e76-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0e76-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d0e76-146">C#</span><span class="sxs-lookup"><span data-stu-id="d0e76-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0e76-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0e76-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d0e76-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0e76-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0e76-149">応答</span><span class="sxs-lookup"><span data-stu-id="d0e76-149">Response</span></span>
<span data-ttu-id="d0e76-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d0e76-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
