---
title: BookingCurrency の取得
description: Microsoft の予約業務で利用できる bookingCurrency オブジェクトのプロパティを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b3e6c49ef67d97b636ed29d84a2e085c90305b1f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419441"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="bdd36-103">BookingCurrency の取得</span><span class="sxs-lookup"><span data-stu-id="bdd36-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdd36-104">Microsoft の予約業務で利用できる[Bookingcurrency](../resources/bookingcurrency.md)オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="bdd36-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="bdd36-105">通貨を指定するには、通貨コードである**id**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="bdd36-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd36-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bdd36-106">Permissions</span></span>
<span data-ttu-id="bdd36-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bdd36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd36-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bdd36-109">Permission type</span></span>      | <span data-ttu-id="bdd36-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bdd36-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd36-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bdd36-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bdd36-112">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="bdd36-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bdd36-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bdd36-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd36-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdd36-114">Not supported.</span></span>   |
|<span data-ttu-id="bdd36-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bdd36-115">Application</span></span> | <span data-ttu-id="bdd36-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdd36-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bdd36-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bdd36-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bdd36-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bdd36-118">Optional query parameters</span></span>
<span data-ttu-id="bdd36-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bdd36-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdd36-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdd36-120">Request headers</span></span>
| <span data-ttu-id="bdd36-121">名前</span><span class="sxs-lookup"><span data-stu-id="bdd36-121">Name</span></span>      |<span data-ttu-id="bdd36-122">説明</span><span class="sxs-lookup"><span data-stu-id="bdd36-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bdd36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdd36-123">Authorization</span></span>  | <span data-ttu-id="bdd36-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bdd36-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdd36-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bdd36-125">Request body</span></span>
<span data-ttu-id="bdd36-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bdd36-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bdd36-127">応答</span><span class="sxs-lookup"><span data-stu-id="bdd36-127">Response</span></span>
<span data-ttu-id="bdd36-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcurrency](../resources/bookingcurrency.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bdd36-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bdd36-129">例</span><span class="sxs-lookup"><span data-stu-id="bdd36-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdd36-130">要求</span><span class="sxs-lookup"><span data-stu-id="bdd36-130">Request</span></span>
<span data-ttu-id="bdd36-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bdd36-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bdd36-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bdd36-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bdd36-133">C#</span><span class="sxs-lookup"><span data-stu-id="bdd36-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdd36-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdd36-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bdd36-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="bdd36-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bdd36-136">応答</span><span class="sxs-lookup"><span data-stu-id="bdd36-136">Response</span></span>
<span data-ttu-id="bdd36-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bdd36-137">The following is an example of the response.</span></span> <span data-ttu-id="bdd36-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="bdd36-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bdd36-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bdd36-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 50

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingCurrencies/$entity",
    "id": "USD",
    "symbol": "$"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
