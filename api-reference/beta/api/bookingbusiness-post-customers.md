---
title: BookingCustomer の作成
description: 新しい Bookcustomer オブジェクトを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a7ad80e8caf0e8c38479fc58dc7b677c58617770
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258157"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="c8f3c-103">BookingCustomer の作成</span><span class="sxs-lookup"><span data-stu-id="c8f3c-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8f3c-104">新しい[Bookcustomer](../resources/bookingcustomer.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8f3c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8f3c-105">Permissions</span></span>
<span data-ttu-id="c8f3c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8f3c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8f3c-108">Permission type</span></span>      | <span data-ttu-id="c8f3c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8f3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8f3c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8f3c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c8f3c-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="c8f3c-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c8f3c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8f3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8f3c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-113">Not supported.</span></span>   |
|<span data-ttu-id="c8f3c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8f3c-114">Application</span></span> | <span data-ttu-id="c8f3c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c8f3c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8f3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="c8f3c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8f3c-117">Request headers</span></span>
| <span data-ttu-id="c8f3c-118">名前</span><span class="sxs-lookup"><span data-stu-id="c8f3c-118">Name</span></span>       | <span data-ttu-id="c8f3c-119">説明</span><span class="sxs-lookup"><span data-stu-id="c8f3c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8f3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8f3c-120">Authorization</span></span>  | <span data-ttu-id="c8f3c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c8f3c-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8f3c-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8f3c-122">Request body</span></span>
<span data-ttu-id="c8f3c-123">要求本文で、 [Bookingcustomer](../resources/bookingcustomer.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c8f3c-124">応答</span><span class="sxs-lookup"><span data-stu-id="c8f3c-124">Response</span></span>
<span data-ttu-id="c8f3c-125">成功した場合、この`201, Created`メソッドは応答コードと、応答本文で[customer](../resources/bookingcustomer.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8f3c-126">例</span><span class="sxs-lookup"><span data-stu-id="c8f3c-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8f3c-127">要求</span><span class="sxs-lookup"><span data-stu-id="c8f3c-127">Request</span></span>
<span data-ttu-id="c8f3c-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
<span data-ttu-id="c8f3c-129">要求本文で、 [Bookingcustomer](../resources/bookingcustomer.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c8f3c-130">応答</span><span class="sxs-lookup"><span data-stu-id="c8f3c-130">Response</span></span>
<span data-ttu-id="c8f3c-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-131">The following is an example of the response.</span></span> <span data-ttu-id="c8f3c-132">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c8f3c-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c8f3c-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c8f3c-134">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c8f3c-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c8f3c-135">C#</span><span class="sxs-lookup"><span data-stu-id="c8f3c-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8f3c-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8f3c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c8f3c-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="c8f3c-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
