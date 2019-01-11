---
title: BookingBusiness を削除します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 273c3f3578653e457122b2bf045eb54644ea6b08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849918"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="a1f0c-104">BookingBusiness を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-104">Delete bookingBusiness</span></span>

 > <span data-ttu-id="a1f0c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1f0c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="a1f0c-107">[BookingBusiness](../resources/bookingbusiness.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-107">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1f0c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1f0c-108">Permissions</span></span>
<span data-ttu-id="a1f0c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1f0c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1f0c-111">Permission type</span></span>      | <span data-ttu-id="a1f0c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1f0c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1f0c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1f0c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="a1f0c-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a1f0c-114">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a1f0c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1f0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1f0c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-116">Not supported.</span></span>   |
|<span data-ttu-id="a1f0c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1f0c-117">Application</span></span> | <span data-ttu-id="a1f0c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="a1f0c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1f0c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="a1f0c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1f0c-120">Request headers</span></span>
| <span data-ttu-id="a1f0c-121">名前</span><span class="sxs-lookup"><span data-stu-id="a1f0c-121">Name</span></span>       | <span data-ttu-id="a1f0c-122">説明</span><span class="sxs-lookup"><span data-stu-id="a1f0c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1f0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1f0c-123">Authorization</span></span>  | <span data-ttu-id="a1f0c-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a1f0c-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1f0c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1f0c-125">Request body</span></span>
<span data-ttu-id="a1f0c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a1f0c-127">応答</span><span class="sxs-lookup"><span data-stu-id="a1f0c-127">Response</span></span>
<span data-ttu-id="a1f0c-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1f0c-130">例</span><span class="sxs-lookup"><span data-stu-id="a1f0c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1f0c-131">要求</span><span class="sxs-lookup"><span data-stu-id="a1f0c-131">Request</span></span>
<span data-ttu-id="a1f0c-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="a1f0c-133">応答</span><span class="sxs-lookup"><span data-stu-id="a1f0c-133">Response</span></span>
<span data-ttu-id="a1f0c-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1f0c-134">The following is an example of the response.</span></span> 
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
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
