---
title: BookingStaffMember を削除します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 16ee4c5fa244e3507238abd0a696b31477173e11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819776"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="c4663-104">BookingStaffMember を削除します。</span><span class="sxs-lookup"><span data-stu-id="c4663-104">Delete bookingStaffMember</span></span>

 > <span data-ttu-id="c4663-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4663-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4663-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4663-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="c4663-107">指定された[bookingbusiness](../resources/bookingbusiness.md)では、[スタッフ メンバー](../resources/bookingstaffmember.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c4663-107">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c4663-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4663-108">Permissions</span></span>
<span data-ttu-id="c4663-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4663-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4663-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4663-111">Permission type</span></span>      | <span data-ttu-id="c4663-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4663-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4663-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4663-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c4663-114">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c4663-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c4663-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4663-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4663-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4663-116">Not supported.</span></span>   |
|<span data-ttu-id="c4663-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4663-117">Application</span></span> | <span data-ttu-id="c4663-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4663-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c4663-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4663-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c4663-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4663-120">Request headers</span></span>
| <span data-ttu-id="c4663-121">名前</span><span class="sxs-lookup"><span data-stu-id="c4663-121">Name</span></span>       | <span data-ttu-id="c4663-122">説明</span><span class="sxs-lookup"><span data-stu-id="c4663-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4663-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4663-123">Authorization</span></span>  | <span data-ttu-id="c4663-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c4663-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4663-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4663-125">Request body</span></span>
<span data-ttu-id="c4663-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c4663-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c4663-127">応答</span><span class="sxs-lookup"><span data-stu-id="c4663-127">Response</span></span>
<span data-ttu-id="c4663-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c4663-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4663-130">例</span><span class="sxs-lookup"><span data-stu-id="c4663-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4663-131">要求</span><span class="sxs-lookup"><span data-stu-id="c4663-131">Request</span></span>
<span data-ttu-id="c4663-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c4663-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
##### <a name="response"></a><span data-ttu-id="c4663-133">応答</span><span class="sxs-lookup"><span data-stu-id="c4663-133">Response</span></span>
<span data-ttu-id="c4663-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c4663-134">The following is an example of the response.</span></span> 
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
  "description": "Delete bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
