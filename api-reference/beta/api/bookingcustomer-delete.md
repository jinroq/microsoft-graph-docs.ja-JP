---
title: BookingCustomer を削除します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: c4ba9267e2a3fde3ac43460160ffd4bb37cfb56d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068355"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="1e78b-104">BookingCustomer を削除します。</span><span class="sxs-lookup"><span data-stu-id="1e78b-104">Delete bookingCustomer</span></span>

 > <span data-ttu-id="1e78b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e78b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e78b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e78b-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1e78b-107">指定した[bookingCustomer](../resources/bookingcustomer.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1e78b-107">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e78b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e78b-108">Permissions</span></span>
<span data-ttu-id="1e78b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e78b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e78b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e78b-111">Permission type</span></span>      | <span data-ttu-id="1e78b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e78b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e78b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e78b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1e78b-114">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="1e78b-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1e78b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e78b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e78b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e78b-116">Not supported.</span></span>   |
|<span data-ttu-id="1e78b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e78b-117">Application</span></span> | <span data-ttu-id="1e78b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e78b-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="1e78b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e78b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1e78b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e78b-120">Request headers</span></span>
| <span data-ttu-id="1e78b-121">名前</span><span class="sxs-lookup"><span data-stu-id="1e78b-121">Name</span></span>       | <span data-ttu-id="1e78b-122">説明</span><span class="sxs-lookup"><span data-stu-id="1e78b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e78b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e78b-123">Authorization</span></span>  | <span data-ttu-id="1e78b-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1e78b-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e78b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e78b-125">Request body</span></span>
<span data-ttu-id="1e78b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e78b-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1e78b-127">応答</span><span class="sxs-lookup"><span data-stu-id="1e78b-127">Response</span></span>
<span data-ttu-id="1e78b-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1e78b-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e78b-130">例</span><span class="sxs-lookup"><span data-stu-id="1e78b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e78b-131">要求</span><span class="sxs-lookup"><span data-stu-id="1e78b-131">Request</span></span>
<span data-ttu-id="1e78b-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e78b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="1e78b-133">応答</span><span class="sxs-lookup"><span data-stu-id="1e78b-133">Response</span></span>
<span data-ttu-id="1e78b-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e78b-134">The following is an example of the response.</span></span> <span data-ttu-id="1e78b-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="1e78b-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1e78b-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e78b-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->