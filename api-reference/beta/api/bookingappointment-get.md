---
title: BookingAppointment を取得します。
description: 指定された bookingbusiness のプロパティと、bookingAppointment オブジェクトの関係を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e9e9fffa3101656d4e426578185683065b4f5e5a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525270"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="3a8ed-103">BookingAppointment を取得します。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-103">Get bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a8ed-104">指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 [bookingAppointment](../resources/bookingappointment.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-104">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="3a8ed-105">**Start**および**end**プロパティは常に UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-105">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a8ed-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a8ed-106">Permissions</span></span>
<span data-ttu-id="3a8ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a8ed-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a8ed-109">Permission type</span></span>      | <span data-ttu-id="3a8ed-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a8ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a8ed-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a8ed-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="3a8ed-112">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3a8ed-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3a8ed-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a8ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a8ed-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-114">Not supported.</span></span>   |
|<span data-ttu-id="3a8ed-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a8ed-115">Application</span></span> | <span data-ttu-id="3a8ed-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3a8ed-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a8ed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a8ed-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a8ed-118">Optional query parameters</span></span>
<span data-ttu-id="3a8ed-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a8ed-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a8ed-120">Request headers</span></span>
| <span data-ttu-id="3a8ed-121">名前</span><span class="sxs-lookup"><span data-stu-id="3a8ed-121">Name</span></span>      |<span data-ttu-id="3a8ed-122">説明</span><span class="sxs-lookup"><span data-stu-id="3a8ed-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a8ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a8ed-123">Authorization</span></span>  | <span data-ttu-id="3a8ed-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3a8ed-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a8ed-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a8ed-125">Request body</span></span>
<span data-ttu-id="3a8ed-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3a8ed-127">応答</span><span class="sxs-lookup"><span data-stu-id="3a8ed-127">Response</span></span>
<span data-ttu-id="3a8ed-128">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[bookingAppointment](../resources/bookingappointment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-128">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a8ed-129">例</span><span class="sxs-lookup"><span data-stu-id="3a8ed-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a8ed-130">要求</span><span class="sxs-lookup"><span data-stu-id="3a8ed-130">Request</span></span>
<span data-ttu-id="3a8ed-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="3a8ed-132">応答</span><span class="sxs-lookup"><span data-stu-id="3a8ed-132">Response</span></span>
<span data-ttu-id="3a8ed-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-133">The following is an example of the response.</span></span> <span data-ttu-id="3a8ed-134">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3a8ed-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3a8ed-135">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADKnAAA=",
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
        "dateTime": "2018-05-06T12:00:00.0000000Z",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2018-05-06T12:30:00.0000000Z",
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
        "dateTime": "2018-05-06T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
