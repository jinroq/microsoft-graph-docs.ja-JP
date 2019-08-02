---
title: 'calendar: getSchedule'
description: 指定した期間について、ユーザー、配布リスト、またはリソースのコレクションの空き時間情報を取得します。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d8e42d2c0ab59153b32ead33fb18453cbb624f98
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944717"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="fa5b8-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="fa5b8-103">calendar: getSchedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa5b8-104">指定された期間のユーザー、配布リスト、またはリソース（部屋または備品）のコレクションの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-104">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa5b8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa5b8-105">Permissions</span></span>
<span data-ttu-id="fa5b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa5b8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa5b8-108">Permission type</span></span>      | <span data-ttu-id="fa5b8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa5b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa5b8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa5b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa5b8-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa5b8-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fa5b8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa5b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa5b8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-113">Not supported.</span></span> |
|<span data-ttu-id="fa5b8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa5b8-114">Application</span></span> | <span data-ttu-id="fa5b8-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa5b8-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa5b8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa5b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="fa5b8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa5b8-117">Request headers</span></span>
| <span data-ttu-id="fa5b8-118">名前</span><span class="sxs-lookup"><span data-stu-id="fa5b8-118">Name</span></span>       | <span data-ttu-id="fa5b8-119">種類</span><span class="sxs-lookup"><span data-stu-id="fa5b8-119">Type</span></span> | <span data-ttu-id="fa5b8-120">説明</span><span class="sxs-lookup"><span data-stu-id="fa5b8-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fa5b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa5b8-121">Authorization</span></span>  | <span data-ttu-id="fa5b8-122">string</span><span class="sxs-lookup"><span data-stu-id="fa5b8-122">string</span></span>  | <span data-ttu-id="fa5b8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa5b8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa5b8-125">Content-Type</span></span>  | <span data-ttu-id="fa5b8-126">string</span><span class="sxs-lookup"><span data-stu-id="fa5b8-126">string</span></span> | <span data-ttu-id="fa5b8-127">エンティティの本体内にあるデータの性質 (application/json)。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="fa5b8-128">必須。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-128">Required.</span></span>  |
| <span data-ttu-id="fa5b8-129">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="fa5b8-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="fa5b8-130">string</span><span class="sxs-lookup"><span data-stu-id="fa5b8-130">string</span></span> | <span data-ttu-id="fa5b8-131">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="fa5b8-132">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="fa5b8-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa5b8-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa5b8-134">Request body</span></span>
<span data-ttu-id="fa5b8-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa5b8-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa5b8-136">Property</span></span>     | <span data-ttu-id="fa5b8-137">型</span><span class="sxs-lookup"><span data-stu-id="fa5b8-137">Type</span></span>   |<span data-ttu-id="fa5b8-138">説明</span><span class="sxs-lookup"><span data-stu-id="fa5b8-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa5b8-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="fa5b8-139">availabilityViewInterval</span></span>|<span data-ttu-id="fa5b8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fa5b8-140">Int32</span></span>|<span data-ttu-id="fa5b8-141">応答内の **availabilityView** の時間帯の期間を表します。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="fa5b8-142">既定値は 30 分。最小値 6、最大値は 1440 です。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="fa5b8-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-143">Optional.</span></span>|
|<span data-ttu-id="fa5b8-144">endTime</span><span class="sxs-lookup"><span data-stu-id="fa5b8-144">endTime</span></span>|[<span data-ttu-id="fa5b8-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fa5b8-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="fa5b8-146">期間が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="fa5b8-147">スケジュール</span><span class="sxs-lookup"><span data-stu-id="fa5b8-147">schedules</span></span>|<span data-ttu-id="fa5b8-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fa5b8-148">String collection</span></span>|<span data-ttu-id="fa5b8-149">空き時間情報を取得する対象のユーザーの SMTP アドレス、配布リスト、またはリソースのコレクション。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="fa5b8-150">startTime</span><span class="sxs-lookup"><span data-stu-id="fa5b8-150">startTime</span></span>|[<span data-ttu-id="fa5b8-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fa5b8-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="fa5b8-152">期間が開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="fa5b8-153">応答</span><span class="sxs-lookup"><span data-stu-id="fa5b8-153">Response</span></span>

<span data-ttu-id="fa5b8-154">成功した場合、このメソッドは `200 OK` 応答コードと、`schedules` パラメーター内の各オブジェクトに対応する [scheduleInformation](../resources/scheduleinformation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="fa5b8-155">例</span><span class="sxs-lookup"><span data-stu-id="fa5b8-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa5b8-156">要求</span><span class="sxs-lookup"><span data-stu-id="fa5b8-156">Request</span></span>
<span data-ttu-id="fa5b8-157">次の例では、指定した日時およびタイム ゾーンについて、2 人のユーザーの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fa5b8-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa5b8-158">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["adelev@contoso.onmicrosoft.com", "meganb@contoso.onmicrosoft.com"],
    "startTime": {
        "dateTime": "2019-03-15T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2019-03-15T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "60"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa5b8-159">C#</span><span class="sxs-lookup"><span data-stu-id="fa5b8-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-getschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa5b8-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa5b8-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-getschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa5b8-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa5b8-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-getschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa5b8-162">Java</span><span class="sxs-lookup"><span data-stu-id="fa5b8-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-getschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fa5b8-163">応答</span><span class="sxs-lookup"><span data-stu-id="fa5b8-163">Response</span></span>
<span data-ttu-id="fa5b8-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa5b8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value": [
        {
            "scheduleId": "adelev@contoso.onmicrosoft.com",
            "availabilityView": "000220000",
            "scheduleItems": [
                {
                    "isPrivate": false,
                    "status": "busy",
                    "subject": "Let's go for lunch",
                    "location": "Harry's Bar",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                }
            ],
            "workingHours": {
                "daysOfWeek": [
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime": "08:00:00.0000000",
                "endTime": "17:00:00.0000000",
                "timeZone": {
                    "name": "Pacific Standard Time"
                }
            }
        },
        {
            "scheduleId": "meganb@contoso.onmicrosoft.com",
            "availabilityView": "200220010",
            "scheduleItems": [
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T08:30:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T09:30:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "tentative",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T13:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T13:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "tentative",
                    "start": {
                        "dateTime": "2019-03-15T16:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T17:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                }
            ],
            "workingHours": {
                "daysOfWeek": [
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime": "08:00:00.0000000",
                "endTime": "17:00:00.0000000",
                "timeZone": {
                    "@odata.type": "#microsoft.graph.customTimeZone",
                    "bias": 480,
                    "name": "Customized Time Zone",
                    "standardOffset": {
                        "time": "02:00:00.0000000",
                        "dayOccurrence": 1,
                        "dayOfWeek": "sunday",
                        "month": 11,
                        "year": 0
                    },
                    "daylightOffset": {
                        "daylightBias": -60,
                        "time": "02:00:00.0000000",
                        "dayOccurrence": 2,
                        "dayOfWeek": "sunday",
                        "month": 3,
                        "year": 0
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
  "suppressions": []
}
-->
