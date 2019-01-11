---
title: インスタンスの一覧表示
description: 指定の時間範囲のイベントのインスタンス (文字列) を取得します。 イベントの場合、`SeriesMaster`を入力、これが返されます、
localization_priority: Normal
ms.openlocfilehash: 79f6f5832a30f37a4f66e07eb44c2d31a39f7546
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843443"
---
# <a name="list-instances"></a><span data-ttu-id="7ff3d-104">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="7ff3d-104">List instances</span></span>

> <span data-ttu-id="7ff3d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ff3d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ff3d-p103">指定した時間範囲のイベントのインスタンス (発生) を取得します。イベントが`SeriesMaster`タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-p103">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ff3d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7ff3d-109">Permissions</span></span>
<span data-ttu-id="7ff3d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff3d-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ff3d-112">Permission type</span></span>      | <span data-ttu-id="7ff3d-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ff3d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ff3d-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ff3d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7ff3d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7ff3d-115">Calendars.Read</span></span>    |
|<span data-ttu-id="7ff3d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ff3d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ff3d-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7ff3d-117">Calendars.Read</span></span>    |
|<span data-ttu-id="7ff3d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ff3d-118">Application</span></span> | <span data-ttu-id="7ff3d-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7ff3d-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ff3d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ff3d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="7ff3d-121">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff3d-121">Query parameters</span></span>

<span data-ttu-id="7ff3d-122">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="7ff3d-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff3d-123">Parameter</span></span>    | <span data-ttu-id="7ff3d-124">Type</span><span class="sxs-lookup"><span data-stu-id="7ff3d-124">Type</span></span>   |<span data-ttu-id="7ff3d-125">説明</span><span class="sxs-lookup"><span data-stu-id="7ff3d-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ff3d-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7ff3d-126">startDateTime</span></span>|<span data-ttu-id="7ff3d-127">String</span><span class="sxs-lookup"><span data-stu-id="7ff3d-127">String</span></span>|<span data-ttu-id="7ff3d-p105">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-p105">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="7ff3d-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7ff3d-130">endDateTime</span></span>|<span data-ttu-id="7ff3d-131">String</span><span class="sxs-lookup"><span data-stu-id="7ff3d-131">String</span></span>|<span data-ttu-id="7ff3d-p106">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-p106">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="7ff3d-134">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7ff3d-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ff3d-135">Request headers</span></span>
| <span data-ttu-id="7ff3d-136">名前</span><span class="sxs-lookup"><span data-stu-id="7ff3d-136">Name</span></span>       | <span data-ttu-id="7ff3d-137">種類</span><span class="sxs-lookup"><span data-stu-id="7ff3d-137">Type</span></span> | <span data-ttu-id="7ff3d-138">説明</span><span class="sxs-lookup"><span data-stu-id="7ff3d-138">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="7ff3d-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ff3d-139">Authorization</span></span>  | <span data-ttu-id="7ff3d-140">string</span><span class="sxs-lookup"><span data-stu-id="7ff3d-140">string</span></span> | <span data-ttu-id="7ff3d-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ff3d-143">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7ff3d-143">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="7ff3d-144">文字列</span><span class="sxs-lookup"><span data-stu-id="7ff3d-144">string</span></span> | <span data-ttu-id="7ff3d-145">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-145">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="7ff3d-146">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-146">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="7ff3d-147">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-147">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ff3d-148">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ff3d-148">Request body</span></span>
<span data-ttu-id="7ff3d-149">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ff3d-150">応答</span><span class="sxs-lookup"><span data-stu-id="7ff3d-150">Response</span></span>

<span data-ttu-id="7ff3d-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-151">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ff3d-152">例</span><span class="sxs-lookup"><span data-stu-id="7ff3d-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ff3d-153">要求</span><span class="sxs-lookup"><span data-stu-id="7ff3d-153">Request</span></span>
<span data-ttu-id="7ff3d-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="7ff3d-155">応答</span><span class="sxs-lookup"><span data-stu-id="7ff3d-155">Response</span></span>
<span data-ttu-id="7ff3d-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7ff3d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
