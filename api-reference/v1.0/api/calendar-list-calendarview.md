---
title: calendarView を一覧表示する
description: 時間範囲で定義した予定表ビューから、予定、例外、およびイベントの単一インスタンスを取得し、
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 43a0884e8b229facaf98c06160430fb087a89e87
ms.sourcegitcommit: eb5f63deafcdd6db44e791f2d1f4c46604ab06fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245573"
---
# <a name="list-calendarview"></a><span data-ttu-id="e422d-103">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e422d-103">List calendarView</span></span>

<span data-ttu-id="e422d-104">ユーザーの既定の予定表`(../me/calendarview)`またはユーザーが所有する他の予定表を元に、時間範囲で定義した予定表ビューから、イベントの発生、例外、および単一のインスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="e422d-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="e422d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e422d-105">Permissions</span></span>
<span data-ttu-id="e422d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e422d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e422d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e422d-108">Permission type</span></span>      | <span data-ttu-id="e422d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e422d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e422d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e422d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e422d-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e422d-111">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="e422d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e422d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e422d-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e422d-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e422d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e422d-114">Application</span></span> | <span data-ttu-id="e422d-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e422d-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e422d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e422d-116">HTTP request</span></span>

<span data-ttu-id="e422d-117">ユーザーの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="e422d-117">A user's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="e422d-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="e422d-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="e422d-119">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="e422d-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="e422d-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e422d-120">Query parameters</span></span>

<span data-ttu-id="e422d-121">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="e422d-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="e422d-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e422d-122">Parameter</span></span>    | <span data-ttu-id="e422d-123">型</span><span class="sxs-lookup"><span data-stu-id="e422d-123">Type</span></span>   |<span data-ttu-id="e422d-124">説明</span><span class="sxs-lookup"><span data-stu-id="e422d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e422d-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e422d-125">startDateTime</span></span>|<span data-ttu-id="e422d-126">String</span><span class="sxs-lookup"><span data-stu-id="e422d-126">String</span></span>|<span data-ttu-id="e422d-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="e422d-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="e422d-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e422d-129">endDateTime</span></span>|<span data-ttu-id="e422d-130">String</span><span class="sxs-lookup"><span data-stu-id="e422d-130">String</span></span>|<span data-ttu-id="e422d-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="e422d-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="e422d-133">また、このメソッドは応答をカスタマイズするための一部の [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="e422d-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="e422d-134">[イベント](../resources/event.md)の **createdDateTime** プロパティおよび **lastModifiedDateTime** プロパティは、`$select` をサポートしません。</span><span class="sxs-lookup"><span data-stu-id="e422d-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="e422d-135">これらの値を取得するには、**calendarView** にクエリするだけで、`$select` を適用しません。</span><span class="sxs-lookup"><span data-stu-id="e422d-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e422d-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e422d-136">Request headers</span></span>
| <span data-ttu-id="e422d-137">名前</span><span class="sxs-lookup"><span data-stu-id="e422d-137">Name</span></span>       | <span data-ttu-id="e422d-138">種類</span><span class="sxs-lookup"><span data-stu-id="e422d-138">Type</span></span> | <span data-ttu-id="e422d-139">説明</span><span class="sxs-lookup"><span data-stu-id="e422d-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="e422d-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="e422d-140">Authorization</span></span>  | <span data-ttu-id="e422d-141">string</span><span class="sxs-lookup"><span data-stu-id="e422d-141">string</span></span> | <span data-ttu-id="e422d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e422d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e422d-144">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e422d-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="e422d-145">string</span><span class="sxs-lookup"><span data-stu-id="e422d-145">string</span></span> | <span data-ttu-id="e422d-146">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="e422d-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e422d-147">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="e422d-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e422d-148">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e422d-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e422d-149">要求本文</span><span class="sxs-lookup"><span data-stu-id="e422d-149">Request body</span></span>
<span data-ttu-id="e422d-150">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e422d-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e422d-151">応答</span><span class="sxs-lookup"><span data-stu-id="e422d-151">Response</span></span>

<span data-ttu-id="e422d-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e422d-152">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e422d-153">例</span><span class="sxs-lookup"><span data-stu-id="e422d-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e422d-154">要求</span><span class="sxs-lookup"><span data-stu-id="e422d-154">Request</span></span>
<span data-ttu-id="e422d-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e422d-155">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e422d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="e422d-156">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e422d-157">C#</span><span class="sxs-lookup"><span data-stu-id="e422d-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e422d-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="e422d-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e422d-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e422d-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e422d-160">Java</span><span class="sxs-lookup"><span data-stu-id="e422d-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e422d-161">応答</span><span class="sxs-lookup"><span data-stu-id="e422d-161">Response</span></span>
<span data-ttu-id="e422d-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e422d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
