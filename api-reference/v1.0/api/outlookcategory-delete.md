---
title: Outlook カテゴリを削除する
description: 指定した outlookCategory オブジェクトを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: bdc0bbb2cc27a5ad8fcb4ed14bca48d72d2b155b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448327"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="e4d72-103">Outlook カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="e4d72-103">Delete Outlook category</span></span>


<span data-ttu-id="e4d72-104">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e4d72-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4d72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e4d72-105">Permissions</span></span>
<span data-ttu-id="e4d72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4d72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4d72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e4d72-108">Permission type</span></span>      | <span data-ttu-id="e4d72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e4d72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4d72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e4d72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4d72-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d72-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e4d72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e4d72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4d72-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d72-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e4d72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4d72-114">Application</span></span> | <span data-ttu-id="e4d72-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d72-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4d72-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e4d72-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e4d72-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4d72-117">Request headers</span></span>
| <span data-ttu-id="e4d72-118">名前</span><span class="sxs-lookup"><span data-stu-id="e4d72-118">Name</span></span>      |<span data-ttu-id="e4d72-119">説明</span><span class="sxs-lookup"><span data-stu-id="e4d72-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4d72-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4d72-120">Authorization</span></span>  | <span data-ttu-id="e4d72-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e4d72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4d72-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e4d72-123">Request body</span></span>
<span data-ttu-id="e4d72-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e4d72-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4d72-125">応答</span><span class="sxs-lookup"><span data-stu-id="e4d72-125">Response</span></span>

<span data-ttu-id="e4d72-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e4d72-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4d72-128">例</span><span class="sxs-lookup"><span data-stu-id="e4d72-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4d72-129">要求</span><span class="sxs-lookup"><span data-stu-id="e4d72-129">Request</span></span>
<span data-ttu-id="e4d72-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e4d72-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e4d72-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e4d72-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e4d72-132">C#</span><span class="sxs-lookup"><span data-stu-id="e4d72-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4d72-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="e4d72-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e4d72-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="e4d72-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e4d72-135">応答</span><span class="sxs-lookup"><span data-stu-id="e4d72-135">Response</span></span>
<span data-ttu-id="e4d72-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e4d72-136">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
