---
title: calendarView を一覧表示する
description: ユーザーの既定の予定表からの時間の範囲で定義されている予定表ビューで出現する、例外、およびイベントの 1 つのインスタンスを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: efef09cd8f0167804fb6b94dc71f7ab0cf30b183
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529720"
---
# <a name="list-calendarview"></a><span data-ttu-id="537b8-103">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="537b8-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="537b8-104">ユーザーの既定の予定表またはユーザーが所有する他の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="537b8-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="537b8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="537b8-105">Permissions</span></span>
<span data-ttu-id="537b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="537b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="537b8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="537b8-108">Permission type</span></span>      | <span data-ttu-id="537b8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="537b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="537b8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="537b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="537b8-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="537b8-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="537b8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="537b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="537b8-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="537b8-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="537b8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="537b8-114">Application</span></span> | <span data-ttu-id="537b8-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="537b8-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="537b8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="537b8-116">HTTP request</span></span>
<span data-ttu-id="537b8-117">ユーザーの既定の[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="537b8-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="537b8-118">既定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="537b8-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="537b8-119">特定の [calendarGroup](../resources/calendargroup.md) のユーザーの[予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="537b8-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="537b8-120">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="537b8-120">Query parameters</span></span>

<span data-ttu-id="537b8-121">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="537b8-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="537b8-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="537b8-122">Parameter</span></span>    | <span data-ttu-id="537b8-123">型</span><span class="sxs-lookup"><span data-stu-id="537b8-123">Type</span></span>   |<span data-ttu-id="537b8-124">説明</span><span class="sxs-lookup"><span data-stu-id="537b8-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="537b8-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="537b8-125">startDateTime</span></span>|<span data-ttu-id="537b8-126">String</span><span class="sxs-lookup"><span data-stu-id="537b8-126">String</span></span>|<span data-ttu-id="537b8-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="537b8-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="537b8-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="537b8-129">endDateTime</span></span>|<span data-ttu-id="537b8-130">String</span><span class="sxs-lookup"><span data-stu-id="537b8-130">String</span></span>|<span data-ttu-id="537b8-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="537b8-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="537b8-133">また、このメソッドは応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)もサポートします。</span><span class="sxs-lookup"><span data-stu-id="537b8-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="537b8-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="537b8-134">Request headers</span></span>
| <span data-ttu-id="537b8-135">名前</span><span class="sxs-lookup"><span data-stu-id="537b8-135">Name</span></span>       | <span data-ttu-id="537b8-136">型</span><span class="sxs-lookup"><span data-stu-id="537b8-136">Type</span></span> | <span data-ttu-id="537b8-137">説明</span><span class="sxs-lookup"><span data-stu-id="537b8-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="537b8-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="537b8-138">Authorization</span></span>  | <span data-ttu-id="537b8-139">string</span><span class="sxs-lookup"><span data-stu-id="537b8-139">string</span></span> | <span data-ttu-id="537b8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="537b8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="537b8-142">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="537b8-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="537b8-143">string</span><span class="sxs-lookup"><span data-stu-id="537b8-143">string</span></span> | <span data-ttu-id="537b8-144">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="537b8-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="537b8-145">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="537b8-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="537b8-146">省略可能。</span><span class="sxs-lookup"><span data-stu-id="537b8-146">Optional.</span></span> |
| <span data-ttu-id="537b8-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="537b8-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="537b8-148">string</span><span class="sxs-lookup"><span data-stu-id="537b8-148">string</span></span> | <span data-ttu-id="537b8-149">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="537b8-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="537b8-150">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="537b8-150">Values can be "text" or "html".</span></span> <span data-ttu-id="537b8-151">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="537b8-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="537b8-152">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="537b8-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="537b8-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="537b8-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="537b8-154">要求本文</span><span class="sxs-lookup"><span data-stu-id="537b8-154">Request body</span></span>
<span data-ttu-id="537b8-155">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="537b8-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="537b8-156">応答</span><span class="sxs-lookup"><span data-stu-id="537b8-156">Response</span></span>

<span data-ttu-id="537b8-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="537b8-157">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="537b8-158">例</span><span class="sxs-lookup"><span data-stu-id="537b8-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="537b8-159">要求</span><span class="sxs-lookup"><span data-stu-id="537b8-159">Request</span></span>
<span data-ttu-id="537b8-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="537b8-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="537b8-161">応答</span><span class="sxs-lookup"><span data-stu-id="537b8-161">Response</span></span>
<span data-ttu-id="537b8-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="537b8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List calendarView",
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-calendarview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
