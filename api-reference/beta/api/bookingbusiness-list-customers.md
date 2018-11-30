---
title: 顧客のリスト
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: a46e8dcc39b69e8391829c176eb01d075d23fccf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068360"
---
# <a name="list-customers"></a><span data-ttu-id="b356f-104">顧客のリスト</span><span class="sxs-lookup"><span data-stu-id="b356f-104">List customers</span></span>

 > <span data-ttu-id="b356f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b356f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b356f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b356f-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b356f-107">[BookingCustomer](../resources/bookingcustomer.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b356f-107">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b356f-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b356f-108">Permissions</span></span>
<span data-ttu-id="b356f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b356f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b356f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b356f-111">Permission type</span></span>      | <span data-ttu-id="b356f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b356f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b356f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b356f-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b356f-114">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b356f-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b356f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b356f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b356f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b356f-116">Not supported.</span></span>   |
|<span data-ttu-id="b356f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b356f-117">Application</span></span> | <span data-ttu-id="b356f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b356f-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="b356f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b356f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b356f-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b356f-120">Optional query parameters</span></span>
<span data-ttu-id="b356f-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b356f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b356f-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b356f-122">Request headers</span></span>
| <span data-ttu-id="b356f-123">名前</span><span class="sxs-lookup"><span data-stu-id="b356f-123">Name</span></span>      |<span data-ttu-id="b356f-124">説明</span><span class="sxs-lookup"><span data-stu-id="b356f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b356f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b356f-125">Authorization</span></span>  | <span data-ttu-id="b356f-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b356f-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b356f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b356f-127">Request body</span></span>
<span data-ttu-id="b356f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b356f-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b356f-129">応答</span><span class="sxs-lookup"><span data-stu-id="b356f-129">Response</span></span>
<span data-ttu-id="b356f-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[bookingCustomer](../resources/bookingcustomer.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b356f-130">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b356f-131">例</span><span class="sxs-lookup"><span data-stu-id="b356f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b356f-132">要求</span><span class="sxs-lookup"><span data-stu-id="b356f-132">Request</span></span>
<span data-ttu-id="b356f-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b356f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
##### <a name="response"></a><span data-ttu-id="b356f-134">応答</span><span class="sxs-lookup"><span data-stu-id="b356f-134">Response</span></span>
<span data-ttu-id="b356f-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b356f-135">The following is an example of the response.</span></span> <span data-ttu-id="b356f-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b356f-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b356f-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b356f-137">All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->