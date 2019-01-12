---
title: BookingCustomer を取得します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 38a0fa87bc3b81c493914b14a8c35a01dad11689
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27989992"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="e65f1-104">BookingCustomer を取得します。</span><span class="sxs-lookup"><span data-stu-id="e65f1-104">Get bookingCustomer</span></span>

 > <span data-ttu-id="e65f1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e65f1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e65f1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e65f1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e65f1-107">プロパティと、 [bookingCustomer](../resources/bookingcustomer.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="e65f1-107">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e65f1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e65f1-108">Permissions</span></span>
<span data-ttu-id="e65f1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e65f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e65f1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e65f1-111">Permission type</span></span>      | <span data-ttu-id="e65f1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e65f1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e65f1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e65f1-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e65f1-114">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e65f1-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e65f1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e65f1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e65f1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e65f1-116">Not supported.</span></span>   |
|<span data-ttu-id="e65f1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e65f1-117">Application</span></span> | <span data-ttu-id="e65f1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e65f1-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="e65f1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e65f1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e65f1-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e65f1-120">Optional query parameters</span></span>
<span data-ttu-id="e65f1-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e65f1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e65f1-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e65f1-122">Request headers</span></span>
| <span data-ttu-id="e65f1-123">名前</span><span class="sxs-lookup"><span data-stu-id="e65f1-123">Name</span></span>      |<span data-ttu-id="e65f1-124">説明</span><span class="sxs-lookup"><span data-stu-id="e65f1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e65f1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e65f1-125">Authorization</span></span>  | <span data-ttu-id="e65f1-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e65f1-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e65f1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e65f1-127">Request body</span></span>
<span data-ttu-id="e65f1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e65f1-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e65f1-129">応答</span><span class="sxs-lookup"><span data-stu-id="e65f1-129">Response</span></span>
<span data-ttu-id="e65f1-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[bookingCustomer](../resources/bookingcustomer.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e65f1-130">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e65f1-131">例</span><span class="sxs-lookup"><span data-stu-id="e65f1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e65f1-132">要求</span><span class="sxs-lookup"><span data-stu-id="e65f1-132">Request</span></span>
<span data-ttu-id="e65f1-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e65f1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
##### <a name="response"></a><span data-ttu-id="e65f1-134">応答</span><span class="sxs-lookup"><span data-stu-id="e65f1-134">Response</span></span>
<span data-ttu-id="e65f1-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e65f1-135">The following is an example of the response.</span></span> <span data-ttu-id="e65f1-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e65f1-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e65f1-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e65f1-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
