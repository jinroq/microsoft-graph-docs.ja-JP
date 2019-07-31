---
title: BookingAppointment を取得する
description: 指定した bookingappointment の bookingAppointment オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 75efcf0c9afc33d6422e082f01c6b7e77988261d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945250"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="c8b4e-103">BookingAppointment を取得する</span><span class="sxs-lookup"><span data-stu-id="c8b4e-103">Get bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8b4e-104">指定した[bookingappointment](../resources/bookingbusiness.md)の[bookingappointment](../resources/bookingappointment.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-104">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="c8b4e-105">**Start**プロパティと**end**プロパティは、常に UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-105">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8b4e-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8b4e-106">Permissions</span></span>
<span data-ttu-id="c8b4e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8b4e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8b4e-109">Permission type</span></span>      | <span data-ttu-id="c8b4e-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8b4e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8b4e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8b4e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c8b4e-112">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c8b4e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8b4e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8b4e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-114">Not supported.</span></span>   |
|<span data-ttu-id="c8b4e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8b4e-115">Application</span></span> | <span data-ttu-id="c8b4e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c8b4e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8b4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8b4e-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8b4e-118">Optional query parameters</span></span>
<span data-ttu-id="c8b4e-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8b4e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8b4e-120">Request headers</span></span>
| <span data-ttu-id="c8b4e-121">名前</span><span class="sxs-lookup"><span data-stu-id="c8b4e-121">Name</span></span>      |<span data-ttu-id="c8b4e-122">説明</span><span class="sxs-lookup"><span data-stu-id="c8b4e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8b4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8b4e-123">Authorization</span></span>  | <span data-ttu-id="c8b4e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c8b4e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8b4e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8b4e-125">Request body</span></span>
<span data-ttu-id="c8b4e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c8b4e-127">応答</span><span class="sxs-lookup"><span data-stu-id="c8b4e-127">Response</span></span>
<span data-ttu-id="c8b4e-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingappointment](../resources/bookingappointment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-128">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8b4e-129">例</span><span class="sxs-lookup"><span data-stu-id="c8b4e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8b4e-130">要求</span><span class="sxs-lookup"><span data-stu-id="c8b4e-130">Request</span></span>
<span data-ttu-id="c8b4e-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c8b4e-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c8b4e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8b4e-133">C#</span><span class="sxs-lookup"><span data-stu-id="c8b4e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8b4e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8b4e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8b4e-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="c8b4e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c8b4e-136">Java</span><span class="sxs-lookup"><span data-stu-id="c8b4e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c8b4e-137">応答</span><span class="sxs-lookup"><span data-stu-id="c8b4e-137">Response</span></span>
<span data-ttu-id="c8b4e-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-138">The following is an example of the response.</span></span> <span data-ttu-id="c8b4e-139">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c8b4e-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c8b4e-140">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
