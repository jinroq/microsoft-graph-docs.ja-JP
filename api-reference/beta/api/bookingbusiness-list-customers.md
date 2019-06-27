---
title: 顧客を一覧表示する
description: BookingCustomer オブジェクトのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 069bc29ca920268033981cc458c7eebab527b0a0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258129"
---
# <a name="list-customers"></a><span data-ttu-id="67c12-103">顧客を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="67c12-103">List customers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67c12-104">[Bookingcustomer](../resources/bookingcustomer.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="67c12-104">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="67c12-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67c12-105">Permissions</span></span>
<span data-ttu-id="67c12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67c12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67c12-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67c12-108">Permission type</span></span>      | <span data-ttu-id="67c12-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67c12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67c12-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67c12-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="67c12-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="67c12-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="67c12-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67c12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67c12-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c12-113">Not supported.</span></span>   |
|<span data-ttu-id="67c12-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67c12-114">Application</span></span> | <span data-ttu-id="67c12-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c12-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="67c12-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67c12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67c12-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="67c12-117">Optional query parameters</span></span>
<span data-ttu-id="67c12-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="67c12-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67c12-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67c12-119">Request headers</span></span>
| <span data-ttu-id="67c12-120">名前</span><span class="sxs-lookup"><span data-stu-id="67c12-120">Name</span></span>      |<span data-ttu-id="67c12-121">説明</span><span class="sxs-lookup"><span data-stu-id="67c12-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67c12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67c12-122">Authorization</span></span>  | <span data-ttu-id="67c12-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="67c12-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="67c12-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="67c12-124">Request body</span></span>
<span data-ttu-id="67c12-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="67c12-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="67c12-126">応答</span><span class="sxs-lookup"><span data-stu-id="67c12-126">Response</span></span>
<span data-ttu-id="67c12-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcustomer](../resources/bookingcustomer.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="67c12-127">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67c12-128">例</span><span class="sxs-lookup"><span data-stu-id="67c12-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67c12-129">要求</span><span class="sxs-lookup"><span data-stu-id="67c12-129">Request</span></span>
<span data-ttu-id="67c12-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67c12-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
##### <a name="response"></a><span data-ttu-id="67c12-131">応答</span><span class="sxs-lookup"><span data-stu-id="67c12-131">Response</span></span>
<span data-ttu-id="67c12-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67c12-132">The following is an example of the response.</span></span> <span data-ttu-id="67c12-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="67c12-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="67c12-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="67c12-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers",
    "value": [
        {
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com"
        },
        {
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="67c12-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="67c12-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="67c12-136">C#</span><span class="sxs-lookup"><span data-stu-id="67c12-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_customers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67c12-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="67c12-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_customers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="67c12-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="67c12-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_customers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-customers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-list-customers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list-customers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
