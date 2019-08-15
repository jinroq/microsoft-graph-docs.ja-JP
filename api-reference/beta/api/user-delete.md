---
title: ユーザーを削除する - Microsoft Graph API
description: Microsoft Graph API (REST) のユーザー リソース (エンティティ) の削除方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ef3d3de7b5c5ade167446b9943859608bacee25
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409071"
---
# <a name="delete-a-user"></a><span data-ttu-id="356c8-103">ユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="356c8-103">Delete a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="356c8-104">ユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="356c8-104">Delete user.</span></span>  

<span data-ttu-id="356c8-105">ユーザー リソースを削除すると、一時的なコンテナーに移動され、30 日以内であれば復元できます。</span><span class="sxs-lookup"><span data-stu-id="356c8-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="356c8-106">それ以降、これらのユーザーは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="356c8-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="356c8-107">詳細については、「[deletedItems](../resources/directory.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="356c8-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="356c8-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="356c8-108">Permissions</span></span>

<span data-ttu-id="356c8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="356c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="356c8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="356c8-111">Permission type</span></span>      | <span data-ttu-id="356c8-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="356c8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="356c8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="356c8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="356c8-114">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="356c8-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="356c8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="356c8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="356c8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="356c8-116">Not supported.</span></span>    |
|<span data-ttu-id="356c8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="356c8-117">Application</span></span> | <span data-ttu-id="356c8-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356c8-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="356c8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="356c8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="356c8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="356c8-120">Request headers</span></span>

| <span data-ttu-id="356c8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="356c8-121">Header</span></span>       | <span data-ttu-id="356c8-122">値</span><span class="sxs-lookup"><span data-stu-id="356c8-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="356c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="356c8-123">Authorization</span></span>  | <span data-ttu-id="356c8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="356c8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="356c8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="356c8-126">Request body</span></span>

<span data-ttu-id="356c8-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="356c8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="356c8-128">応答</span><span class="sxs-lookup"><span data-stu-id="356c8-128">Response</span></span>

<span data-ttu-id="356c8-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="356c8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="356c8-131">例</span><span class="sxs-lookup"><span data-stu-id="356c8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="356c8-132">要求</span><span class="sxs-lookup"><span data-stu-id="356c8-132">Request</span></span>

<span data-ttu-id="356c8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="356c8-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="356c8-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="356c8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="356c8-135">C#</span><span class="sxs-lookup"><span data-stu-id="356c8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="356c8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="356c8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="356c8-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="356c8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="356c8-138">応答</span><span class="sxs-lookup"><span data-stu-id="356c8-138">Response</span></span>

<span data-ttu-id="356c8-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="356c8-139">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
