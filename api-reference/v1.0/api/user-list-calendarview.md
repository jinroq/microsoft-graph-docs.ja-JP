---
title: calendarView を一覧表示する
description: 'ユーザーの既定の予定表からの時間の範囲で定義されている予定表ビューで出現する、例外、およびイベントの 1 つのインスタンスを取得します。 '
ms.openlocfilehash: db2c0b4d5fe2b3929aab7c30e00aff0f30dff5b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021080"
---
# <a name="list-calendarview"></a><span data-ttu-id="be6da-103">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="be6da-103">List calendarView</span></span>

<span data-ttu-id="be6da-104">ユーザーの既定の予定表またはユーザーが所有する他の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="be6da-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="be6da-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be6da-105">Permissions</span></span>
<span data-ttu-id="be6da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be6da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be6da-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be6da-108">Permission type</span></span>      | <span data-ttu-id="be6da-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be6da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be6da-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be6da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be6da-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be6da-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="be6da-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be6da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be6da-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be6da-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="be6da-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be6da-114">Application</span></span> | <span data-ttu-id="be6da-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be6da-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="be6da-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be6da-116">HTTP request</span></span>

<span data-ttu-id="be6da-117">ユーザーの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="be6da-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="be6da-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="be6da-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="be6da-119">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="be6da-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="be6da-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="be6da-120">Query parameters</span></span>

<span data-ttu-id="be6da-121">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="be6da-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="be6da-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="be6da-122">Parameter</span></span>    | <span data-ttu-id="be6da-123">型</span><span class="sxs-lookup"><span data-stu-id="be6da-123">Type</span></span>   |<span data-ttu-id="be6da-124">説明</span><span class="sxs-lookup"><span data-stu-id="be6da-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be6da-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="be6da-125">startDateTime</span></span>|<span data-ttu-id="be6da-126">String</span><span class="sxs-lookup"><span data-stu-id="be6da-126">String</span></span>|<span data-ttu-id="be6da-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="be6da-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="be6da-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="be6da-129">endDateTime</span></span>|<span data-ttu-id="be6da-130">String</span><span class="sxs-lookup"><span data-stu-id="be6da-130">String</span></span>|<span data-ttu-id="be6da-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="be6da-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="be6da-133">また、このメソッドは応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="be6da-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be6da-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be6da-134">Request headers</span></span>
| <span data-ttu-id="be6da-135">名前</span><span class="sxs-lookup"><span data-stu-id="be6da-135">Name</span></span>       | <span data-ttu-id="be6da-136">型</span><span class="sxs-lookup"><span data-stu-id="be6da-136">Type</span></span> | <span data-ttu-id="be6da-137">説明</span><span class="sxs-lookup"><span data-stu-id="be6da-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="be6da-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="be6da-138">Authorization</span></span>  | <span data-ttu-id="be6da-139">string</span><span class="sxs-lookup"><span data-stu-id="be6da-139">string</span></span> | <span data-ttu-id="be6da-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be6da-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="be6da-142">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="be6da-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="be6da-143">文字列</span><span class="sxs-lookup"><span data-stu-id="be6da-143">string</span></span> | <span data-ttu-id="be6da-144">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="be6da-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="be6da-145">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="be6da-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="be6da-146">省略可能。</span><span class="sxs-lookup"><span data-stu-id="be6da-146">Optional.</span></span> |
| <span data-ttu-id="be6da-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="be6da-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="be6da-148">文字列</span><span class="sxs-lookup"><span data-stu-id="be6da-148">string</span></span> | <span data-ttu-id="be6da-149">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="be6da-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="be6da-150">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="be6da-150">Values can be "text" or "html".</span></span> <span data-ttu-id="be6da-151">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="be6da-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="be6da-152">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="be6da-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="be6da-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="be6da-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be6da-154">要求本文</span><span class="sxs-lookup"><span data-stu-id="be6da-154">Request body</span></span>
<span data-ttu-id="be6da-155">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="be6da-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be6da-156">応答</span><span class="sxs-lookup"><span data-stu-id="be6da-156">Response</span></span>

<span data-ttu-id="be6da-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="be6da-157">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be6da-158">例</span><span class="sxs-lookup"><span data-stu-id="be6da-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be6da-159">要求</span><span class="sxs-lookup"><span data-stu-id="be6da-159">Request</span></span>
<span data-ttu-id="be6da-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be6da-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="be6da-161">応答</span><span class="sxs-lookup"><span data-stu-id="be6da-161">Response</span></span>
<span data-ttu-id="be6da-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be6da-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
