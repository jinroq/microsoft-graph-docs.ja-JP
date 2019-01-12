---
title: BookingCustomer を作成します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 555723fdb4eb7bacb2c876ed3fd87eb539a5239d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922257"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="6f6f3-104">BookingCustomer を作成します。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-104">Create bookingCustomer</span></span>

 > <span data-ttu-id="6f6f3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f6f3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="6f6f3-107">新しい[bookingCustomer](../resources/bookingcustomer.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-107">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f6f3-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6f6f3-108">Permissions</span></span>
<span data-ttu-id="6f6f3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6f3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f6f3-111">Permission type</span></span>      | <span data-ttu-id="6f6f3-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f6f3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f6f3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f6f3-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="6f6f3-114">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6f6f3-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6f6f3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f6f3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f6f3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-116">Not supported.</span></span>   |
|<span data-ttu-id="6f6f3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f6f3-117">Application</span></span> | <span data-ttu-id="6f6f3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="6f6f3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f6f3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="6f6f3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f6f3-120">Request headers</span></span>
| <span data-ttu-id="6f6f3-121">名前</span><span class="sxs-lookup"><span data-stu-id="6f6f3-121">Name</span></span>       | <span data-ttu-id="6f6f3-122">説明</span><span class="sxs-lookup"><span data-stu-id="6f6f3-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f6f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f6f3-123">Authorization</span></span>  | <span data-ttu-id="6f6f3-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6f6f3-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6f3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f6f3-125">Request body</span></span>
<span data-ttu-id="6f6f3-126">要求の本文には、 [bookingCustomer](../resources/bookingcustomer.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-126">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="6f6f3-127">応答</span><span class="sxs-lookup"><span data-stu-id="6f6f3-127">Response</span></span>
<span data-ttu-id="6f6f3-128">かどうかは成功すると、このメソッドを返します`201, Created`、応答の本体で応答コードと[bookingCustomer](../resources/bookingcustomer.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-128">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f6f3-129">例</span><span class="sxs-lookup"><span data-stu-id="6f6f3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f6f3-130">要求</span><span class="sxs-lookup"><span data-stu-id="6f6f3-130">Request</span></span>
<span data-ttu-id="6f6f3-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="6f6f3-132">要求の本文には、 [bookingCustomer](../resources/bookingcustomer.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-132">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6f6f3-133">応答</span><span class="sxs-lookup"><span data-stu-id="6f6f3-133">Response</span></span>
<span data-ttu-id="6f6f3-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-134">The following is an example of the response.</span></span> <span data-ttu-id="6f6f3-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6f6f3-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6f6f3-136">All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
