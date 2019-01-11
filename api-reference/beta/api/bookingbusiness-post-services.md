---
title: BookingService を作成します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 73e38c0abfeacb43d3ac7f4e28345ac56becb667
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814295"
---
# <a name="create-bookingservice"></a><span data-ttu-id="37d68-104">BookingService を作成します。</span><span class="sxs-lookup"><span data-stu-id="37d68-104">Create bookingService</span></span>

 > <span data-ttu-id="37d68-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="37d68-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37d68-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37d68-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="37d68-107">指定した[bookingbusiness](../resources/bookingbusiness.md)用の新しい[bookingService](../resources/bookingservice.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="37d68-107">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="37d68-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37d68-108">Permissions</span></span>
<span data-ttu-id="37d68-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37d68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37d68-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37d68-111">Permission type</span></span>      | <span data-ttu-id="37d68-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37d68-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37d68-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37d68-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="37d68-114">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="37d68-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="37d68-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37d68-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37d68-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37d68-116">Not supported.</span></span>   |
|<span data-ttu-id="37d68-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37d68-117">Application</span></span> | <span data-ttu-id="37d68-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37d68-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="37d68-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37d68-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="37d68-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37d68-120">Request headers</span></span>
| <span data-ttu-id="37d68-121">名前</span><span class="sxs-lookup"><span data-stu-id="37d68-121">Name</span></span>       | <span data-ttu-id="37d68-122">説明</span><span class="sxs-lookup"><span data-stu-id="37d68-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="37d68-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37d68-123">Authorization</span></span>  | <span data-ttu-id="37d68-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="37d68-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="37d68-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="37d68-125">Request body</span></span>
<span data-ttu-id="37d68-126">要求の本文には、 [bookingService](../resources/bookingservice.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="37d68-126">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="37d68-127">応答</span><span class="sxs-lookup"><span data-stu-id="37d68-127">Response</span></span>
<span data-ttu-id="37d68-128">かどうかは成功すると、このメソッドを返します`201, Created`、応答の本体で応答コードと[bookingService](../resources/bookingservice.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="37d68-128">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37d68-129">例</span><span class="sxs-lookup"><span data-stu-id="37d68-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37d68-130">要求</span><span class="sxs-lookup"><span data-stu-id="37d68-130">Request</span></span>
<span data-ttu-id="37d68-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="37d68-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingservice_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT1H30M",
    "defaultLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"4567 First Street",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Contoso Lunch Delivery",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "defaultPrice":10.0,
    "defaultPriceType@odata.type":"#microsoft.graph.bookingPriceType",
    "defaultPriceType":"fixedPrice",
    "defaultReminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "defaultReminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be reminded that this service is tomorrow.",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        }
    ],
    "description":"Individual bento box lunch delivery",
    "displayName":"Bento",
    "isHiddenFromCustomers":false,
    "notes":"Home-cooked special",
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "schedulingPolicy":{
        "@odata.type":"#microsoft.graph.bookingSchedulingPolicy",
        "allowStaffSelection":true,
        "maximumAdvance":"P10D",
        "minimumLeadTime":"PT10H",
        "sendConfirmationsToOwner":true,
        "timeSlotInterval":"PT1H"
    },
    "staffMemberIds@odata.type":"#Collection(String)",
    "staffMemberIds":[
        "d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
        "2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
    ]
}
```
<span data-ttu-id="37d68-132">要求の本文には、 [bookingService](../resources/bookingservice.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="37d68-132">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="37d68-133">応答</span><span class="sxs-lookup"><span data-stu-id="37d68-133">Response</span></span>
<span data-ttu-id="37d68-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="37d68-134">The following is an example of the response.</span></span> <span data-ttu-id="37d68-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="37d68-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="37d68-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="37d68-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT1H30M",
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
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
