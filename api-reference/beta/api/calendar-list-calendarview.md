---
title: calendarView を一覧表示する
description: 時間範囲で定義した予定表ビューから、予定、例外、およびイベントの単一インスタンスを取得し、
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e951fb8fdf06d2fa6cf3edd312fb7843ae24d8aa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419133"
---
# <a name="list-calendarview"></a><span data-ttu-id="48f7c-103">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="48f7c-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48f7c-104">ユーザーの既定の予定表`(../me/calendarview)`またはユーザーのその他の予定表から、時間範囲で定義された予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="48f7c-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="48f7c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48f7c-105">Permissions</span></span>
<span data-ttu-id="48f7c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48f7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48f7c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48f7c-108">Permission type</span></span>      | <span data-ttu-id="48f7c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48f7c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48f7c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48f7c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48f7c-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f7c-111">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="48f7c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48f7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f7c-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f7c-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="48f7c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48f7c-114">Application</span></span> | <span data-ttu-id="48f7c-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f7c-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="48f7c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48f7c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="48f7c-117">ユーザーの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="48f7c-117">A user's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="48f7c-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="48f7c-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="48f7c-119">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="48f7c-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="48f7c-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="48f7c-120">Query parameters</span></span>

<span data-ttu-id="48f7c-121">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="48f7c-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="48f7c-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="48f7c-122">Parameter</span></span>    | <span data-ttu-id="48f7c-123">型</span><span class="sxs-lookup"><span data-stu-id="48f7c-123">Type</span></span>   |<span data-ttu-id="48f7c-124">説明</span><span class="sxs-lookup"><span data-stu-id="48f7c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48f7c-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="48f7c-125">startDateTime</span></span>|<span data-ttu-id="48f7c-126">String</span><span class="sxs-lookup"><span data-stu-id="48f7c-126">String</span></span>|<span data-ttu-id="48f7c-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="48f7c-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="48f7c-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="48f7c-129">endDateTime</span></span>|<span data-ttu-id="48f7c-130">String</span><span class="sxs-lookup"><span data-stu-id="48f7c-130">String</span></span>|<span data-ttu-id="48f7c-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="48f7c-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="48f7c-133">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)の一部もサポートしています。</span><span class="sxs-lookup"><span data-stu-id="48f7c-133">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="48f7c-134">[イベント](../resources/event.md)の**lastModifiedDateTime**プロパティは、をサポート\*\*\*\* `$select`していません。</span><span class="sxs-lookup"><span data-stu-id="48f7c-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="48f7c-135">値を取得するには、 **calendarView**を適用`$select`せずに単にクエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="48f7c-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48f7c-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48f7c-136">Request headers</span></span>
| <span data-ttu-id="48f7c-137">名前</span><span class="sxs-lookup"><span data-stu-id="48f7c-137">Name</span></span>       | <span data-ttu-id="48f7c-138">型</span><span class="sxs-lookup"><span data-stu-id="48f7c-138">Type</span></span> | <span data-ttu-id="48f7c-139">説明</span><span class="sxs-lookup"><span data-stu-id="48f7c-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="48f7c-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="48f7c-140">Authorization</span></span>  | <span data-ttu-id="48f7c-141">string</span><span class="sxs-lookup"><span data-stu-id="48f7c-141">string</span></span> | <span data-ttu-id="48f7c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="48f7c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48f7c-144">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="48f7c-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="48f7c-145">string</span><span class="sxs-lookup"><span data-stu-id="48f7c-145">string</span></span> | <span data-ttu-id="48f7c-146">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="48f7c-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="48f7c-147">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="48f7c-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="48f7c-148">省略可能。</span><span class="sxs-lookup"><span data-stu-id="48f7c-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48f7c-149">要求本文</span><span class="sxs-lookup"><span data-stu-id="48f7c-149">Request body</span></span>
<span data-ttu-id="48f7c-150">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="48f7c-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48f7c-151">応答</span><span class="sxs-lookup"><span data-stu-id="48f7c-151">Response</span></span>

<span data-ttu-id="48f7c-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="48f7c-152">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48f7c-153">例</span><span class="sxs-lookup"><span data-stu-id="48f7c-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48f7c-154">要求</span><span class="sxs-lookup"><span data-stu-id="48f7c-154">Request</span></span>
<span data-ttu-id="48f7c-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="48f7c-155">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48f7c-156">プロトコル</span><span class="sxs-lookup"><span data-stu-id="48f7c-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48f7c-157">C#</span><span class="sxs-lookup"><span data-stu-id="48f7c-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48f7c-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48f7c-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48f7c-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="48f7c-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="48f7c-160">応答</span><span class="sxs-lookup"><span data-stu-id="48f7c-160">Response</span></span>
<span data-ttu-id="48f7c-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48f7c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
