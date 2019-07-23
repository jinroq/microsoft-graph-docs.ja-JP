---
title: calendarView を一覧表示する
description: 時間範囲で定義した予定表ビューから、予定、例外、およびイベントの単一インスタンスを取得し、
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5d47c6891fda52a94d2fe1ac7474490419764683
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820613"
---
# <a name="list-calendarview"></a><span data-ttu-id="d2df7-103">calendarView を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d2df7-103">List calendarView</span></span>
<span data-ttu-id="d2df7-104">グループの既定の予定表から、時間範囲で定義した予定表ビューのイベントの発生、例外、および単一インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d2df7-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2df7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2df7-105">Permissions</span></span>
<span data-ttu-id="d2df7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2df7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2df7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2df7-108">Permission type</span></span>      | <span data-ttu-id="d2df7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2df7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2df7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2df7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2df7-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2df7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2df7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2df7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2df7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2df7-113">Not supported.</span></span>    |
|<span data-ttu-id="d2df7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2df7-114">Application</span></span> | <span data-ttu-id="d2df7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2df7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2df7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2df7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="d2df7-117">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2df7-117">Query parameters</span></span>
<span data-ttu-id="d2df7-118">要求 URL に、次の必須のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="d2df7-118">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d2df7-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2df7-119">Parameter</span></span>    | <span data-ttu-id="d2df7-120">型</span><span class="sxs-lookup"><span data-stu-id="d2df7-120">Type</span></span>   |<span data-ttu-id="d2df7-121">説明</span><span class="sxs-lookup"><span data-stu-id="d2df7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2df7-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d2df7-122">startDateTime</span></span>|<span data-ttu-id="d2df7-123">String</span><span class="sxs-lookup"><span data-stu-id="d2df7-123">String</span></span>|<span data-ttu-id="d2df7-p102">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="d2df7-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d2df7-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d2df7-126">endDateTime</span></span>|<span data-ttu-id="d2df7-127">String</span><span class="sxs-lookup"><span data-stu-id="d2df7-127">String</span></span>|<span data-ttu-id="d2df7-p103">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="d2df7-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d2df7-130">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)の一部もサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d2df7-130">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="d2df7-131">[イベント](../resources/event.md)の**lastModifiedDateTime**プロパティは、をサポート\*\*\*\* `$select`していません。</span><span class="sxs-lookup"><span data-stu-id="d2df7-131">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="d2df7-132">値を取得するには、 **calendarView**を適用`$select`せずに単にクエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="d2df7-132">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2df7-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2df7-133">Request headers</span></span>
| <span data-ttu-id="d2df7-134">名前</span><span class="sxs-lookup"><span data-stu-id="d2df7-134">Name</span></span>       | <span data-ttu-id="d2df7-135">型</span><span class="sxs-lookup"><span data-stu-id="d2df7-135">Type</span></span> | <span data-ttu-id="d2df7-136">説明</span><span class="sxs-lookup"><span data-stu-id="d2df7-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d2df7-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2df7-137">Authorization</span></span>  | <span data-ttu-id="d2df7-138">string</span><span class="sxs-lookup"><span data-stu-id="d2df7-138">string</span></span> | <span data-ttu-id="d2df7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2df7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2df7-141">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d2df7-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d2df7-142">string</span><span class="sxs-lookup"><span data-stu-id="d2df7-142">string</span></span> | <span data-ttu-id="d2df7-143">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="d2df7-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d2df7-144">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="d2df7-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d2df7-145">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d2df7-145">Optional.</span></span> |
| <span data-ttu-id="d2df7-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="d2df7-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="d2df7-147">string</span><span class="sxs-lookup"><span data-stu-id="d2df7-147">string</span></span> | <span data-ttu-id="d2df7-148">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="d2df7-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="d2df7-149">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="d2df7-149">Values can be "text" or "html".</span></span> <span data-ttu-id="d2df7-150">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="d2df7-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="d2df7-151">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="d2df7-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="d2df7-152">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d2df7-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2df7-153">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2df7-153">Request body</span></span>
<span data-ttu-id="d2df7-154">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2df7-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2df7-155">応答</span><span class="sxs-lookup"><span data-stu-id="d2df7-155">Response</span></span>
<span data-ttu-id="d2df7-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d2df7-156">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2df7-157">例</span><span class="sxs-lookup"><span data-stu-id="d2df7-157">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d2df7-158">要求</span><span class="sxs-lookup"><span data-stu-id="d2df7-158">Request</span></span>
<span data-ttu-id="d2df7-159">次の例では、イベントの本文をテキスト形式で返すよう要求します。</span><span class="sxs-lookup"><span data-stu-id="d2df7-159">The following example requests event bodies to be returned in text format.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2df7-160">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d2df7-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2df7-161">C#</span><span class="sxs-lookup"><span data-stu-id="d2df7-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2df7-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2df7-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2df7-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="d2df7-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d2df7-164">応答</span><span class="sxs-lookup"><span data-stu-id="d2df7-164">Response</span></span>
<span data-ttu-id="d2df7-165">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d2df7-165">The following is an example of the response.</span></span>
><span data-ttu-id="d2df7-166">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d2df7-166">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d2df7-167">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d2df7-167">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1354
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
    "value":[
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-14T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-14T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                 {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
             ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Follow-up meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-16T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-16T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
