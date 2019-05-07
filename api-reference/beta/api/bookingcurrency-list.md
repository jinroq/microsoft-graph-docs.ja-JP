---
title: BookingCurrencies のリスト
description: Microsoft の予約ビジネスで使用できる bookingCurrency オブジェクトの一覧を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d33f5980d41620487be95f6d2b30175b2238bb38
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636080"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="bed45-103">BookingCurrencies のリスト</span><span class="sxs-lookup"><span data-stu-id="bed45-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bed45-104">Microsoft の予約ビジネスで使用できる[Bookingcurrency](../resources/bookingcurrency.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="bed45-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="bed45-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bed45-105">Permissions</span></span>
<span data-ttu-id="bed45-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bed45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bed45-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bed45-108">Permission type</span></span>      | <span data-ttu-id="bed45-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bed45-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bed45-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bed45-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bed45-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="bed45-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bed45-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bed45-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bed45-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bed45-113">Not supported.</span></span>   |
|<span data-ttu-id="bed45-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bed45-114">Application</span></span> | <span data-ttu-id="bed45-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bed45-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bed45-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bed45-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bed45-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bed45-117">Optional query parameters</span></span>
<span data-ttu-id="bed45-118">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters) ($count、$filter、$select、$skip、$top を含む) をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bed45-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bed45-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bed45-119">Request headers</span></span>
| <span data-ttu-id="bed45-120">名前</span><span class="sxs-lookup"><span data-stu-id="bed45-120">Name</span></span>      |<span data-ttu-id="bed45-121">説明</span><span class="sxs-lookup"><span data-stu-id="bed45-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bed45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bed45-122">Authorization</span></span>  | <span data-ttu-id="bed45-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bed45-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bed45-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="bed45-124">Request body</span></span>
<span data-ttu-id="bed45-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bed45-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bed45-126">応答</span><span class="sxs-lookup"><span data-stu-id="bed45-126">Response</span></span>
<span data-ttu-id="bed45-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcurrency](../resources/bookingcurrency.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bed45-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bed45-128">例</span><span class="sxs-lookup"><span data-stu-id="bed45-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bed45-129">要求</span><span class="sxs-lookup"><span data-stu-id="bed45-129">Request</span></span>
<span data-ttu-id="bed45-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bed45-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="bed45-131">応答</span><span class="sxs-lookup"><span data-stu-id="bed45-131">Response</span></span>
<span data-ttu-id="bed45-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bed45-132">The following is an example of the response.</span></span> <span data-ttu-id="bed45-133">注: 簡潔にするために、ここに示す response オブジェクトは切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="bed45-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="bed45-134">サポートされているすべての通貨およびプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bed45-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bed45-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="bed45-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bed45-136">Visual</span><span class="sxs-lookup"><span data-stu-id="bed45-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bed45-137">Java</span><span class="sxs-lookup"><span data-stu-id="bed45-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
