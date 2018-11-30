---
title: BookingBusiness を取得します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 809bfad0685f595b4b8076210c6345760b22f3bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068675"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="9eef2-104">BookingBusiness を取得します。</span><span class="sxs-lookup"><span data-stu-id="9eef2-104">Get bookingBusiness</span></span>

 > <span data-ttu-id="9eef2-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9eef2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9eef2-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9eef2-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="9eef2-107">プロパティと、 [bookingBusiness](../resources/bookingbusiness.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="9eef2-107">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9eef2-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9eef2-108">Permissions</span></span>
<span data-ttu-id="9eef2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9eef2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eef2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9eef2-111">Permission type</span></span>      | <span data-ttu-id="9eef2-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9eef2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9eef2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9eef2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="9eef2-114">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="9eef2-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9eef2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9eef2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eef2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9eef2-116">Not supported.</span></span>   |
|<span data-ttu-id="9eef2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9eef2-117">Application</span></span> | <span data-ttu-id="9eef2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9eef2-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="9eef2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9eef2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9eef2-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9eef2-120">Optional query parameters</span></span>
<span data-ttu-id="9eef2-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9eef2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9eef2-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9eef2-122">Request headers</span></span>
| <span data-ttu-id="9eef2-123">名前</span><span class="sxs-lookup"><span data-stu-id="9eef2-123">Name</span></span>      |<span data-ttu-id="9eef2-124">説明</span><span class="sxs-lookup"><span data-stu-id="9eef2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9eef2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9eef2-125">Authorization</span></span>  | <span data-ttu-id="9eef2-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9eef2-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eef2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9eef2-127">Request body</span></span>
<span data-ttu-id="9eef2-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9eef2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9eef2-129">応答</span><span class="sxs-lookup"><span data-stu-id="9eef2-129">Response</span></span>
<span data-ttu-id="9eef2-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[bookingBusiness](../resources/bookingbusiness.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9eef2-130">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9eef2-131">例</span><span class="sxs-lookup"><span data-stu-id="9eef2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9eef2-132">要求</span><span class="sxs-lookup"><span data-stu-id="9eef2-132">Request</span></span>
<span data-ttu-id="9eef2-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9eef2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="9eef2-134">応答</span><span class="sxs-lookup"><span data-stu-id="9eef2-134">Response</span></span>
<span data-ttu-id="9eef2-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9eef2-135">The following is an example of the response.</span></span> <span data-ttu-id="9eef2-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="9eef2-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9eef2-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9eef2-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->