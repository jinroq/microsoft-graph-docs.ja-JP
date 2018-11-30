---
title: BookingAppointment を取得します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: c3dedab3cbd5fc3848e222317d27527b19671b06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068363"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="7de19-104">BookingAppointment を取得します。</span><span class="sxs-lookup"><span data-stu-id="7de19-104">Get bookingAppointment</span></span>

 > <span data-ttu-id="7de19-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7de19-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7de19-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7de19-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="7de19-107">指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 [bookingAppointment](../resources/bookingappointment.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="7de19-107">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="7de19-108">**Start**および**end**プロパティは常に UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="7de19-108">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="7de19-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7de19-109">Permissions</span></span>
<span data-ttu-id="7de19-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7de19-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7de19-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7de19-112">Permission type</span></span>      | <span data-ttu-id="7de19-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7de19-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7de19-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7de19-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="7de19-115">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="7de19-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7de19-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7de19-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7de19-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7de19-117">Not supported.</span></span>   |
|<span data-ttu-id="7de19-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7de19-118">Application</span></span> | <span data-ttu-id="7de19-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7de19-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="7de19-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7de19-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7de19-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7de19-121">Optional query parameters</span></span>
<span data-ttu-id="7de19-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7de19-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7de19-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7de19-123">Request headers</span></span>
| <span data-ttu-id="7de19-124">名前</span><span class="sxs-lookup"><span data-stu-id="7de19-124">Name</span></span>      |<span data-ttu-id="7de19-125">説明</span><span class="sxs-lookup"><span data-stu-id="7de19-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7de19-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7de19-126">Authorization</span></span>  | <span data-ttu-id="7de19-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7de19-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7de19-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7de19-128">Request body</span></span>
<span data-ttu-id="7de19-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7de19-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7de19-130">応答</span><span class="sxs-lookup"><span data-stu-id="7de19-130">Response</span></span>
<span data-ttu-id="7de19-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[bookingAppointment](../resources/bookingappointment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7de19-131">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7de19-132">例</span><span class="sxs-lookup"><span data-stu-id="7de19-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7de19-133">要求</span><span class="sxs-lookup"><span data-stu-id="7de19-133">Request</span></span>
<span data-ttu-id="7de19-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7de19-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="7de19-135">応答</span><span class="sxs-lookup"><span data-stu-id="7de19-135">Response</span></span>
<span data-ttu-id="7de19-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7de19-136">The following is an example of the response.</span></span> <span data-ttu-id="7de19-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7de19-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7de19-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7de19-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->