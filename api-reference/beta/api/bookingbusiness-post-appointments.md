---
title: BookingAppointment の作成
description: 指定した bookingappointment の新しいブックを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 50605b91af3f00d0f6d448c21bea165b1ce60321
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258094"
---
# <a name="create-bookingappointment"></a><span data-ttu-id="ab2aa-103">BookingAppointment の作成</span><span class="sxs-lookup"><span data-stu-id="ab2aa-103">Create bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab2aa-104">指定した[bookingappointment](../resources/bookingbusiness.md)の新しい[ブック](../resources/bookingappointment.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-104">Create a new [bookingAppointment](../resources/bookingappointment.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ab2aa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab2aa-105">Permissions</span></span>
<span data-ttu-id="ab2aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab2aa-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab2aa-108">Permission type</span></span>      | <span data-ttu-id="ab2aa-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab2aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab2aa-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab2aa-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ab2aa-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="ab2aa-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ab2aa-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab2aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab2aa-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-113">Not supported.</span></span>   |
|<span data-ttu-id="ab2aa-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab2aa-114">Application</span></span> | <span data-ttu-id="ab2aa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ab2aa-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab2aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments

```
## <a name="request-headers"></a><span data-ttu-id="ab2aa-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab2aa-117">Request headers</span></span>
| <span data-ttu-id="ab2aa-118">名前</span><span class="sxs-lookup"><span data-stu-id="ab2aa-118">Name</span></span>       | <span data-ttu-id="ab2aa-119">説明</span><span class="sxs-lookup"><span data-stu-id="ab2aa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab2aa-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab2aa-120">Authorization</span></span>  | <span data-ttu-id="ab2aa-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ab2aa-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab2aa-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab2aa-122">Request body</span></span>
<span data-ttu-id="ab2aa-123">要求本文で、 [Bookingappointment](../resources/bookingappointment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-123">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ab2aa-124">応答</span><span class="sxs-lookup"><span data-stu-id="ab2aa-124">Response</span></span>
<span data-ttu-id="ab2aa-125">成功した場合、この`201, Created`メソッドは応答コードと、応答本文で[bookingappointment](../resources/bookingappointment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-125">If successful, this method returns `201, Created` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab2aa-126">例</span><span class="sxs-lookup"><span data-stu-id="ab2aa-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab2aa-127">要求</span><span class="sxs-lookup"><span data-stu-id="ab2aa-127">Request</span></span>
<span data-ttu-id="ab2aa-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-128">The following is an example of the request.</span></span> <span data-ttu-id="ab2aa-129">この予定には、特定のスタッフメンバーの予約は含まれません。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-129">This appointment does not involve booking specific staff members.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingappointment_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "customerEmailAddress":"jordanm@contoso.com",
    "customerLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "customerName":"Jordan Miller",
    "customerNotes":"Please be on time.",
    "customerPhone":"213-555-0199",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceAmount":10.0,
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceId":"1001",
    "invoiceStatus@odata.type":"#microsoft.graph.bookingInvoiceStatus",
    "invoiceStatus":"open",
    "invoiceUrl":"theInvoiceUrl",
    "optOutOfCustomerEmail":false,
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "price":10.0,
    "priceType@odata.type":"#microsoft.graph.bookingPriceType",
    "priceType":"fixedPrice",
    "reminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "reminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"This service is tomorrow",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be available to enjoy your lunch service.",
            "offset":"PT1H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"customer"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please check traffic for next cater.",
            "offset":"PT2H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"staff"
        }
    ],
    "serviceId":"57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer location",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "serviceName":"Catered bento",
    "serviceNotes":"Customer requires punctual service.",
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
<span data-ttu-id="ab2aa-130">要求本文で、 [Bookingappointment](../resources/bookingappointment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-130">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ab2aa-131">応答</span><span class="sxs-lookup"><span data-stu-id="ab2aa-131">Response</span></span>
<span data-ttu-id="ab2aa-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-132">The following is an example of the response.</span></span> <span data-ttu-id="ab2aa-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ab2aa-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ab2aa-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADc7zF4J0AAA8v_KnAAA=",
    "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
    "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
    "customerName": "Jordan Miller",
    "customerEmailAddress": "jordanm@contoso.com",
    "customerPhone": "213-555-0199",
    "customerNotes": null,
    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceName": "Catered bento",
    "duration": "PT30M",
    "preBuffer": "PT5M",
    "postBuffer": "PT10M",
    "priceType": "fixedPrice",
    "price": 10,
    "serviceNotes": "Customer requires punctual service.",
    "optOutOfCustomerEmail": false,
    "staffMemberIds": [],
    "invoiceAmount": 10,
    "invoiceId": "1001",
    "invoiceStatus": "open",
    "invoiceUrl": "theInvoiceUrl",
    "customerLocation": {
        "displayName": "Customer",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "start": {
        "dateTime": "2018-05-01T12:00:00.0000000Z",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    },
    "serviceLocation": {
        "displayName": "Customer location (123 First Avenue, Buffalo, NY 98052, USA)",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "reminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "This service is tomorrow"
        },
        {
            "offset": "PT1H",
            "recipients": "customer",
            "message": "Please be available to enjoy your lunch service."
        },
        {
            "offset": "PT2H",
            "recipients": "staff",
            "message": "Please check traffic for next cater."
        }
    ],
    "invoiceDate": {
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ab2aa-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ab2aa-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ab2aa-136">C#</span><span class="sxs-lookup"><span data-stu-id="ab2aa-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingappointment_from_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab2aa-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ab2aa-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingappointment_from_bookingbusiness-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ab2aa-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="ab2aa-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_bookingappointment_from_bookingbusiness-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-appointments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-post-appointments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-appointments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
