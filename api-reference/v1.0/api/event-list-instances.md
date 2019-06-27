---
title: インスタンスの一覧表示
description: 指定した時間範囲のイベントのインスタンス (発生) を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e87a70ed46ede2ba6dc6f3106eccab17c89736a3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263603"
---
# <a name="list-instances"></a><span data-ttu-id="7f419-103">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="7f419-103">List instances</span></span>

<span data-ttu-id="7f419-104">指定した時間範囲のイベントのインスタンス (発生) を取得します。</span><span class="sxs-lookup"><span data-stu-id="7f419-104">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="7f419-105">イベントが `seriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="7f419-105">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f419-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f419-106">Permissions</span></span>
<span data-ttu-id="7f419-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f419-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f419-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f419-109">Permission type</span></span>      | <span data-ttu-id="7f419-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f419-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f419-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f419-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f419-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f419-112">Calendars.Read</span></span>    |
|<span data-ttu-id="7f419-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f419-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f419-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f419-114">Calendars.Read</span></span>    |
|<span data-ttu-id="7f419-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f419-115">Application</span></span> | <span data-ttu-id="7f419-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f419-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f419-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f419-117">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="7f419-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f419-118">Query parameters</span></span>

<span data-ttu-id="7f419-119">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="7f419-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="7f419-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f419-120">Parameter</span></span>    | <span data-ttu-id="7f419-121">型</span><span class="sxs-lookup"><span data-stu-id="7f419-121">Type</span></span>   |<span data-ttu-id="7f419-122">説明</span><span class="sxs-lookup"><span data-stu-id="7f419-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f419-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7f419-123">startDateTime</span></span>|<span data-ttu-id="7f419-124">String</span><span class="sxs-lookup"><span data-stu-id="7f419-124">String</span></span>|<span data-ttu-id="7f419-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="7f419-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="7f419-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7f419-127">endDateTime</span></span>|<span data-ttu-id="7f419-128">String</span><span class="sxs-lookup"><span data-stu-id="7f419-128">String</span></span>|<span data-ttu-id="7f419-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="7f419-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="7f419-131">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7f419-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f419-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f419-132">Request headers</span></span>
| <span data-ttu-id="7f419-133">名前</span><span class="sxs-lookup"><span data-stu-id="7f419-133">Name</span></span>       | <span data-ttu-id="7f419-134">型</span><span class="sxs-lookup"><span data-stu-id="7f419-134">Type</span></span> | <span data-ttu-id="7f419-135">説明</span><span class="sxs-lookup"><span data-stu-id="7f419-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="7f419-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f419-136">Authorization</span></span>  | <span data-ttu-id="7f419-137">string</span><span class="sxs-lookup"><span data-stu-id="7f419-137">string</span></span> | <span data-ttu-id="7f419-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f419-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7f419-140">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7f419-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="7f419-141">string</span><span class="sxs-lookup"><span data-stu-id="7f419-141">string</span></span> | <span data-ttu-id="7f419-142">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f419-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="7f419-143">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="7f419-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="7f419-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7f419-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f419-145">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f419-145">Request body</span></span>
<span data-ttu-id="7f419-146">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f419-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f419-147">応答</span><span class="sxs-lookup"><span data-stu-id="7f419-147">Response</span></span>

<span data-ttu-id="7f419-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7f419-148">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f419-149">例</span><span class="sxs-lookup"><span data-stu-id="7f419-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f419-150">要求</span><span class="sxs-lookup"><span data-stu-id="7f419-150">Request</span></span>
<span data-ttu-id="7f419-151">次の例では、指定された時間範囲内に、定期的なアイテムのマスタイベントであるイベントの発生と例外を取得します。</span><span class="sxs-lookup"><span data-stu-id="7f419-151">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
##### <a name="response"></a><span data-ttu-id="7f419-152">応答</span><span class="sxs-lookup"><span data-stu-id="7f419-152">Response</span></span>
<span data-ttu-id="7f419-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7f419-153">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "get_instances",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/events('AAMkAGUzYRgWAAA%3D')/instances(subject,bodyPreview,seriesMasterId,type,recurrence,start,end)",
    "value": [
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sE1TatAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "Changing meeting from 4/15 to 4/16.",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "exception",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-16T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-16T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1ru1JMcAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-08T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-08T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sa1do_AAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-22T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-22T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sw1n3PAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-29T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-29T21:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7f419-154">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7f419-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7f419-155">C#</span><span class="sxs-lookup"><span data-stu-id="7f419-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_instances-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f419-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f419-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_instances-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7f419-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="7f419-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_instances-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-list-instances.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/event-list-instances.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-list-instances.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
