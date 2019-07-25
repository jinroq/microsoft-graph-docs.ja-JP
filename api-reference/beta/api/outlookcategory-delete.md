---
title: Outlook カテゴリを削除する
description: 指定した outlookCategory オブジェクトを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7c9a58dc1c970d68ec2956854388b0ab5b9814a7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877811"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="891e5-103">Outlook カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="891e5-103">Delete Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="891e5-104">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="891e5-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="891e5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="891e5-105">Permissions</span></span>
<span data-ttu-id="891e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="891e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="891e5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="891e5-108">Permission type</span></span>      | <span data-ttu-id="891e5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="891e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="891e5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="891e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="891e5-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="891e5-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="891e5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="891e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="891e5-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="891e5-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="891e5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="891e5-114">Application</span></span> | <span data-ttu-id="891e5-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="891e5-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="891e5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="891e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="891e5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="891e5-117">Request headers</span></span>
| <span data-ttu-id="891e5-118">名前</span><span class="sxs-lookup"><span data-stu-id="891e5-118">Name</span></span>      |<span data-ttu-id="891e5-119">説明</span><span class="sxs-lookup"><span data-stu-id="891e5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="891e5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="891e5-120">Authorization</span></span>  | <span data-ttu-id="891e5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="891e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="891e5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="891e5-123">Request body</span></span>
<span data-ttu-id="891e5-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="891e5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="891e5-125">応答</span><span class="sxs-lookup"><span data-stu-id="891e5-125">Response</span></span>

<span data-ttu-id="891e5-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="891e5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="891e5-128">例</span><span class="sxs-lookup"><span data-stu-id="891e5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="891e5-129">要求</span><span class="sxs-lookup"><span data-stu-id="891e5-129">Request</span></span>
<span data-ttu-id="891e5-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="891e5-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="891e5-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="891e5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="891e5-132">C#</span><span class="sxs-lookup"><span data-stu-id="891e5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="891e5-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="891e5-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="891e5-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="891e5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="891e5-135">Java</span><span class="sxs-lookup"><span data-stu-id="891e5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="891e5-136">応答</span><span class="sxs-lookup"><span data-stu-id="891e5-136">Response</span></span>
<span data-ttu-id="891e5-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="891e5-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
