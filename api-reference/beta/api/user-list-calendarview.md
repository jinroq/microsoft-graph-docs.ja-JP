---
title: calendarView を一覧表示する
description: 既定の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4abdda111c4bb00f1fe977413f3e6f5c686a812f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270211"
---
# <a name="list-calendarview"></a><span data-ttu-id="d502a-103">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d502a-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d502a-104">ユーザーの既定の予定表またはユーザーが所有する他の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d502a-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="d502a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d502a-105">Permissions</span></span>
<span data-ttu-id="d502a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d502a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d502a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d502a-108">Permission type</span></span>      | <span data-ttu-id="d502a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d502a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d502a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d502a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d502a-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d502a-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d502a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d502a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d502a-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d502a-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d502a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d502a-114">Application</span></span> | <span data-ttu-id="d502a-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d502a-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d502a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d502a-116">HTTP request</span></span>
<span data-ttu-id="d502a-117">ユーザーの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d502a-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d502a-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d502a-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d502a-119">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d502a-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="d502a-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d502a-120">Query parameters</span></span>

<span data-ttu-id="d502a-121">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="d502a-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d502a-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d502a-122">Parameter</span></span>    | <span data-ttu-id="d502a-123">型</span><span class="sxs-lookup"><span data-stu-id="d502a-123">Type</span></span>   |<span data-ttu-id="d502a-124">説明</span><span class="sxs-lookup"><span data-stu-id="d502a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d502a-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d502a-125">startDateTime</span></span>|<span data-ttu-id="d502a-126">String</span><span class="sxs-lookup"><span data-stu-id="d502a-126">String</span></span>|<span data-ttu-id="d502a-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="d502a-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d502a-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d502a-129">endDateTime</span></span>|<span data-ttu-id="d502a-130">String</span><span class="sxs-lookup"><span data-stu-id="d502a-130">String</span></span>|<span data-ttu-id="d502a-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="d502a-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d502a-133">また、このメソッドは応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="d502a-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d502a-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d502a-134">Request headers</span></span>
| <span data-ttu-id="d502a-135">名前</span><span class="sxs-lookup"><span data-stu-id="d502a-135">Name</span></span>       | <span data-ttu-id="d502a-136">型</span><span class="sxs-lookup"><span data-stu-id="d502a-136">Type</span></span> | <span data-ttu-id="d502a-137">説明</span><span class="sxs-lookup"><span data-stu-id="d502a-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d502a-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="d502a-138">Authorization</span></span>  | <span data-ttu-id="d502a-139">string</span><span class="sxs-lookup"><span data-stu-id="d502a-139">string</span></span> | <span data-ttu-id="d502a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d502a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d502a-142">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d502a-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d502a-143">string</span><span class="sxs-lookup"><span data-stu-id="d502a-143">string</span></span> | <span data-ttu-id="d502a-144">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="d502a-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d502a-145">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="d502a-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d502a-146">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d502a-146">Optional.</span></span> |
| <span data-ttu-id="d502a-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="d502a-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="d502a-148">string</span><span class="sxs-lookup"><span data-stu-id="d502a-148">string</span></span> | <span data-ttu-id="d502a-149">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="d502a-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="d502a-150">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="d502a-150">Values can be "text" or "html".</span></span> <span data-ttu-id="d502a-151">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="d502a-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="d502a-152">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d502a-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="d502a-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d502a-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d502a-154">要求本文</span><span class="sxs-lookup"><span data-stu-id="d502a-154">Request body</span></span>
<span data-ttu-id="d502a-155">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d502a-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d502a-156">応答</span><span class="sxs-lookup"><span data-stu-id="d502a-156">Response</span></span>

<span data-ttu-id="d502a-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d502a-157">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d502a-158">例</span><span class="sxs-lookup"><span data-stu-id="d502a-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d502a-159">要求</span><span class="sxs-lookup"><span data-stu-id="d502a-159">Request</span></span>
<span data-ttu-id="d502a-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d502a-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="d502a-161">応答</span><span class="sxs-lookup"><span data-stu-id="d502a-161">Response</span></span>
<span data-ttu-id="d502a-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d502a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d502a-165">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d502a-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d502a-166">C#</span><span class="sxs-lookup"><span data-stu-id="d502a-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendarview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d502a-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="d502a-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendarview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d502a-168">目的-C</span><span class="sxs-lookup"><span data-stu-id="d502a-168">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendarview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
