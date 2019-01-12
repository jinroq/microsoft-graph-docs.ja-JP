---
title: BookingService を取得します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6a914a20fd002bd2d3a042239a17366d328878a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928389"
---
# <a name="get-bookingservice"></a><span data-ttu-id="c0442-104">BookingService を取得します。</span><span class="sxs-lookup"><span data-stu-id="c0442-104">Get bookingService</span></span>

 > <span data-ttu-id="c0442-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0442-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0442-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0442-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="c0442-107">指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 [bookingService](../resources/bookingservice.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c0442-107">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c0442-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0442-108">Permissions</span></span>
<span data-ttu-id="c0442-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0442-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0442-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0442-111">Permission type</span></span>      | <span data-ttu-id="c0442-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0442-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0442-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0442-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0442-114">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c0442-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c0442-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0442-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0442-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0442-116">Not supported.</span></span>   |
|<span data-ttu-id="c0442-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0442-117">Application</span></span> | <span data-ttu-id="c0442-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0442-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c0442-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0442-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0442-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c0442-120">Optional query parameters</span></span>
<span data-ttu-id="c0442-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c0442-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0442-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0442-122">Request headers</span></span>
| <span data-ttu-id="c0442-123">名前</span><span class="sxs-lookup"><span data-stu-id="c0442-123">Name</span></span>      |<span data-ttu-id="c0442-124">説明</span><span class="sxs-lookup"><span data-stu-id="c0442-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0442-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0442-125">Authorization</span></span>  | <span data-ttu-id="c0442-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c0442-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0442-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0442-127">Request body</span></span>
<span data-ttu-id="c0442-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c0442-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c0442-129">応答</span><span class="sxs-lookup"><span data-stu-id="c0442-129">Response</span></span>
<span data-ttu-id="c0442-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[bookingService](../resources/bookingservice.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c0442-130">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0442-131">例</span><span class="sxs-lookup"><span data-stu-id="c0442-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0442-132">要求</span><span class="sxs-lookup"><span data-stu-id="c0442-132">Request</span></span>
<span data-ttu-id="c0442-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0442-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="c0442-134">応答</span><span class="sxs-lookup"><span data-stu-id="c0442-134">Response</span></span>
<span data-ttu-id="c0442-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0442-135">The following is an example of the response.</span></span> <span data-ttu-id="c0442-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c0442-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c0442-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c0442-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT30M",
    "defaultPrice": 10,
    "defaultPriceType": "fixedPrice",
    "description": "Individual bento box lunch delivery",
    "isHiddenFromCustomers": false,
    "notes": "Home-cooked special",
    "preBuffer": "PT5M",
    "postBuffer": "PT10M",
    "staffMemberIds": [],
    "defaultLocation": {
        "displayName": "Contoso Lunch Delivery",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "4567 First Street",
            "city": "Buffalo",
            "state": "NY",
            "countryOrRegion": "USA",
            "postalCode": "98052"
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "defaultReminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "Please be reminded that this service is tomorrow."
        }
    ],
    "schedulingPolicy": {
        "timeSlotInterval": "PT1H",
        "minimumLeadTime": "PT10H",
        "maximumAdvance": "P10D",
        "sendConfirmationsToOwner": true,
        "allowStaffSelection": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
