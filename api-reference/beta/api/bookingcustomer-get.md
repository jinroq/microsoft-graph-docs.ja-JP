---
title: BookingCustomer を取得する
description: BookingCustomer オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 865e4019097b7487446c938e3b3cbe72cb80c3a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439057"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="fd877-103">BookingCustomer を取得する</span><span class="sxs-lookup"><span data-stu-id="fd877-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd877-104">[Bookingcustomer](../resources/bookingcustomer.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="fd877-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd877-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd877-105">Permissions</span></span>
<span data-ttu-id="fd877-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd877-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd877-108">Permission type</span></span>      | <span data-ttu-id="fd877-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd877-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd877-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd877-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fd877-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="fd877-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fd877-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd877-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd877-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd877-113">Not supported.</span></span>   |
|<span data-ttu-id="fd877-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd877-114">Application</span></span> | <span data-ttu-id="fd877-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd877-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fd877-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd877-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd877-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fd877-117">Optional query parameters</span></span>
<span data-ttu-id="fd877-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fd877-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd877-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd877-119">Request headers</span></span>
| <span data-ttu-id="fd877-120">名前</span><span class="sxs-lookup"><span data-stu-id="fd877-120">Name</span></span>      |<span data-ttu-id="fd877-121">説明</span><span class="sxs-lookup"><span data-stu-id="fd877-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd877-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd877-122">Authorization</span></span>  | <span data-ttu-id="fd877-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fd877-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd877-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd877-124">Request body</span></span>
<span data-ttu-id="fd877-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fd877-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fd877-126">応答</span><span class="sxs-lookup"><span data-stu-id="fd877-126">Response</span></span>
<span data-ttu-id="fd877-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcustomer](../resources/bookingcustomer.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fd877-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd877-128">例</span><span class="sxs-lookup"><span data-stu-id="fd877-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd877-129">要求</span><span class="sxs-lookup"><span data-stu-id="fd877-129">Request</span></span>
<span data-ttu-id="fd877-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd877-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fd877-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fd877-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fd877-132">C#</span><span class="sxs-lookup"><span data-stu-id="fd877-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd877-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="fd877-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fd877-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="fd877-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fd877-135">応答</span><span class="sxs-lookup"><span data-stu-id="fd877-135">Response</span></span>
<span data-ttu-id="fd877-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd877-136">The following is an example of the response.</span></span> <span data-ttu-id="fd877-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="fd877-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fd877-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fd877-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele Vance",
    "emailAddress": "adelev@proseware.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
