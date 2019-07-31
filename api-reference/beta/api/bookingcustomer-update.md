---
title: Bookingcustomer を更新する
description: BookingCustomer オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 933f272d8addcaf0528e5c141291d8f81f3ecb43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944969"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="8e330-103">Bookingcustomer を更新する</span><span class="sxs-lookup"><span data-stu-id="8e330-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e330-104">[Bookingcustomer](../resources/bookingcustomer.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e330-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8e330-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e330-105">Permissions</span></span>
<span data-ttu-id="8e330-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e330-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e330-108">Permission type</span></span>      | <span data-ttu-id="8e330-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e330-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e330-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e330-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e330-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="8e330-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8e330-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e330-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e330-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e330-113">Not supported.</span></span>   |
|<span data-ttu-id="8e330-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e330-114">Application</span></span> | <span data-ttu-id="8e330-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e330-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8e330-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e330-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="8e330-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e330-117">Optional request headers</span></span>
| <span data-ttu-id="8e330-118">名前</span><span class="sxs-lookup"><span data-stu-id="8e330-118">Name</span></span>       | <span data-ttu-id="8e330-119">説明</span><span class="sxs-lookup"><span data-stu-id="8e330-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8e330-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e330-120">Authorization</span></span>  | <span data-ttu-id="8e330-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8e330-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e330-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e330-122">Request body</span></span>
<span data-ttu-id="8e330-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="8e330-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e330-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e330-126">Property</span></span>     | <span data-ttu-id="8e330-127">型</span><span class="sxs-lookup"><span data-stu-id="8e330-127">Type</span></span>   |<span data-ttu-id="8e330-128">説明</span><span class="sxs-lookup"><span data-stu-id="8e330-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e330-129">displayName</span><span class="sxs-lookup"><span data-stu-id="8e330-129">displayName</span></span>|<span data-ttu-id="8e330-130">String</span><span class="sxs-lookup"><span data-stu-id="8e330-130">String</span></span>|<span data-ttu-id="8e330-131">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="8e330-131">The name of the customer.</span></span>|
|<span data-ttu-id="8e330-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8e330-132">emailAddress</span></span>|<span data-ttu-id="8e330-133">String</span><span class="sxs-lookup"><span data-stu-id="8e330-133">String</span></span>|<span data-ttu-id="8e330-134">顧客の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="8e330-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="8e330-135">応答</span><span class="sxs-lookup"><span data-stu-id="8e330-135">Response</span></span>
<span data-ttu-id="8e330-136">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[bookingcustomer](../resources/bookingcustomer.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8e330-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e330-137">例</span><span class="sxs-lookup"><span data-stu-id="8e330-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e330-138">要求</span><span class="sxs-lookup"><span data-stu-id="8e330-138">Request</span></span>
<span data-ttu-id="8e330-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e330-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e330-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8e330-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e330-141">C#</span><span class="sxs-lookup"><span data-stu-id="8e330-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e330-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="8e330-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e330-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="8e330-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e330-144">Java</span><span class="sxs-lookup"><span data-stu-id="8e330-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8e330-145">応答</span><span class="sxs-lookup"><span data-stu-id="8e330-145">Response</span></span>
<span data-ttu-id="8e330-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e330-146">The following is an example of the response.</span></span> <span data-ttu-id="8e330-147">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8e330-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8e330-148">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8e330-148">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
