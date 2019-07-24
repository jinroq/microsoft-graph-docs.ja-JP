---
title: calendarView を一覧表示する
description: 時間範囲で定義した予定表ビューから、予定、例外、およびイベントの単一インスタンスを取得し、
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5f3b3c263ffd4f4a7a2a4663b087527791685573
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820662"
---
# <a name="list-calendarview"></a><span data-ttu-id="b09c5-103">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b09c5-103">List calendarView</span></span>

<span data-ttu-id="b09c5-104">ユーザーまたはグループの既定の予定表 `(../me/calendarview)` またはユーザーが所有する他の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="b09c5-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="b09c5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b09c5-105">Permissions</span></span>
<span data-ttu-id="b09c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b09c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="b09c5-108">ユーザーの予定表のイベント:Calendars.Read または Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b09c5-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="b09c5-109">グループの予定表のイベント:Group.Read.All または Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b09c5-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b09c5-110">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b09c5-110">HTTP request</span></span>

<span data-ttu-id="b09c5-111">ユーザーまたはグループの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b09c5-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b09c5-112">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b09c5-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b09c5-113">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b09c5-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="b09c5-114">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b09c5-114">Query parameters</span></span>

<span data-ttu-id="b09c5-115">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="b09c5-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="b09c5-116">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b09c5-116">Parameter</span></span>    | <span data-ttu-id="b09c5-117">型</span><span class="sxs-lookup"><span data-stu-id="b09c5-117">Type</span></span>   |<span data-ttu-id="b09c5-118">説明</span><span class="sxs-lookup"><span data-stu-id="b09c5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b09c5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b09c5-119">startDateTime</span></span>|<span data-ttu-id="b09c5-120">String</span><span class="sxs-lookup"><span data-stu-id="b09c5-120">String</span></span>|<span data-ttu-id="b09c5-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="b09c5-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="b09c5-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b09c5-123">endDateTime</span></span>|<span data-ttu-id="b09c5-124">String</span><span class="sxs-lookup"><span data-stu-id="b09c5-124">String</span></span>|<span data-ttu-id="b09c5-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="b09c5-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="b09c5-127">また、このメソッドは応答をカスタマイズするための一部の [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="b09c5-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="b09c5-128">[イベント](../resources/event.md)の **createdDateTime** プロパティおよび **lastModifiedDateTime** プロパティは、`$select` をサポートしません。</span><span class="sxs-lookup"><span data-stu-id="b09c5-128">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="b09c5-129">これらの値を取得するには、**calendarView** にクエリするだけで、`$select` を適用しません。</span><span class="sxs-lookup"><span data-stu-id="b09c5-129">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b09c5-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b09c5-130">Request headers</span></span>
| <span data-ttu-id="b09c5-131">名前</span><span class="sxs-lookup"><span data-stu-id="b09c5-131">Name</span></span>       | <span data-ttu-id="b09c5-132">型</span><span class="sxs-lookup"><span data-stu-id="b09c5-132">Type</span></span> | <span data-ttu-id="b09c5-133">説明</span><span class="sxs-lookup"><span data-stu-id="b09c5-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="b09c5-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="b09c5-134">Authorization</span></span>  | <span data-ttu-id="b09c5-135">string</span><span class="sxs-lookup"><span data-stu-id="b09c5-135">string</span></span> | <span data-ttu-id="b09c5-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b09c5-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b09c5-138">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b09c5-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="b09c5-139">string</span><span class="sxs-lookup"><span data-stu-id="b09c5-139">string</span></span> | <span data-ttu-id="b09c5-140">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="b09c5-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="b09c5-141">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="b09c5-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="b09c5-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b09c5-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b09c5-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="b09c5-143">Request body</span></span>
<span data-ttu-id="b09c5-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b09c5-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b09c5-145">応答</span><span class="sxs-lookup"><span data-stu-id="b09c5-145">Response</span></span>

<span data-ttu-id="b09c5-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b09c5-146">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b09c5-147">例</span><span class="sxs-lookup"><span data-stu-id="b09c5-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b09c5-148">要求</span><span class="sxs-lookup"><span data-stu-id="b09c5-148">Request</span></span>
<span data-ttu-id="b09c5-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b09c5-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b09c5-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="b09c5-150">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b09c5-151">C#</span><span class="sxs-lookup"><span data-stu-id="b09c5-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b09c5-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="b09c5-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b09c5-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b09c5-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b09c5-154">応答</span><span class="sxs-lookup"><span data-stu-id="b09c5-154">Response</span></span>
<span data-ttu-id="b09c5-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b09c5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "response-value",
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
