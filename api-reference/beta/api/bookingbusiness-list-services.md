---
title: サービスを一覧表示する
description: 指定した bookingservice の bookingService オブジェクトのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 270043d330138d08ef8e7d84f3dfa02f8cc1fac4
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636143"
---
# <a name="list-services"></a><span data-ttu-id="f490b-103">サービスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f490b-103">List services</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f490b-104">指定した[bookingservice](../resources/bookingbusiness.md)の[bookingservice](../resources/bookingservice.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f490b-104">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f490b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f490b-105">Permissions</span></span>
<span data-ttu-id="f490b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f490b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f490b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f490b-108">Permission type</span></span>      | <span data-ttu-id="f490b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f490b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f490b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f490b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f490b-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="f490b-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f490b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f490b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f490b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f490b-113">Not supported.</span></span>   |
|<span data-ttu-id="f490b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f490b-114">Application</span></span> | <span data-ttu-id="f490b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f490b-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f490b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f490b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f490b-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f490b-117">Optional query parameters</span></span>
<span data-ttu-id="f490b-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f490b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f490b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f490b-119">Request headers</span></span>
| <span data-ttu-id="f490b-120">名前</span><span class="sxs-lookup"><span data-stu-id="f490b-120">Name</span></span>      |<span data-ttu-id="f490b-121">説明</span><span class="sxs-lookup"><span data-stu-id="f490b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f490b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f490b-122">Authorization</span></span>  | <span data-ttu-id="f490b-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f490b-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f490b-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f490b-124">Request body</span></span>
<span data-ttu-id="f490b-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f490b-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f490b-126">応答</span><span class="sxs-lookup"><span data-stu-id="f490b-126">Response</span></span>
<span data-ttu-id="f490b-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingservice](../resources/bookingservice.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f490b-127">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f490b-128">例</span><span class="sxs-lookup"><span data-stu-id="f490b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f490b-129">要求</span><span class="sxs-lookup"><span data-stu-id="f490b-129">Request</span></span>
<span data-ttu-id="f490b-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f490b-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
##### <a name="response"></a><span data-ttu-id="f490b-131">応答</span><span class="sxs-lookup"><span data-stu-id="f490b-131">Response</span></span>
<span data-ttu-id="f490b-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f490b-132">The following is an example of the response.</span></span> <span data-ttu-id="f490b-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f490b-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f490b-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f490b-134">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f490b-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="f490b-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f490b-136">Visual</span><span class="sxs-lookup"><span data-stu-id="f490b-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_services-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f490b-137">Java</span><span class="sxs-lookup"><span data-stu-id="f490b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_services-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-list-services.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list-services.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
