---
title: BookingCurrency を取得します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 3b39b6ba83f77f9b47661e3bf4a98330b5f7ee0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855063"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="51563-104">BookingCurrency を取得します。</span><span class="sxs-lookup"><span data-stu-id="51563-104">Get bookingCurrency</span></span>

 > <span data-ttu-id="51563-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51563-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51563-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51563-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="51563-107">Microsoft 予約ビジネスに提供される[bookingCurrency](../resources/bookingcurrency.md)オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="51563-107">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="51563-108">通貨コードでは、 **id**プロパティを使用すると、通貨を指定します。</span><span class="sxs-lookup"><span data-stu-id="51563-108">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="51563-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="51563-109">Permissions</span></span>
<span data-ttu-id="51563-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51563-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51563-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51563-112">Permission type</span></span>      | <span data-ttu-id="51563-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="51563-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51563-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51563-114">Delegated (work or school account)</span></span> | <span data-ttu-id="51563-115">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="51563-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="51563-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51563-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51563-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51563-117">Not supported.</span></span>   |
|<span data-ttu-id="51563-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51563-118">Application</span></span> | <span data-ttu-id="51563-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51563-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="51563-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51563-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="51563-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="51563-121">Optional query parameters</span></span>
<span data-ttu-id="51563-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="51563-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51563-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51563-123">Request headers</span></span>
| <span data-ttu-id="51563-124">名前</span><span class="sxs-lookup"><span data-stu-id="51563-124">Name</span></span>      |<span data-ttu-id="51563-125">説明</span><span class="sxs-lookup"><span data-stu-id="51563-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51563-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="51563-126">Authorization</span></span>  | <span data-ttu-id="51563-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="51563-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="51563-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="51563-128">Request body</span></span>
<span data-ttu-id="51563-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="51563-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="51563-130">応答</span><span class="sxs-lookup"><span data-stu-id="51563-130">Response</span></span>
<span data-ttu-id="51563-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[bookingCurrency](../resources/bookingcurrency.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="51563-131">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51563-132">例</span><span class="sxs-lookup"><span data-stu-id="51563-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51563-133">要求</span><span class="sxs-lookup"><span data-stu-id="51563-133">Request</span></span>
<span data-ttu-id="51563-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51563-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="51563-135">応答</span><span class="sxs-lookup"><span data-stu-id="51563-135">Response</span></span>
<span data-ttu-id="51563-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51563-136">The following is an example of the response.</span></span> <span data-ttu-id="51563-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="51563-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="51563-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="51563-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
