---
title: BookingStaffMember の削除
description: 指定した bookingbusiness のスタッフメンバーを削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e494943dd547bdee4809b5026e26082490f7e2c1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262497"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="946b5-103">BookingStaffMember の削除</span><span class="sxs-lookup"><span data-stu-id="946b5-103">Delete bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="946b5-104">指定した[bookingbusiness](../resources/bookingbusiness.md)の[スタッフメンバー](../resources/bookingstaffmember.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="946b5-104">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="946b5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="946b5-105">Permissions</span></span>
<span data-ttu-id="946b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="946b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="946b5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="946b5-108">Permission type</span></span>      | <span data-ttu-id="946b5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="946b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="946b5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="946b5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="946b5-111">予約します。すべての予約</span><span class="sxs-lookup"><span data-stu-id="946b5-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="946b5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="946b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="946b5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="946b5-113">Not supported.</span></span>   |
|<span data-ttu-id="946b5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="946b5-114">Application</span></span> | <span data-ttu-id="946b5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="946b5-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="946b5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="946b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="946b5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="946b5-117">Request headers</span></span>
| <span data-ttu-id="946b5-118">名前</span><span class="sxs-lookup"><span data-stu-id="946b5-118">Name</span></span>       | <span data-ttu-id="946b5-119">説明</span><span class="sxs-lookup"><span data-stu-id="946b5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="946b5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="946b5-120">Authorization</span></span>  | <span data-ttu-id="946b5-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="946b5-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="946b5-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="946b5-122">Request body</span></span>
<span data-ttu-id="946b5-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="946b5-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="946b5-124">応答</span><span class="sxs-lookup"><span data-stu-id="946b5-124">Response</span></span>
<span data-ttu-id="946b5-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="946b5-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="946b5-127">例</span><span class="sxs-lookup"><span data-stu-id="946b5-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="946b5-128">要求</span><span class="sxs-lookup"><span data-stu-id="946b5-128">Request</span></span>
<span data-ttu-id="946b5-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="946b5-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
##### <a name="response"></a><span data-ttu-id="946b5-130">応答</span><span class="sxs-lookup"><span data-stu-id="946b5-130">Response</span></span>
<span data-ttu-id="946b5-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="946b5-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="946b5-132">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="946b5-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="946b5-133">C#</span><span class="sxs-lookup"><span data-stu-id="946b5-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingstaffmember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="946b5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="946b5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingstaffmember-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="946b5-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="946b5-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_bookingstaffmember-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingstaffmember-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingstaffmember-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingstaffmember-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
