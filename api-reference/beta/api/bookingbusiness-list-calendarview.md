---
title: 予約予定表ビューを一覧表示します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 96da0d02d58f9ea4a3503e08c0733f4394dbbd6a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956942"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="e9903-104">予約予定表ビューを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e9903-104">List Bookings calendarView</span></span>

 > <span data-ttu-id="e9903-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e9903-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9903-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9903-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e9903-107">[BookingBusiness](../resources/bookingbusiness.md)、指定した日付範囲内に発生するのには、 [bookingAppointment](../resources/bookingappointment.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e9903-107">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9903-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e9903-108">Permissions</span></span>
<span data-ttu-id="e9903-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9903-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9903-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e9903-111">Permission type</span></span>      | <span data-ttu-id="e9903-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e9903-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9903-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e9903-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e9903-114">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e9903-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e9903-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e9903-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9903-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9903-116">Not supported.</span></span>   |
|<span data-ttu-id="e9903-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e9903-117">Application</span></span> | <span data-ttu-id="e9903-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9903-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e9903-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e9903-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="e9903-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9903-120">Request headers</span></span>
| <span data-ttu-id="e9903-121">名前</span><span class="sxs-lookup"><span data-stu-id="e9903-121">Name</span></span>       | <span data-ttu-id="e9903-122">説明</span><span class="sxs-lookup"><span data-stu-id="e9903-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e9903-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9903-123">Authorization</span></span>  | <span data-ttu-id="e9903-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e9903-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9903-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e9903-125">Request body</span></span>
<span data-ttu-id="e9903-126">要求 URL に、次のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="e9903-126">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="e9903-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9903-127">Parameter</span></span>    | <span data-ttu-id="e9903-128">型</span><span class="sxs-lookup"><span data-stu-id="e9903-128">Type</span></span>   |<span data-ttu-id="e9903-129">説明</span><span class="sxs-lookup"><span data-stu-id="e9903-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9903-130">開始</span><span class="sxs-lookup"><span data-stu-id="e9903-130">start</span></span>|<span data-ttu-id="e9903-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9903-131">DateTimeOffset</span></span>|<span data-ttu-id="e9903-132">時間範囲の開始日時は UTC、または UTC からのオフセットとしての ISO 8601 形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="e9903-132">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="e9903-133">など、2018 年 1 月 1 日に UTC 午前 0 時が、これのようになります。: '2018-01-01T00:00:00Z'、PST で同時には次のように、:' 2017-12-31T16:00:00-08:00 ' です。</span><span class="sxs-lookup"><span data-stu-id="e9903-133">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="e9903-134">end</span><span class="sxs-lookup"><span data-stu-id="e9903-134">end</span></span>|<span data-ttu-id="e9903-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9903-135">DateTimeOffset</span></span>|<span data-ttu-id="e9903-136">時間範囲の終了日時は UTC、または UTC からのオフセットとしての ISO 8601 形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="e9903-136">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="e9903-137">例では、3 am UTC、2018 年 1 月 1日には次のように: '2018-01-01T03:00:00Z'、PST で同時には次のように、:' 2017-12-31T19:00:00-08時 00分 ' です。</span><span class="sxs-lookup"><span data-stu-id="e9903-137">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="e9903-138">応答</span><span class="sxs-lookup"><span data-stu-id="e9903-138">Response</span></span>
<span data-ttu-id="e9903-139">かどうかは成功すると、このメソッドを返します`200, OK`、応答の本体で応答コードと[bookingAppointment](../resources/bookingappointment.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e9903-139">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9903-140">例</span><span class="sxs-lookup"><span data-stu-id="e9903-140">Example</span></span>
<span data-ttu-id="e9903-141">次に、この API を呼び出す方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="e9903-141">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e9903-142">要求</span><span class="sxs-lookup"><span data-stu-id="e9903-142">Request</span></span>
<span data-ttu-id="e9903-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9903-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```

##### <a name="response"></a><span data-ttu-id="e9903-144">応答</span><span class="sxs-lookup"><span data-stu-id="e9903-144">Response</span></span>
<span data-ttu-id="e9903-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9903-145">The following is an example of the response.</span></span> <span data-ttu-id="e9903-146">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e9903-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e9903-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e9903-147">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
