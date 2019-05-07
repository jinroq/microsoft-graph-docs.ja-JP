---
title: Bookingcustomer を更新する
description: BookingCustomer オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b9f30ba1fb17e9019910a2aaa55dff408b626122
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636038"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="d06fe-103">Bookingcustomer を更新する</span><span class="sxs-lookup"><span data-stu-id="d06fe-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d06fe-104">[Bookingcustomer](../resources/bookingcustomer.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d06fe-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d06fe-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d06fe-105">Permissions</span></span>
<span data-ttu-id="d06fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d06fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d06fe-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d06fe-108">Permission type</span></span>      | <span data-ttu-id="d06fe-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d06fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d06fe-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d06fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d06fe-111">BookingsAppointment すべての予約。すべて、予約....</span><span class="sxs-lookup"><span data-stu-id="d06fe-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d06fe-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d06fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d06fe-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d06fe-113">Not supported.</span></span>   |
|<span data-ttu-id="d06fe-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d06fe-114">Application</span></span> | <span data-ttu-id="d06fe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d06fe-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d06fe-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d06fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d06fe-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d06fe-117">Optional request headers</span></span>
| <span data-ttu-id="d06fe-118">名前</span><span class="sxs-lookup"><span data-stu-id="d06fe-118">Name</span></span>       | <span data-ttu-id="d06fe-119">説明</span><span class="sxs-lookup"><span data-stu-id="d06fe-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d06fe-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d06fe-120">Authorization</span></span>  | <span data-ttu-id="d06fe-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d06fe-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d06fe-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="d06fe-122">Request body</span></span>
<span data-ttu-id="d06fe-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="d06fe-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d06fe-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d06fe-126">Property</span></span>     | <span data-ttu-id="d06fe-127">型</span><span class="sxs-lookup"><span data-stu-id="d06fe-127">Type</span></span>   |<span data-ttu-id="d06fe-128">説明</span><span class="sxs-lookup"><span data-stu-id="d06fe-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d06fe-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d06fe-129">displayName</span></span>|<span data-ttu-id="d06fe-130">String</span><span class="sxs-lookup"><span data-stu-id="d06fe-130">String</span></span>|<span data-ttu-id="d06fe-131">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="d06fe-131">The name of the customer.</span></span>|
|<span data-ttu-id="d06fe-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d06fe-132">emailAddress</span></span>|<span data-ttu-id="d06fe-133">String</span><span class="sxs-lookup"><span data-stu-id="d06fe-133">String</span></span>|<span data-ttu-id="d06fe-134">顧客の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="d06fe-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="d06fe-135">応答</span><span class="sxs-lookup"><span data-stu-id="d06fe-135">Response</span></span>
<span data-ttu-id="d06fe-136">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[bookingcustomer](../resources/bookingcustomer.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d06fe-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d06fe-137">例</span><span class="sxs-lookup"><span data-stu-id="d06fe-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d06fe-138">要求</span><span class="sxs-lookup"><span data-stu-id="d06fe-138">Request</span></span>
<span data-ttu-id="d06fe-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d06fe-139">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d06fe-140">応答</span><span class="sxs-lookup"><span data-stu-id="d06fe-140">Response</span></span>
<span data-ttu-id="d06fe-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d06fe-141">The following is an example of the response.</span></span> <span data-ttu-id="d06fe-142">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d06fe-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d06fe-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d06fe-143">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d06fe-144">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="d06fe-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d06fe-145">Visual</span><span class="sxs-lookup"><span data-stu-id="d06fe-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingcustomer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d06fe-146">Java</span><span class="sxs-lookup"><span data-stu-id="d06fe-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingcustomer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingcustomer-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcustomer-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
