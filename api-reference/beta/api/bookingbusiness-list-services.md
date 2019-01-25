---
title: サービスの一覧
description: 指定された bookingbusiness では、bookingService オブジェクトのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0571f7c57d2ee37b3095de3e3568cf906c17a987
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511612"
---
# <a name="list-services"></a><span data-ttu-id="ccbb9-103">サービスの一覧</span><span class="sxs-lookup"><span data-stu-id="ccbb9-103">List services</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccbb9-104">指定された[bookingbusiness](../resources/bookingbusiness.md)では、 [bookingService](../resources/bookingservice.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-104">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ccbb9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ccbb9-105">Permissions</span></span>
<span data-ttu-id="ccbb9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccbb9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ccbb9-108">Permission type</span></span>      | <span data-ttu-id="ccbb9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ccbb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccbb9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ccbb9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ccbb9-111">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ccbb9-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ccbb9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ccbb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccbb9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-113">Not supported.</span></span>   |
|<span data-ttu-id="ccbb9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ccbb9-114">Application</span></span> | <span data-ttu-id="ccbb9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ccbb9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ccbb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ccbb9-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ccbb9-117">Optional query parameters</span></span>
<span data-ttu-id="ccbb9-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccbb9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ccbb9-119">Request headers</span></span>
| <span data-ttu-id="ccbb9-120">名前</span><span class="sxs-lookup"><span data-stu-id="ccbb9-120">Name</span></span>      |<span data-ttu-id="ccbb9-121">説明</span><span class="sxs-lookup"><span data-stu-id="ccbb9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ccbb9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccbb9-122">Authorization</span></span>  | <span data-ttu-id="ccbb9-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ccbb9-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccbb9-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="ccbb9-124">Request body</span></span>
<span data-ttu-id="ccbb9-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ccbb9-126">応答</span><span class="sxs-lookup"><span data-stu-id="ccbb9-126">Response</span></span>
<span data-ttu-id="ccbb9-127">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[bookingService](../resources/bookingservice.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-127">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ccbb9-128">例</span><span class="sxs-lookup"><span data-stu-id="ccbb9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccbb9-129">要求</span><span class="sxs-lookup"><span data-stu-id="ccbb9-129">Request</span></span>
<span data-ttu-id="ccbb9-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
##### <a name="response"></a><span data-ttu-id="ccbb9-131">応答</span><span class="sxs-lookup"><span data-stu-id="ccbb9-131">Response</span></span>
<span data-ttu-id="ccbb9-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-132">The following is an example of the response.</span></span> <span data-ttu-id="ccbb9-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ccbb9-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ccbb9-134">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-services.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
