---
title: インスタンスの一覧表示
description: 指定した時間範囲のイベントのインスタンス (発生) を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 73db9643de5fa34d3ff1efff1a22773d859e5055
ms.sourcegitcommit: e6168b868660ad0078d460424d4e6f987d2684a8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2019
ms.locfileid: "31026018"
---
# <a name="list-instances"></a><span data-ttu-id="5d8b3-103">インスタンスの一覧表示</span><span class="sxs-lookup"><span data-stu-id="5d8b3-103">List instances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d8b3-104">指定した時間範囲のイベントのインスタンス (発生) を取得します。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-104">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="5d8b3-105">イベントが `seriesMaster` タイプである場合、これは指定した時間範囲内のイベントの発生と例外を返します。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-105">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d8b3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5d8b3-106">Permissions</span></span>
<span data-ttu-id="5d8b3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d8b3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d8b3-109">Permission type</span></span>      | <span data-ttu-id="5d8b3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d8b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d8b3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d8b3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d8b3-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5d8b3-112">Calendars.Read</span></span>    |
|<span data-ttu-id="5d8b3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d8b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d8b3-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5d8b3-114">Calendars.Read</span></span>    |
|<span data-ttu-id="5d8b3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d8b3-115">Application</span></span> | <span data-ttu-id="5d8b3-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5d8b3-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d8b3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d8b3-117">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="5d8b3-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5d8b3-118">Query parameters</span></span>

<span data-ttu-id="5d8b3-119">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="5d8b3-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5d8b3-120">Parameter</span></span>    | <span data-ttu-id="5d8b3-121">型</span><span class="sxs-lookup"><span data-stu-id="5d8b3-121">Type</span></span>   |<span data-ttu-id="5d8b3-122">説明</span><span class="sxs-lookup"><span data-stu-id="5d8b3-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d8b3-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5d8b3-123">startDateTime</span></span>|<span data-ttu-id="5d8b3-124">String</span><span class="sxs-lookup"><span data-stu-id="5d8b3-124">String</span></span>|<span data-ttu-id="5d8b3-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="5d8b3-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5d8b3-127">endDateTime</span></span>|<span data-ttu-id="5d8b3-128">String</span><span class="sxs-lookup"><span data-stu-id="5d8b3-128">String</span></span>|<span data-ttu-id="5d8b3-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="5d8b3-131">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5d8b3-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d8b3-132">Request headers</span></span>
| <span data-ttu-id="5d8b3-133">名前</span><span class="sxs-lookup"><span data-stu-id="5d8b3-133">Name</span></span>       | <span data-ttu-id="5d8b3-134">型</span><span class="sxs-lookup"><span data-stu-id="5d8b3-134">Type</span></span> | <span data-ttu-id="5d8b3-135">説明</span><span class="sxs-lookup"><span data-stu-id="5d8b3-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="5d8b3-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d8b3-136">Authorization</span></span>  | <span data-ttu-id="5d8b3-137">string</span><span class="sxs-lookup"><span data-stu-id="5d8b3-137">string</span></span> | <span data-ttu-id="5d8b3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5d8b3-140">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5d8b3-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="5d8b3-141">string</span><span class="sxs-lookup"><span data-stu-id="5d8b3-141">string</span></span> | <span data-ttu-id="5d8b3-142">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="5d8b3-143">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="5d8b3-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d8b3-145">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d8b3-145">Request body</span></span>
<span data-ttu-id="5d8b3-146">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d8b3-147">応答</span><span class="sxs-lookup"><span data-stu-id="5d8b3-147">Response</span></span>

<span data-ttu-id="5d8b3-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-148">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d8b3-149">例</span><span class="sxs-lookup"><span data-stu-id="5d8b3-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d8b3-150">要求</span><span class="sxs-lookup"><span data-stu-id="5d8b3-150">Request</span></span>
<span data-ttu-id="5d8b3-151">次の例では、指定された時間範囲内に、定期的なアイテムのマスタイベントであるイベントの発生と例外を取得します。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-151">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
##### <a name="response"></a><span data-ttu-id="5d8b3-152">応答</span><span class="sxs-lookup"><span data-stu-id="5d8b3-152">Response</span></span>
<span data-ttu-id="5d8b3-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5d8b3-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/events('AAMkAGUzYRgWAAA%3D')/instances(subject,bodyPreview,seriesMasterId,type,recurrence,start,end)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-list-instances.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
