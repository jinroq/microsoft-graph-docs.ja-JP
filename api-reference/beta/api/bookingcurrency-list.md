---
title: BookingCurrencies のリスト
description: Microsoft の予約ビジネスで使用できる bookingCurrency オブジェクトの一覧を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 23be76f3b2741918d414043a00a5e56017a3dad8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257947"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="277e6-103">BookingCurrencies のリスト</span><span class="sxs-lookup"><span data-stu-id="277e6-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="277e6-104">Microsoft の予約ビジネスで使用できる[Bookingcurrency](../resources/bookingcurrency.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="277e6-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="277e6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="277e6-105">Permissions</span></span>
<span data-ttu-id="277e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="277e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="277e6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="277e6-108">Permission type</span></span>      | <span data-ttu-id="277e6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="277e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="277e6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="277e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="277e6-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="277e6-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="277e6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="277e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="277e6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="277e6-113">Not supported.</span></span>   |
|<span data-ttu-id="277e6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="277e6-114">Application</span></span> | <span data-ttu-id="277e6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="277e6-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="277e6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="277e6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="277e6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="277e6-117">Optional query parameters</span></span>
<span data-ttu-id="277e6-118">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters) ($count、$filter、$select、$skip、$top を含む) をサポートします。</span><span class="sxs-lookup"><span data-stu-id="277e6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="277e6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="277e6-119">Request headers</span></span>
| <span data-ttu-id="277e6-120">名前</span><span class="sxs-lookup"><span data-stu-id="277e6-120">Name</span></span>      |<span data-ttu-id="277e6-121">説明</span><span class="sxs-lookup"><span data-stu-id="277e6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="277e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="277e6-122">Authorization</span></span>  | <span data-ttu-id="277e6-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="277e6-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="277e6-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="277e6-124">Request body</span></span>
<span data-ttu-id="277e6-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="277e6-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="277e6-126">応答</span><span class="sxs-lookup"><span data-stu-id="277e6-126">Response</span></span>
<span data-ttu-id="277e6-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcurrency](../resources/bookingcurrency.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="277e6-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="277e6-128">例</span><span class="sxs-lookup"><span data-stu-id="277e6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="277e6-129">要求</span><span class="sxs-lookup"><span data-stu-id="277e6-129">Request</span></span>
<span data-ttu-id="277e6-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="277e6-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="277e6-131">応答</span><span class="sxs-lookup"><span data-stu-id="277e6-131">Response</span></span>
<span data-ttu-id="277e6-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="277e6-132">The following is an example of the response.</span></span> <span data-ttu-id="277e6-133">注: 簡潔にするために、ここに示す response オブジェクトは切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="277e6-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="277e6-134">サポートされているすべての通貨およびプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="277e6-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingCurrencies",
    "value":[
        {
            "id":"AED",
            "symbol":"د.إ.‏"
        },
        {
            "id":"AFN",
            "symbol":"؋"
        },
        {
            "id":"ALL",
            "symbol":"Lekë"
        },
        {
            "id":"AMD",
            "symbol":"֏"
        },
        {
            "id":"USD",
            "symbol":"$"
        },
        {
            "id":"YER",
            "symbol":"ر.ي.‏"
        },
        {
            "id":"ZAR",
            "symbol":"R"
        },
        {
            "id":"ZMW",
            "symbol":"K"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="277e6-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="277e6-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="277e6-136">C#</span><span class="sxs-lookup"><span data-stu-id="277e6-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="277e6-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="277e6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="277e6-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="277e6-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
