---
title: List Bookings calendarView
description: 指定された日付範囲内に発生する、Bookingappointment の bookingAppointment オブジェクトのコレクションを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 991a47d72505ddca791b4fb7bd2c39c9a2f1482a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318370"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="d6eb3-103">List Bookings calendarView</span><span class="sxs-lookup"><span data-stu-id="d6eb3-103">List Bookings calendarView</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6eb3-104">指定された日付範囲内に発生する、 [Bookingappointment](../resources/bookingbusiness.md)の[bookingappointment](../resources/bookingappointment.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-104">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6eb3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6eb3-105">Permissions</span></span>
<span data-ttu-id="d6eb3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6eb3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6eb3-108">Permission type</span></span>      | <span data-ttu-id="d6eb3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6eb3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6eb3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6eb3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d6eb3-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d6eb3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6eb3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6eb3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-113">Not supported.</span></span>   |
|<span data-ttu-id="d6eb3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6eb3-114">Application</span></span> | <span data-ttu-id="d6eb3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d6eb3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6eb3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="d6eb3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6eb3-117">Request headers</span></span>
| <span data-ttu-id="d6eb3-118">名前</span><span class="sxs-lookup"><span data-stu-id="d6eb3-118">Name</span></span>       | <span data-ttu-id="d6eb3-119">説明</span><span class="sxs-lookup"><span data-stu-id="d6eb3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d6eb3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6eb3-120">Authorization</span></span>  | <span data-ttu-id="d6eb3-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d6eb3-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6eb3-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6eb3-122">Request body</span></span>
<span data-ttu-id="d6eb3-123">要求 URL に、次のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-123">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="d6eb3-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d6eb3-124">Parameter</span></span>    | <span data-ttu-id="d6eb3-125">型</span><span class="sxs-lookup"><span data-stu-id="d6eb3-125">Type</span></span>   |<span data-ttu-id="d6eb3-126">説明</span><span class="sxs-lookup"><span data-stu-id="d6eb3-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6eb3-127">開始</span><span class="sxs-lookup"><span data-stu-id="d6eb3-127">start</span></span>|<span data-ttu-id="d6eb3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6eb3-128">DateTimeOffset</span></span>|<span data-ttu-id="d6eb3-129">ISO 8601 形式で表される時間範囲の開始日時を UTC または UTC からのオフセットで指定します。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-129">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="d6eb3-130">たとえば、2018年1月1日午前0時 (UTC) は次のようになります。 ' 2018-01-01T00:00: 00Z '、PST の同じ時刻は次のようになります。 ' 2017-12-31T16:00:00-08:00 '。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-130">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="d6eb3-131">end</span><span class="sxs-lookup"><span data-stu-id="d6eb3-131">end</span></span>|<span data-ttu-id="d6eb3-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6eb3-132">DateTimeOffset</span></span>|<span data-ttu-id="d6eb3-133">ISO 8601 形式で表される時間範囲の終了日時 (UTC または UTC からのオフセット)。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-133">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="d6eb3-134">たとえば、3月1日の午前0時 (UTC) では、2018は次のようになります。 ' 2018-01-01T03:00: 00Z '、PST の同じ時刻は ' 2017-12-31T19:00:00-08:00 ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-134">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="d6eb3-135">応答</span><span class="sxs-lookup"><span data-stu-id="d6eb3-135">Response</span></span>
<span data-ttu-id="d6eb3-136">成功した場合、この`200, OK`メソッドは応答コードと、応答本文で[bookingappointment](../resources/bookingappointment.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-136">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6eb3-137">例</span><span class="sxs-lookup"><span data-stu-id="d6eb3-137">Example</span></span>
<span data-ttu-id="d6eb3-138">この API を呼び出す方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d6eb3-139">要求</span><span class="sxs-lookup"><span data-stu-id="d6eb3-139">Request</span></span>
<span data-ttu-id="d6eb3-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6eb3-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d6eb3-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6eb3-142">C#</span><span class="sxs-lookup"><span data-stu-id="d6eb3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6eb3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6eb3-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6eb3-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="d6eb3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d6eb3-145">Java</span><span class="sxs-lookup"><span data-stu-id="d6eb3-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-getcalendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d6eb3-146">応答</span><span class="sxs-lookup"><span data-stu-id="d6eb3-146">Response</span></span>
<span data-ttu-id="d6eb3-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-147">The following is an example of the response.</span></span> <span data-ttu-id="d6eb3-148">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-148">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d6eb3-149">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d6eb3-149">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/calendarView",
    "value": [
        {
            "id": "AAMkADKpAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "customerName": "Adele Vance",
            "customerEmailAddress": "adelev@proseware.com",
            "customerPhone": "213-555-0156",
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
            "invoiceId": "1003",
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
                "dateTime": "2018-05-05T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-05T12:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (876 Tenth Avenue, Buffalo, NY 98052, USA)",
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
                "dateTime": "2018-05-05T12:30:00.0000000Z",
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-06T12:30:00.0000000Z",
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
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
