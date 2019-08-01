---
title: イベントを取得する
description: event オブジェクトを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 61d43f8d1fa87d88c6828d3d20349ca7b66bc99d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014936"
---
# <a name="get-event"></a><span data-ttu-id="8ddcc-103">イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="8ddcc-103">Get event</span></span>
<span data-ttu-id="8ddcc-104">[event](../resources/event.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-104">Get an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ddcc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8ddcc-105">Permissions</span></span>
<span data-ttu-id="8ddcc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ddcc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ddcc-108">Permission type</span></span>      | <span data-ttu-id="8ddcc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ddcc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ddcc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ddcc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ddcc-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ddcc-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ddcc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ddcc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ddcc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-113">Not supported.</span></span>    |
|<span data-ttu-id="8ddcc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ddcc-114">Application</span></span> | <span data-ttu-id="8ddcc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ddcc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ddcc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ddcc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ddcc-117">Optional query parameters</span></span>
<span data-ttu-id="8ddcc-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ddcc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ddcc-119">Request headers</span></span>
| <span data-ttu-id="8ddcc-120">名前</span><span class="sxs-lookup"><span data-stu-id="8ddcc-120">Name</span></span>       | <span data-ttu-id="8ddcc-121">型</span><span class="sxs-lookup"><span data-stu-id="8ddcc-121">Type</span></span> | <span data-ttu-id="8ddcc-122">説明</span><span class="sxs-lookup"><span data-stu-id="8ddcc-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="8ddcc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ddcc-123">Authorization</span></span>  | <span data-ttu-id="8ddcc-124">string</span><span class="sxs-lookup"><span data-stu-id="8ddcc-124">string</span></span> | <span data-ttu-id="8ddcc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ddcc-127">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8ddcc-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="8ddcc-128">string</span><span class="sxs-lookup"><span data-stu-id="8ddcc-128">string</span></span> | <span data-ttu-id="8ddcc-129">これを使用して、応答内の開始および終了時刻のタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="8ddcc-130">指定しない場合、これらの時刻値は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="8ddcc-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-131">Optional.</span></span> |
| <span data-ttu-id="8ddcc-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="8ddcc-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="8ddcc-133">string</span><span class="sxs-lookup"><span data-stu-id="8ddcc-133">string</span></span> | <span data-ttu-id="8ddcc-134">**body** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="8ddcc-135">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-135">Values can be "text" or "html".</span></span> <span data-ttu-id="8ddcc-136">この `Prefer` ヘッダーが指定されている場合、`Preference-Applied` ヘッダーが確認として返されます。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="8ddcc-137">このヘッダーが指定されていない場合は、**body** プロパティが HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="8ddcc-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ddcc-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ddcc-139">Request body</span></span>
<span data-ttu-id="8ddcc-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ddcc-141">応答</span><span class="sxs-lookup"><span data-stu-id="8ddcc-141">Response</span></span>
<span data-ttu-id="8ddcc-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [event](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-142">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ddcc-143">例</span><span class="sxs-lookup"><span data-stu-id="8ddcc-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8ddcc-144">要求</span><span class="sxs-lookup"><span data-stu-id="8ddcc-144">Request</span></span>
<span data-ttu-id="8ddcc-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-145">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ddcc-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8ddcc-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "get_group_event"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ddcc-147">C#</span><span class="sxs-lookup"><span data-stu-id="8ddcc-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ddcc-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ddcc-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ddcc-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="8ddcc-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ddcc-150">Java</span><span class="sxs-lookup"><span data-stu-id="8ddcc-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8ddcc-151">応答</span><span class="sxs-lookup"><span data-stu-id="8ddcc-151">Response</span></span>
<span data-ttu-id="8ddcc-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-152">The following is an example of the response.</span></span>
><span data-ttu-id="8ddcc-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8ddcc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Eastern Standard Time",
            "numberOfOccurrences": 0
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "HR Taskforce",
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
