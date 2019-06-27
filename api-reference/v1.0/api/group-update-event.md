---
title: イベントを更新する
description: event オブジェクトを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c01f52688ffa4944dff4a1f5e77f4ce71ff1cc48
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274992"
---
# <a name="update-event"></a><span data-ttu-id="a941c-103">イベントを更新する</span><span class="sxs-lookup"><span data-stu-id="a941c-103">Update event</span></span>
<span data-ttu-id="a941c-104">[event](../resources/event.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a941c-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a941c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a941c-105">Permissions</span></span>
<span data-ttu-id="a941c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a941c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a941c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a941c-108">Permission type</span></span>      | <span data-ttu-id="a941c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a941c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a941c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a941c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a941c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a941c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a941c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a941c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a941c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a941c-113">Not supported.</span></span>    |
|<span data-ttu-id="a941c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a941c-114">Application</span></span> | <span data-ttu-id="a941c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a941c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a941c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a941c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a941c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a941c-117">Request headers</span></span>
| <span data-ttu-id="a941c-118">名前</span><span class="sxs-lookup"><span data-stu-id="a941c-118">Name</span></span>       | <span data-ttu-id="a941c-119">型</span><span class="sxs-lookup"><span data-stu-id="a941c-119">Type</span></span> | <span data-ttu-id="a941c-120">説明</span><span class="sxs-lookup"><span data-stu-id="a941c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a941c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a941c-121">Authorization</span></span>  | <span data-ttu-id="a941c-122">string</span><span class="sxs-lookup"><span data-stu-id="a941c-122">string</span></span>  | <span data-ttu-id="a941c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a941c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a941c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a941c-125">Request body</span></span>
<span data-ttu-id="a941c-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a941c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a941c-129">応答</span><span class="sxs-lookup"><span data-stu-id="a941c-129">Response</span></span>
<span data-ttu-id="a941c-130">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a941c-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a941c-131">例</span><span class="sxs-lookup"><span data-stu-id="a941c-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a941c-132">要求</span><span class="sxs-lookup"><span data-stu-id="a941c-132">Request</span></span>
<span data-ttu-id="a941c-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a941c-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4", "AAMkADZlAAAAABERAAA="],
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/calendar/events/AAMkADZlAAAAABERAAA=
Content-type: application/json

{ 
  "location":{
      "displayName":"Conf Room 2"
  }
}
```

#### <a name="response"></a><span data-ttu-id="a941c-134">応答</span><span class="sxs-lookup"><span data-stu-id="a941c-134">Response</span></span>
<span data-ttu-id="a941c-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a941c-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.event",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/calendar/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMKyZg==\"",
    "id": "AAMkADZlAAAAABERAAA=",
    "createdDateTime": "2019-04-06T13:19:09.2517612Z",
    "lastModifiedDateTime": "2019-05-20T00:14:51.2677891Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMKyZg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B7CA7D517BECD40100000000000000001000000011E38F935AD4FF41BDAB12A2F3E15103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Planogram Training",
    "bodyPreview": "Need more help with visual merchandising?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZlAAAAABERAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\n<div>Need more help with visual merchandising?\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-04-16T22:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-04-16T23:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Conf Room 2",
        "locationType": "default",
        "uniqueId": "Conf Room 2",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Conf Room 2",
            "locationType": "default",
            "uniqueId": "Conf Room 2",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2019-04-06T13:19:12.1060982Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Retail",
                "address": "Retail@contoso.onmicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
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
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Nestor Wilke",
                "address": "NestorW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Retail",
            "address": "Retail@contoso.onmicrosoft.com"
        }
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a941c-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a941c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a941c-137">C#</span><span class="sxs-lookup"><span data-stu-id="a941c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a941c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="a941c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group_event-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a941c-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="a941c-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_group_event-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
