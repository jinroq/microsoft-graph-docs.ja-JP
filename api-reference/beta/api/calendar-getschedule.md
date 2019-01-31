---
title: 'calendar: getSchedule'
description: 指定した期間について、ユーザー、配布リスト、またはリソースのコレクションの空き時間情報を取得します。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0c2f6a54664242831d7fd3f2ddfc6a44984674e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530028"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="03375-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="03375-103">calendar: getSchedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03375-104">指定した期間について、ユーザー、配布リスト、またはリソースのコレクションの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="03375-104">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="03375-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03375-105">Permissions</span></span>
<span data-ttu-id="03375-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03375-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03375-108">Permission type</span></span>      | <span data-ttu-id="03375-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="03375-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03375-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03375-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03375-111">Calendar.Read、Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03375-111">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="03375-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03375-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03375-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03375-113">Not supported.</span></span> |
|<span data-ttu-id="03375-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03375-114">Application</span></span> | <span data-ttu-id="03375-115">Calendar.Read、Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03375-115">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="03375-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03375-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="03375-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03375-117">Request headers</span></span>
| <span data-ttu-id="03375-118">名前</span><span class="sxs-lookup"><span data-stu-id="03375-118">Name</span></span>       | <span data-ttu-id="03375-119">型</span><span class="sxs-lookup"><span data-stu-id="03375-119">Type</span></span> | <span data-ttu-id="03375-120">説明</span><span class="sxs-lookup"><span data-stu-id="03375-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="03375-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03375-121">Authorization</span></span>  | <span data-ttu-id="03375-122">string</span><span class="sxs-lookup"><span data-stu-id="03375-122">string</span></span>  | <span data-ttu-id="03375-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="03375-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03375-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03375-125">Content-Type</span></span>  | <span data-ttu-id="03375-126">string</span><span class="sxs-lookup"><span data-stu-id="03375-126">string</span></span> | <span data-ttu-id="03375-127">エンティティの本体内にあるデータの性質 (application/json)。</span><span class="sxs-lookup"><span data-stu-id="03375-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="03375-128">必須。</span><span class="sxs-lookup"><span data-stu-id="03375-128">Required.</span></span>  |
| <span data-ttu-id="03375-129">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="03375-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="03375-130">string</span><span class="sxs-lookup"><span data-stu-id="03375-130">string</span></span> | <span data-ttu-id="03375-131">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="03375-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="03375-132">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="03375-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="03375-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="03375-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03375-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="03375-134">Request body</span></span>
<span data-ttu-id="03375-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="03375-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03375-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03375-136">Property</span></span>     | <span data-ttu-id="03375-137">型</span><span class="sxs-lookup"><span data-stu-id="03375-137">Type</span></span>   |<span data-ttu-id="03375-138">説明</span><span class="sxs-lookup"><span data-stu-id="03375-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03375-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="03375-139">availabilityViewInterval</span></span>|<span data-ttu-id="03375-140">String</span><span class="sxs-lookup"><span data-stu-id="03375-140">String</span></span>|<span data-ttu-id="03375-141">応答内の **availabilityView** の時間帯の期間を表します。</span><span class="sxs-lookup"><span data-stu-id="03375-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="03375-142">既定値は 30 分。最小値 6、最大値は 1440 です。</span><span class="sxs-lookup"><span data-stu-id="03375-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="03375-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="03375-143">Optional.</span></span>|
|<span data-ttu-id="03375-144">endTime</span><span class="sxs-lookup"><span data-stu-id="03375-144">endTime</span></span>|[<span data-ttu-id="03375-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="03375-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="03375-146">期間が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="03375-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="03375-147">スケジュール</span><span class="sxs-lookup"><span data-stu-id="03375-147">schedules</span></span>|<span data-ttu-id="03375-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="03375-148">String collection</span></span>|<span data-ttu-id="03375-149">空き時間情報を取得する対象のユーザーの SMTP アドレス、配布リスト、またはリソースのコレクション。</span><span class="sxs-lookup"><span data-stu-id="03375-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="03375-150">startTime</span><span class="sxs-lookup"><span data-stu-id="03375-150">startTime</span></span>|[<span data-ttu-id="03375-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="03375-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="03375-152">期間が開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="03375-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="03375-153">応答</span><span class="sxs-lookup"><span data-stu-id="03375-153">Response</span></span>

<span data-ttu-id="03375-154">成功した場合、このメソッドは `200 OK` 応答コードと、`schedules` パラメーター内の各オブジェクトに対応する [scheduleInformation](../resources/scheduleinformation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="03375-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="03375-155">例</span><span class="sxs-lookup"><span data-stu-id="03375-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03375-156">要求</span><span class="sxs-lookup"><span data-stu-id="03375-156">Request</span></span>
<span data-ttu-id="03375-157">次の例では、指定した日時およびタイム ゾーンについて、2 人のユーザーの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="03375-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

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

##### <a name="response"></a><span data-ttu-id="03375-158">応答</span><span class="sxs-lookup"><span data-stu-id="03375-158">Response</span></span>
<span data-ttu-id="03375-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="03375-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-getschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
