---
title: BookingService を取得する
description: 指定した bookingservice の bookingService オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c1fd07f466fcc81cec7394caa96e24781256728d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439036"
---
# <a name="get-bookingservice"></a><span data-ttu-id="d4666-103">BookingService を取得する</span><span class="sxs-lookup"><span data-stu-id="d4666-103">Get bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4666-104">指定した[bookingservice](../resources/bookingbusiness.md)の[bookingservice](../resources/bookingservice.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d4666-104">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d4666-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d4666-105">Permissions</span></span>
<span data-ttu-id="d4666-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4666-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4666-108">Permission type</span></span>      | <span data-ttu-id="d4666-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4666-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4666-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4666-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d4666-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="d4666-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d4666-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4666-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4666-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4666-113">Not supported.</span></span>   |
|<span data-ttu-id="d4666-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4666-114">Application</span></span> | <span data-ttu-id="d4666-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4666-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d4666-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4666-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d4666-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d4666-117">Optional query parameters</span></span>
<span data-ttu-id="d4666-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d4666-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4666-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4666-119">Request headers</span></span>
| <span data-ttu-id="d4666-120">名前</span><span class="sxs-lookup"><span data-stu-id="d4666-120">Name</span></span>      |<span data-ttu-id="d4666-121">説明</span><span class="sxs-lookup"><span data-stu-id="d4666-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4666-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4666-122">Authorization</span></span>  | <span data-ttu-id="d4666-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d4666-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4666-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4666-124">Request body</span></span>
<span data-ttu-id="d4666-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d4666-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d4666-126">応答</span><span class="sxs-lookup"><span data-stu-id="d4666-126">Response</span></span>
<span data-ttu-id="d4666-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingservice](../resources/bookingservice.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4666-127">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d4666-128">例</span><span class="sxs-lookup"><span data-stu-id="d4666-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4666-129">要求</span><span class="sxs-lookup"><span data-stu-id="d4666-129">Request</span></span>
<span data-ttu-id="d4666-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4666-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d4666-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d4666-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4666-132">C#</span><span class="sxs-lookup"><span data-stu-id="d4666-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4666-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4666-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4666-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="d4666-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d4666-135">応答</span><span class="sxs-lookup"><span data-stu-id="d4666-135">Response</span></span>
<span data-ttu-id="d4666-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4666-136">The following is an example of the response.</span></span> <span data-ttu-id="d4666-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d4666-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d4666-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d4666-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT30M",
    "defaultPrice": 10,
    "defaultPriceType": "fixedPrice",
    "description": "Individual bento box lunch delivery",
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
    "defaultReminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "Please be reminded that this service is tomorrow."
        }
    ],
    "schedulingPolicy": {
        "timeSlotInterval": "PT1H",
        "minimumLeadTime": "PT10H",
        "maximumAdvance": "P10D",
        "sendConfirmationsToOwner": true,
        "allowStaffSelection": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
