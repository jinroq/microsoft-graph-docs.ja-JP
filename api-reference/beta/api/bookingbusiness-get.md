---
title: BookingBusiness の取得
description: BookingBusiness オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: afb5bfc7484635034c67b6e61e12b9e392b4dfb1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865792"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="83e88-103">BookingBusiness の取得</span><span class="sxs-lookup"><span data-stu-id="83e88-103">Get bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83e88-104">[Bookingbusiness](../resources/bookingbusiness.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="83e88-104">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="83e88-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83e88-105">Permissions</span></span>
<span data-ttu-id="83e88-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83e88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83e88-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83e88-108">Permission type</span></span>      | <span data-ttu-id="83e88-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83e88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83e88-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83e88-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="83e88-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="83e88-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="83e88-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83e88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83e88-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83e88-113">Not supported.</span></span>   |
|<span data-ttu-id="83e88-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83e88-114">Application</span></span> | <span data-ttu-id="83e88-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83e88-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="83e88-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83e88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83e88-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83e88-117">Optional query parameters</span></span>
<span data-ttu-id="83e88-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83e88-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83e88-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83e88-119">Request headers</span></span>
| <span data-ttu-id="83e88-120">名前</span><span class="sxs-lookup"><span data-stu-id="83e88-120">Name</span></span>      |<span data-ttu-id="83e88-121">説明</span><span class="sxs-lookup"><span data-stu-id="83e88-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83e88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83e88-122">Authorization</span></span>  | <span data-ttu-id="83e88-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="83e88-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="83e88-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="83e88-124">Request body</span></span>
<span data-ttu-id="83e88-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83e88-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="83e88-126">応答</span><span class="sxs-lookup"><span data-stu-id="83e88-126">Response</span></span>
<span data-ttu-id="83e88-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingbusiness](../resources/bookingbusiness.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83e88-127">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83e88-128">例</span><span class="sxs-lookup"><span data-stu-id="83e88-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83e88-129">要求</span><span class="sxs-lookup"><span data-stu-id="83e88-129">Request</span></span>
<span data-ttu-id="83e88-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="83e88-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="83e88-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="83e88-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83e88-132">C#</span><span class="sxs-lookup"><span data-stu-id="83e88-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83e88-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="83e88-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83e88-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="83e88-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="83e88-135">Java</span><span class="sxs-lookup"><span data-stu-id="83e88-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="83e88-136">応答</span><span class="sxs-lookup"><span data-stu-id="83e88-136">Response</span></span>
<span data-ttu-id="83e88-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="83e88-137">The following is an example of the response.</span></span> <span data-ttu-id="83e88-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="83e88-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="83e88-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="83e88-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"Fabrikam@M365B489948.onmicrosoft.com",
    "displayName":"Fabrikam",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fabrikam.com",
    "webSiteUrl":"https://www.fabrikam.com/",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"home",
        "postOfficeBox":"",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
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
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
