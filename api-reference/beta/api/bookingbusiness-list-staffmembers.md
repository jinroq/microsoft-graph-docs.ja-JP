---
title: リスト staffMembers
description: 指定した bookingbusiness の bookingStaffMember オブジェクトのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 7ac16244f3dbaf175cff8a41a4b5fba75cb12d8b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415548"
---
# <a name="list-staffmembers"></a><span data-ttu-id="f1ee6-103">リスト staffMembers</span><span class="sxs-lookup"><span data-stu-id="f1ee6-103">List staffMembers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1ee6-104">指定した[bookingbusiness](../resources/bookingbusiness.md)の[bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-104">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f1ee6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1ee6-105">Permissions</span></span>
<span data-ttu-id="f1ee6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ee6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1ee6-108">Permission type</span></span>      | <span data-ttu-id="f1ee6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1ee6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1ee6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1ee6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f1ee6-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f1ee6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1ee6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1ee6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-113">Not supported.</span></span>   |
|<span data-ttu-id="f1ee6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1ee6-114">Application</span></span> | <span data-ttu-id="f1ee6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f1ee6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1ee6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1ee6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f1ee6-117">Optional query parameters</span></span>
<span data-ttu-id="f1ee6-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1ee6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1ee6-119">Request headers</span></span>
| <span data-ttu-id="f1ee6-120">名前</span><span class="sxs-lookup"><span data-stu-id="f1ee6-120">Name</span></span>      |<span data-ttu-id="f1ee6-121">説明</span><span class="sxs-lookup"><span data-stu-id="f1ee6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f1ee6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1ee6-122">Authorization</span></span>  | <span data-ttu-id="f1ee6-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f1ee6-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1ee6-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1ee6-124">Request body</span></span>
<span data-ttu-id="f1ee6-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f1ee6-126">応答</span><span class="sxs-lookup"><span data-stu-id="f1ee6-126">Response</span></span>
<span data-ttu-id="f1ee6-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingStaffMember](../resources/bookingstaffmember.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-127">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1ee6-128">例</span><span class="sxs-lookup"><span data-stu-id="f1ee6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1ee6-129">要求</span><span class="sxs-lookup"><span data-stu-id="f1ee6-129">Request</span></span>
<span data-ttu-id="f1ee6-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f1ee6-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f1ee6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1ee6-132">C#</span><span class="sxs-lookup"><span data-stu-id="f1ee6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-staffmembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1ee6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1ee6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-staffmembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1ee6-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="f1ee6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-staffmembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1ee6-135">応答</span><span class="sxs-lookup"><span data-stu-id="f1ee6-135">Response</span></span>
<span data-ttu-id="f1ee6-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-136">The following is an example of the response.</span></span> <span data-ttu-id="f1ee6-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f1ee6-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f1ee6-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers",
    "value":[
        {
            "id":"8ee1c803-a1fa-406d-8259-7ab53233f148",
            "displayName":"Dana Swope",
            "emailAddress":"danas@contoso.com",
            "availabilityIsAffectedByPersonalCalendar":false,
            "colorIndex":1,
            "role":"externalGuest",
            "useBusinessHours":true,
            "workingHours":[
                {
                    "day":"monday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"tuesday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"wednesday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"thursday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"friday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                }
            ]
        },
        {
            "id":"71d64d0e-7225-49b6-b0b1-070d476cda51",
            "displayName":"Samantha Booth",
            "emailAddress":"samanthab@M365B489948.OnMicrosoft.com",
            "availabilityIsAffectedByPersonalCalendar":true,
            "colorIndex":0,
            "role":"administrator",
            "useBusinessHours":true,
            "workingHours":[
                {
                    "day":"monday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"tuesday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"wednesday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"thursday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"friday",
                    "timeSlots":[
                        {
                            "start":"08:00:00.0000000",
                            "end":"17:00:00.0000000"
                        }
                    ]
                },
                {
                    "day":"saturday",
                    "timeSlots":[

                    ]
                },
                {
                    "day":"sunday",
                    "timeSlots":[

                    ]
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
