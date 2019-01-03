---
title: Bookingcustomer を更新します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: d28a2a30da1c626c65c65a1dc3cab000a06580d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068021"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="801b7-104">Bookingcustomer を更新します。</span><span class="sxs-lookup"><span data-stu-id="801b7-104">Update bookingcustomer</span></span>

 > <span data-ttu-id="801b7-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="801b7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="801b7-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="801b7-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="801b7-107">[BookingCustomer](../resources/bookingcustomer.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="801b7-107">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="801b7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="801b7-108">Permissions</span></span>
<span data-ttu-id="801b7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="801b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="801b7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="801b7-111">Permission type</span></span>      | <span data-ttu-id="801b7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="801b7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="801b7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="801b7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="801b7-114">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="801b7-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="801b7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="801b7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="801b7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="801b7-116">Not supported.</span></span>   |
|<span data-ttu-id="801b7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="801b7-117">Application</span></span> | <span data-ttu-id="801b7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="801b7-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="801b7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="801b7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="801b7-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="801b7-120">Optional request headers</span></span>
| <span data-ttu-id="801b7-121">名前</span><span class="sxs-lookup"><span data-stu-id="801b7-121">Name</span></span>       | <span data-ttu-id="801b7-122">説明</span><span class="sxs-lookup"><span data-stu-id="801b7-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="801b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="801b7-123">Authorization</span></span>  | <span data-ttu-id="801b7-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="801b7-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="801b7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="801b7-125">Request body</span></span>
<span data-ttu-id="801b7-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="801b7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="801b7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="801b7-129">Property</span></span>     | <span data-ttu-id="801b7-130">型</span><span class="sxs-lookup"><span data-stu-id="801b7-130">Type</span></span>   |<span data-ttu-id="801b7-131">説明</span><span class="sxs-lookup"><span data-stu-id="801b7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="801b7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="801b7-132">displayName</span></span>|<span data-ttu-id="801b7-133">String</span><span class="sxs-lookup"><span data-stu-id="801b7-133">String</span></span>|<span data-ttu-id="801b7-134">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="801b7-134">The name of the customer.</span></span>|
|<span data-ttu-id="801b7-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="801b7-135">emailAddress</span></span>|<span data-ttu-id="801b7-136">String</span><span class="sxs-lookup"><span data-stu-id="801b7-136">String</span></span>|<span data-ttu-id="801b7-137">お客様の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="801b7-137">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="801b7-138">応答</span><span class="sxs-lookup"><span data-stu-id="801b7-138">Response</span></span>
<span data-ttu-id="801b7-139">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[bookingCustomer](../resources/bookingcustomer.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="801b7-139">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="801b7-140">例</span><span class="sxs-lookup"><span data-stu-id="801b7-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="801b7-141">要求</span><span class="sxs-lookup"><span data-stu-id="801b7-141">Request</span></span>
<span data-ttu-id="801b7-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="801b7-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
##### <a name="response"></a><span data-ttu-id="801b7-143">応答</span><span class="sxs-lookup"><span data-stu-id="801b7-143">Response</span></span>
<span data-ttu-id="801b7-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="801b7-144">The following is an example of the response.</span></span> <span data-ttu-id="801b7-145">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="801b7-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="801b7-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="801b7-146">All of the properties will be returned from an actual call.</span></span>
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
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->