---
title: リスト bookingCurrencies
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 809ee9222f8ae997633becbe13f87539dd816b1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849218"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="4f808-104">リスト bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="4f808-104">List bookingCurrencies</span></span>

 > <span data-ttu-id="4f808-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f808-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f808-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f808-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="4f808-107">Microsoft 予約業務に利用可能な[bookingCurrency](../resources/bookingcurrency.md)のオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="4f808-107">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f808-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f808-108">Permissions</span></span>
<span data-ttu-id="4f808-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f808-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f808-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f808-111">Permission type</span></span>      | <span data-ttu-id="4f808-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f808-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f808-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f808-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4f808-114">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4f808-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4f808-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f808-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f808-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f808-116">Not supported.</span></span>   |
|<span data-ttu-id="4f808-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f808-117">Application</span></span> | <span data-ttu-id="4f808-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f808-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="4f808-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f808-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4f808-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4f808-120">Optional query parameters</span></span>
<span data-ttu-id="4f808-121">このメソッドは、$count、$filter、$select、$skip、$top など、応答をカスタマイズするために[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4f808-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f808-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f808-122">Request headers</span></span>
| <span data-ttu-id="4f808-123">名前</span><span class="sxs-lookup"><span data-stu-id="4f808-123">Name</span></span>      |<span data-ttu-id="4f808-124">説明</span><span class="sxs-lookup"><span data-stu-id="4f808-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f808-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f808-125">Authorization</span></span>  | <span data-ttu-id="4f808-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4f808-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f808-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f808-127">Request body</span></span>
<span data-ttu-id="4f808-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4f808-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4f808-129">応答</span><span class="sxs-lookup"><span data-stu-id="4f808-129">Response</span></span>
<span data-ttu-id="4f808-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[bookingCurrency](../resources/bookingcurrency.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4f808-130">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f808-131">例</span><span class="sxs-lookup"><span data-stu-id="4f808-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f808-132">要求</span><span class="sxs-lookup"><span data-stu-id="4f808-132">Request</span></span>
<span data-ttu-id="4f808-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f808-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="4f808-134">応答</span><span class="sxs-lookup"><span data-stu-id="4f808-134">Response</span></span>
<span data-ttu-id="4f808-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f808-135">The following is an example of the response.</span></span> <span data-ttu-id="4f808-136">注: ここに示す応答オブジェクトは、簡潔にするため切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="4f808-136">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="4f808-137">すべてのサポートされている通貨とプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4f808-137">All of the supported currencies and properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
