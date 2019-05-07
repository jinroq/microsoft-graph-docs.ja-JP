---
title: BookingCustomer を取得する
description: BookingCustomer オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3d6b51dc43d5f713dbdb99733cf05ca66c1e31f0
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636024"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="568b5-103">BookingCustomer を取得する</span><span class="sxs-lookup"><span data-stu-id="568b5-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="568b5-104">[Bookingcustomer](../resources/bookingcustomer.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="568b5-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="568b5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="568b5-105">Permissions</span></span>
<span data-ttu-id="568b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="568b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="568b5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="568b5-108">Permission type</span></span>      | <span data-ttu-id="568b5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="568b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="568b5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="568b5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="568b5-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="568b5-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="568b5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="568b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="568b5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="568b5-113">Not supported.</span></span>   |
|<span data-ttu-id="568b5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="568b5-114">Application</span></span> | <span data-ttu-id="568b5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="568b5-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="568b5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="568b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="568b5-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="568b5-117">Optional query parameters</span></span>
<span data-ttu-id="568b5-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="568b5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="568b5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="568b5-119">Request headers</span></span>
| <span data-ttu-id="568b5-120">名前</span><span class="sxs-lookup"><span data-stu-id="568b5-120">Name</span></span>      |<span data-ttu-id="568b5-121">説明</span><span class="sxs-lookup"><span data-stu-id="568b5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="568b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="568b5-122">Authorization</span></span>  | <span data-ttu-id="568b5-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="568b5-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="568b5-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="568b5-124">Request body</span></span>
<span data-ttu-id="568b5-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="568b5-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="568b5-126">応答</span><span class="sxs-lookup"><span data-stu-id="568b5-126">Response</span></span>
<span data-ttu-id="568b5-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcustomer](../resources/bookingcustomer.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="568b5-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="568b5-128">例</span><span class="sxs-lookup"><span data-stu-id="568b5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="568b5-129">要求</span><span class="sxs-lookup"><span data-stu-id="568b5-129">Request</span></span>
<span data-ttu-id="568b5-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="568b5-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
##### <a name="response"></a><span data-ttu-id="568b5-131">応答</span><span class="sxs-lookup"><span data-stu-id="568b5-131">Response</span></span>
<span data-ttu-id="568b5-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="568b5-132">The following is an example of the response.</span></span> <span data-ttu-id="568b5-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="568b5-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="568b5-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="568b5-134">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="568b5-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="568b5-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="568b5-136">Visual</span><span class="sxs-lookup"><span data-stu-id="568b5-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingcustomer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="568b5-137">Java</span><span class="sxs-lookup"><span data-stu-id="568b5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingcustomer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingcustomer-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcustomer-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
