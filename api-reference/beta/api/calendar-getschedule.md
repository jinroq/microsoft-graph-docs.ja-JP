---
title: 'カレンダー: getSchedule'
description: コレクションの空き時間情報の可用性の情報をユーザー、配布リスト、または、リソースの指定された時間を取得します。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9089489d2b26b3dd4cd56b950538a72ab533c933
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956956"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="8cb42-103">カレンダー: getSchedule</span><span class="sxs-lookup"><span data-stu-id="8cb42-103">calendar: getSchedule</span></span>

> <span data-ttu-id="8cb42-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cb42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cb42-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb42-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cb42-106">コレクションの空き時間情報の可用性の情報をユーザー、配布リスト、または、リソースの指定された時間を取得します。</span><span class="sxs-lookup"><span data-stu-id="8cb42-106">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cb42-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8cb42-107">Permissions</span></span>
<span data-ttu-id="8cb42-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cb42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb42-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cb42-110">Permission type</span></span>      | <span data-ttu-id="8cb42-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cb42-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cb42-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cb42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8cb42-113">Calendar.Read、Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cb42-113">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="8cb42-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cb42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cb42-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb42-115">Not supported.</span></span> |
|<span data-ttu-id="8cb42-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cb42-116">Application</span></span> | <span data-ttu-id="8cb42-117">Calendar.Read、Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cb42-117">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cb42-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cb42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="8cb42-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cb42-119">Request headers</span></span>
| <span data-ttu-id="8cb42-120">名前</span><span class="sxs-lookup"><span data-stu-id="8cb42-120">Name</span></span>       | <span data-ttu-id="8cb42-121">型</span><span class="sxs-lookup"><span data-stu-id="8cb42-121">Type</span></span> | <span data-ttu-id="8cb42-122">説明</span><span class="sxs-lookup"><span data-stu-id="8cb42-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8cb42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb42-123">Authorization</span></span>  | <span data-ttu-id="8cb42-124">string</span><span class="sxs-lookup"><span data-stu-id="8cb42-124">string</span></span>  | <span data-ttu-id="8cb42-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8cb42-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8cb42-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cb42-127">Content-Type</span></span>  | <span data-ttu-id="8cb42-128">string</span><span class="sxs-lookup"><span data-stu-id="8cb42-128">string</span></span> | <span data-ttu-id="8cb42-129">アプリケーションと json では、エンティティの本文内のデータの性質です。</span><span class="sxs-lookup"><span data-stu-id="8cb42-129">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="8cb42-130">必須。</span><span class="sxs-lookup"><span data-stu-id="8cb42-130">Required.</span></span>  |
| <span data-ttu-id="8cb42-131">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8cb42-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="8cb42-132">文字列</span><span class="sxs-lookup"><span data-stu-id="8cb42-132">string</span></span> | <span data-ttu-id="8cb42-133">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="8cb42-133">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="8cb42-134">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="8cb42-134">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="8cb42-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8cb42-135">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cb42-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cb42-136">Request body</span></span>
<span data-ttu-id="8cb42-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8cb42-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8cb42-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cb42-138">Property</span></span>     | <span data-ttu-id="8cb42-139">型</span><span class="sxs-lookup"><span data-stu-id="8cb42-139">Type</span></span>   |<span data-ttu-id="8cb42-140">説明</span><span class="sxs-lookup"><span data-stu-id="8cb42-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cb42-141">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="8cb42-141">availabilityViewInterval</span></span>|<span data-ttu-id="8cb42-142">String</span><span class="sxs-lookup"><span data-stu-id="8cb42-142">String</span></span>|<span data-ttu-id="8cb42-143">応答では、 **availabilityView**の時間帯の期間を表します。</span><span class="sxs-lookup"><span data-stu-id="8cb42-143">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="8cb42-144">既定値は 30 分、最小値は 6、最大値は 1440 です。</span><span class="sxs-lookup"><span data-stu-id="8cb42-144">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="8cb42-145">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8cb42-145">Optional.</span></span>|
|<span data-ttu-id="8cb42-146">endTime</span><span class="sxs-lookup"><span data-stu-id="8cb42-146">endTime</span></span>|[<span data-ttu-id="8cb42-147">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8cb42-147">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="8cb42-148">日付、時刻、および期間を終了するタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="8cb42-148">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="8cb42-149">スケジュール</span><span class="sxs-lookup"><span data-stu-id="8cb42-149">schedules</span></span>|<span data-ttu-id="8cb42-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8cb42-150">String collection</span></span>|<span data-ttu-id="8cb42-151">可用性情報を取得するには、ユーザー、配布リスト、またはリソースの SMTP アドレスのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8cb42-151">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="8cb42-152">startTime</span><span class="sxs-lookup"><span data-stu-id="8cb42-152">startTime</span></span>|[<span data-ttu-id="8cb42-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8cb42-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="8cb42-154">日付、時刻、および期間を開始するタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="8cb42-154">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="8cb42-155">応答</span><span class="sxs-lookup"><span data-stu-id="8cb42-155">Response</span></span>

<span data-ttu-id="8cb42-156">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードと[scheduleInformation](../resources/scheduleinformation.md)オブジェクト内の各オブジェクトのコレクション、`schedules`パラメーター。</span><span class="sxs-lookup"><span data-stu-id="8cb42-156">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="8cb42-157">例</span><span class="sxs-lookup"><span data-stu-id="8cb42-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cb42-158">要求</span><span class="sxs-lookup"><span data-stu-id="8cb42-158">Request</span></span>
<span data-ttu-id="8cb42-159">次の例では、指定した日付、時刻、タイム ゾーンの 2 つのユーザーの情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="8cb42-159">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["AdeleV@contoso.onmicrosoft.com", "AlexW@contoso.OnMicrosoft.com"],
    "startTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

##### <a name="response"></a><span data-ttu-id="8cb42-160">応答</span><span class="sxs-lookup"><span data-stu-id="8cb42-160">Response</span></span>
<span data-ttu-id="8cb42-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8cb42-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AdeleV@contoso.onmicrosoft.com",
            "availabilityView":"222222000022000000000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Lunch yoga",
                    "location":"Courtyard",
                    "start":{
                        "dateTime":"2018-08-06T11:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T12:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        },
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Q4 planning",
                    "location":"Big Bear",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
