---
title: bookingservice の作成
description: 指定した bookingservice の新しい bookingservice を作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 50501ac1dd79b41b9e970f870964fffaace2f8da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461776"
---
# <a name="create-bookingservice"></a><span data-ttu-id="15a0e-103">bookingservice の作成</span><span class="sxs-lookup"><span data-stu-id="15a0e-103">Create bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15a0e-104">指定した[bookingservice](../resources/bookingbusiness.md)の新しい[bookingservice](../resources/bookingservice.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="15a0e-104">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="15a0e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15a0e-105">Permissions</span></span>
<span data-ttu-id="15a0e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15a0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15a0e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15a0e-108">Permission type</span></span>      | <span data-ttu-id="15a0e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15a0e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15a0e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15a0e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="15a0e-111">予約します。すべての予約</span><span class="sxs-lookup"><span data-stu-id="15a0e-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="15a0e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15a0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15a0e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15a0e-113">Not supported.</span></span>   |
|<span data-ttu-id="15a0e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15a0e-114">Application</span></span> | <span data-ttu-id="15a0e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15a0e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="15a0e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15a0e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="15a0e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15a0e-117">Request headers</span></span>
| <span data-ttu-id="15a0e-118">名前</span><span class="sxs-lookup"><span data-stu-id="15a0e-118">Name</span></span>       | <span data-ttu-id="15a0e-119">説明</span><span class="sxs-lookup"><span data-stu-id="15a0e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="15a0e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="15a0e-120">Authorization</span></span>  | <span data-ttu-id="15a0e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="15a0e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="15a0e-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="15a0e-122">Request body</span></span>
<span data-ttu-id="15a0e-123">要求本文で、 [bookingservice](../resources/bookingservice.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="15a0e-123">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="15a0e-124">応答</span><span class="sxs-lookup"><span data-stu-id="15a0e-124">Response</span></span>
<span data-ttu-id="15a0e-125">成功した場合、この`201, Created`メソッドは応答コードと、応答本文で[bookingservice](../resources/bookingservice.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15a0e-125">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15a0e-126">例</span><span class="sxs-lookup"><span data-stu-id="15a0e-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15a0e-127">要求</span><span class="sxs-lookup"><span data-stu-id="15a0e-127">Request</span></span>
<span data-ttu-id="15a0e-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15a0e-128">The following is an example of the request.</span></span>
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
<span data-ttu-id="15a0e-129">要求本文で、 [bookingservice](../resources/bookingservice.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="15a0e-129">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="15a0e-130">応答</span><span class="sxs-lookup"><span data-stu-id="15a0e-130">Response</span></span>
<span data-ttu-id="15a0e-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15a0e-131">The following is an example of the response.</span></span> <span data-ttu-id="15a0e-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="15a0e-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="15a0e-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="15a0e-133">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-services.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
