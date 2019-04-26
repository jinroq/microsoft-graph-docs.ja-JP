---
title: bookingStaffMember の削除
description: 指定した bookingbusiness のスタッフメンバーを削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b4a99c2970f62b08592387b75fed5dcff33e437b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322322"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="e644e-103">bookingStaffMember の削除</span><span class="sxs-lookup"><span data-stu-id="e644e-103">Delete bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e644e-104">指定した[bookingbusiness](../resources/bookingbusiness.md)の[スタッフメンバー](../resources/bookingstaffmember.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e644e-104">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e644e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e644e-105">Permissions</span></span>
<span data-ttu-id="e644e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e644e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e644e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e644e-108">Permission type</span></span>      | <span data-ttu-id="e644e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e644e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e644e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e644e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e644e-111">予約します。すべての予約</span><span class="sxs-lookup"><span data-stu-id="e644e-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e644e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e644e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e644e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e644e-113">Not supported.</span></span>   |
|<span data-ttu-id="e644e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e644e-114">Application</span></span> | <span data-ttu-id="e644e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e644e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e644e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e644e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e644e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e644e-117">Request headers</span></span>
| <span data-ttu-id="e644e-118">名前</span><span class="sxs-lookup"><span data-stu-id="e644e-118">Name</span></span>       | <span data-ttu-id="e644e-119">説明</span><span class="sxs-lookup"><span data-stu-id="e644e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e644e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e644e-120">Authorization</span></span>  | <span data-ttu-id="e644e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e644e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e644e-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="e644e-122">Request body</span></span>
<span data-ttu-id="e644e-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e644e-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e644e-124">応答</span><span class="sxs-lookup"><span data-stu-id="e644e-124">Response</span></span>
<span data-ttu-id="e644e-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e644e-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e644e-127">例</span><span class="sxs-lookup"><span data-stu-id="e644e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e644e-128">要求</span><span class="sxs-lookup"><span data-stu-id="e644e-128">Request</span></span>
<span data-ttu-id="e644e-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e644e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
##### <a name="response"></a><span data-ttu-id="e644e-130">応答</span><span class="sxs-lookup"><span data-stu-id="e644e-130">Response</span></span>
<span data-ttu-id="e644e-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e644e-131">The following is an example of the response.</span></span>
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
  "description": "Delete bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
