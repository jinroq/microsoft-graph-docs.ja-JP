---
title: BookingBusiness の削除
description: BookingBusiness オブジェクトを削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6c5f68ec3df3256f94454ebbe3f0253375e98776
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865806"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="76498-103">BookingBusiness の削除</span><span class="sxs-lookup"><span data-stu-id="76498-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76498-104">[Bookingbusiness](../resources/bookingbusiness.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="76498-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="76498-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="76498-105">Permissions</span></span>
<span data-ttu-id="76498-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76498-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76498-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76498-108">Permission type</span></span>      | <span data-ttu-id="76498-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="76498-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76498-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76498-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="76498-111">予約。すべて</span><span class="sxs-lookup"><span data-stu-id="76498-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="76498-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76498-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76498-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76498-113">Not supported.</span></span>   |
|<span data-ttu-id="76498-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76498-114">Application</span></span> | <span data-ttu-id="76498-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76498-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="76498-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76498-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="76498-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76498-117">Request headers</span></span>
| <span data-ttu-id="76498-118">名前</span><span class="sxs-lookup"><span data-stu-id="76498-118">Name</span></span>       | <span data-ttu-id="76498-119">説明</span><span class="sxs-lookup"><span data-stu-id="76498-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="76498-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="76498-120">Authorization</span></span>  | <span data-ttu-id="76498-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="76498-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="76498-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="76498-122">Request body</span></span>
<span data-ttu-id="76498-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="76498-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="76498-124">応答</span><span class="sxs-lookup"><span data-stu-id="76498-124">Response</span></span>
<span data-ttu-id="76498-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="76498-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76498-127">例</span><span class="sxs-lookup"><span data-stu-id="76498-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76498-128">要求</span><span class="sxs-lookup"><span data-stu-id="76498-128">Request</span></span>
<span data-ttu-id="76498-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76498-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76498-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="76498-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76498-131">C#</span><span class="sxs-lookup"><span data-stu-id="76498-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76498-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="76498-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76498-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="76498-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="76498-134">Java</span><span class="sxs-lookup"><span data-stu-id="76498-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="76498-135">応答</span><span class="sxs-lookup"><span data-stu-id="76498-135">Response</span></span>
<span data-ttu-id="76498-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76498-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
