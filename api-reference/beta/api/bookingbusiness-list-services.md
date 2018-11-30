---
title: サービスの一覧
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 74326f68f86eeb461b18e3533e9c4da262ccd847
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068970"
---
# <a name="list-services"></a><span data-ttu-id="58b55-104">サービスの一覧</span><span class="sxs-lookup"><span data-stu-id="58b55-104">List services</span></span>

 > <span data-ttu-id="58b55-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58b55-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58b55-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58b55-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="58b55-107">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 [bookingService](../resources/bookingservice.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="58b55-107">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="58b55-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58b55-108">Permissions</span></span>
<span data-ttu-id="58b55-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58b55-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58b55-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58b55-111">Permission type</span></span>      | <span data-ttu-id="58b55-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58b55-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58b55-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58b55-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="58b55-114">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="58b55-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="58b55-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58b55-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58b55-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58b55-116">Not supported.</span></span>   |
|<span data-ttu-id="58b55-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58b55-117">Application</span></span> | <span data-ttu-id="58b55-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58b55-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="58b55-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58b55-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58b55-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="58b55-120">Optional query parameters</span></span>
<span data-ttu-id="58b55-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="58b55-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58b55-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58b55-122">Request headers</span></span>
| <span data-ttu-id="58b55-123">名前</span><span class="sxs-lookup"><span data-stu-id="58b55-123">Name</span></span>      |<span data-ttu-id="58b55-124">説明</span><span class="sxs-lookup"><span data-stu-id="58b55-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58b55-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="58b55-125">Authorization</span></span>  | <span data-ttu-id="58b55-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="58b55-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="58b55-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="58b55-127">Request body</span></span>
<span data-ttu-id="58b55-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="58b55-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="58b55-129">応答</span><span class="sxs-lookup"><span data-stu-id="58b55-129">Response</span></span>
<span data-ttu-id="58b55-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[bookingService](../resources/bookingservice.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="58b55-130">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58b55-131">例</span><span class="sxs-lookup"><span data-stu-id="58b55-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58b55-132">要求</span><span class="sxs-lookup"><span data-stu-id="58b55-132">Request</span></span>
<span data-ttu-id="58b55-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58b55-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
##### <a name="response"></a><span data-ttu-id="58b55-134">応答</span><span class="sxs-lookup"><span data-stu-id="58b55-134">Response</span></span>
<span data-ttu-id="58b55-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58b55-135">The following is an example of the response.</span></span> <span data-ttu-id="58b55-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="58b55-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="58b55-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="58b55-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services",
    "value": [
        {
            "id": "f9b9121f-aed7-4c8c-bb3a-a1796a0b0b2d",
            "displayName": "Initial service",
            "defaultDuration": "PT10M",
            "defaultPrice": 0,
            "defaultPriceType": "notSet",
            "description": "Not sure how to choose? Let us introduce you to our traditional family recipes.",
            "isHiddenFromCustomers": false,
            "notes": "This is where you can add notes about this service that only you and your staff see.",
            "preBuffer": "PT0S",
            "postBuffer": "PT0S",
            "staffMemberIds": [],
            "schedulingPolicy": null,
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
            "defaultReminders": []
        },
        {
            "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "displayName": "Catered bento",
            "defaultDuration": "PT30M",
            "defaultPrice": 10,
            "defaultPriceType": "fixedPrice",
            "description": "Catered individual bento box lunch",
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
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        },
        {
            "id": "635a7b7c-4230-4d3b-a42b-698e89927528",
            "displayName": "Kaiseki",
            "defaultDuration": "PT1H30M",
            "defaultPrice": 30,
            "defaultPriceType": "fixedPrice",
            "description": "Individual kaiseki lunch delivery",
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
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->