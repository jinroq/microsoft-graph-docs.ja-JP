---
title: BookingCustomer を取得する
description: BookingCustomer オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6501603add6a4df4a3e031e37e1ca1a96fb20a14
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865373"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="28eea-103">BookingCustomer を取得する</span><span class="sxs-lookup"><span data-stu-id="28eea-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28eea-104">[Bookingcustomer](../resources/bookingcustomer.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="28eea-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="28eea-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="28eea-105">Permissions</span></span>
<span data-ttu-id="28eea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28eea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28eea-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28eea-108">Permission type</span></span>      | <span data-ttu-id="28eea-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="28eea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28eea-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28eea-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="28eea-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="28eea-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="28eea-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28eea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28eea-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28eea-113">Not supported.</span></span>   |
|<span data-ttu-id="28eea-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28eea-114">Application</span></span> | <span data-ttu-id="28eea-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28eea-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="28eea-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28eea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28eea-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="28eea-117">Optional query parameters</span></span>
<span data-ttu-id="28eea-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="28eea-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28eea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28eea-119">Request headers</span></span>
| <span data-ttu-id="28eea-120">名前</span><span class="sxs-lookup"><span data-stu-id="28eea-120">Name</span></span>      |<span data-ttu-id="28eea-121">説明</span><span class="sxs-lookup"><span data-stu-id="28eea-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28eea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28eea-122">Authorization</span></span>  | <span data-ttu-id="28eea-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="28eea-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="28eea-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="28eea-124">Request body</span></span>
<span data-ttu-id="28eea-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="28eea-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="28eea-126">応答</span><span class="sxs-lookup"><span data-stu-id="28eea-126">Response</span></span>
<span data-ttu-id="28eea-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcustomer](../resources/bookingcustomer.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="28eea-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28eea-128">例</span><span class="sxs-lookup"><span data-stu-id="28eea-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28eea-129">要求</span><span class="sxs-lookup"><span data-stu-id="28eea-129">Request</span></span>
<span data-ttu-id="28eea-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="28eea-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28eea-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="28eea-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28eea-132">C#</span><span class="sxs-lookup"><span data-stu-id="28eea-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28eea-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="28eea-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28eea-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="28eea-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="28eea-135">Java</span><span class="sxs-lookup"><span data-stu-id="28eea-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28eea-136">応答</span><span class="sxs-lookup"><span data-stu-id="28eea-136">Response</span></span>
<span data-ttu-id="28eea-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="28eea-137">The following is an example of the response.</span></span> <span data-ttu-id="28eea-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="28eea-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="28eea-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="28eea-139">All of the properties will be returned from an actual call.</span></span>
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
