---
title: 予定を一覧表示する
description: 指定した bookingappointment の bookingAppointment オブジェクトのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: fceed2834463497291e6c3bc661b237562da76ef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439316"
---
# <a name="list-appointments"></a><span data-ttu-id="c0d36-103">予定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c0d36-103">List appointments</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0d36-104">指定した[bookingappointment](../resources/bookingbusiness.md)の[bookingappointment](../resources/bookingappointment.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c0d36-104">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c0d36-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0d36-105">Permissions</span></span>
<span data-ttu-id="c0d36-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0d36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0d36-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0d36-108">Permission type</span></span>      | <span data-ttu-id="c0d36-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0d36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0d36-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0d36-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0d36-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="c0d36-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c0d36-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0d36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0d36-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0d36-113">Not supported.</span></span>   |
|<span data-ttu-id="c0d36-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0d36-114">Application</span></span> | <span data-ttu-id="c0d36-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0d36-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c0d36-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0d36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0d36-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c0d36-117">Optional query parameters</span></span>
<span data-ttu-id="c0d36-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c0d36-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c0d36-119">ではなく`$filter`、特定の期間における予約ビジネスの一連の予定を取得するには、その日付範囲の[calendarView を取得](bookingbusiness-list-calendarview.md)します。</span><span class="sxs-lookup"><span data-stu-id="c0d36-119">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0d36-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0d36-120">Request headers</span></span>
| <span data-ttu-id="c0d36-121">名前</span><span class="sxs-lookup"><span data-stu-id="c0d36-121">Name</span></span>      |<span data-ttu-id="c0d36-122">説明</span><span class="sxs-lookup"><span data-stu-id="c0d36-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0d36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0d36-123">Authorization</span></span>  | <span data-ttu-id="c0d36-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c0d36-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0d36-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0d36-125">Request body</span></span>
<span data-ttu-id="c0d36-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c0d36-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c0d36-127">応答</span><span class="sxs-lookup"><span data-stu-id="c0d36-127">Response</span></span>
<span data-ttu-id="c0d36-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingappointment](../resources/bookingappointment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c0d36-128">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0d36-129">例</span><span class="sxs-lookup"><span data-stu-id="c0d36-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0d36-130">要求</span><span class="sxs-lookup"><span data-stu-id="c0d36-130">Request</span></span>
<span data-ttu-id="c0d36-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0d36-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0d36-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c0d36-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0d36-133">C#</span><span class="sxs-lookup"><span data-stu-id="c0d36-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appointments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0d36-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0d36-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appointments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0d36-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="c0d36-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appointments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0d36-136">応答</span><span class="sxs-lookup"><span data-stu-id="c0d36-136">Response</span></span>
<span data-ttu-id="c0d36-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0d36-137">The following is an example of the response.</span></span> <span data-ttu-id="c0d36-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c0d36-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c0d36-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c0d36-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments",
    "value": [
        {
            "id": "AAMkADKoAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "customerName": "Bob Kelly",
            "customerEmailAddress": "bobk@tailspintoys.com",
            "customerPhone": "213-555-0108",
            "customerNotes": null,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
            "optOutOfCustomerEmail": false,
            "staffMemberIds": [],
            "invoiceAmount": 10,
            "invoiceId": "1002",
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
                "dateTime": "2018-04-30T13:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-04-30T13:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (987 Third Avenue, Buffalo, NY 98052, USA)",
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-04-30T13:30:00.0000000Z",
                "timeZone": "UTC"
            }
        },
        {
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
            "serviceNotes": null,
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-01T12:30:00.0000000Z",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
