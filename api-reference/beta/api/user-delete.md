---
title: ユーザーを削除する - Microsoft Graph API
description: Microsoft Graph API (REST) のユーザー リソース (エンティティ) の削除方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f96bbdce7773fa7401e087d4962f1272926496f3
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637403"
---
# <a name="delete-a-user"></a><span data-ttu-id="9b99b-103">ユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="9b99b-103">Delete a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b99b-104">ユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="9b99b-104">Delete user.</span></span>  

<span data-ttu-id="9b99b-105">ユーザー リソースを削除すると、一時的なコンテナーに移動され、30 日以内であれば復元できます。</span><span class="sxs-lookup"><span data-stu-id="9b99b-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="9b99b-106">それ以降、これらのユーザーは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="9b99b-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="9b99b-107">詳細については、「[deletedItems](../resources/directory.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b99b-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b99b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9b99b-108">Permissions</span></span>

<span data-ttu-id="9b99b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b99b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b99b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b99b-111">Permission type</span></span>      | <span data-ttu-id="9b99b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b99b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b99b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b99b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9b99b-114">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9b99b-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9b99b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b99b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b99b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b99b-116">Not supported.</span></span>    |
|<span data-ttu-id="9b99b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b99b-117">Application</span></span> | <span data-ttu-id="9b99b-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b99b-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b99b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b99b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="9b99b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b99b-120">Request headers</span></span>

| <span data-ttu-id="9b99b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b99b-121">Header</span></span>       | <span data-ttu-id="9b99b-122">値</span><span class="sxs-lookup"><span data-stu-id="9b99b-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9b99b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b99b-123">Authorization</span></span>  | <span data-ttu-id="9b99b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9b99b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b99b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b99b-126">Request body</span></span>

<span data-ttu-id="9b99b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9b99b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b99b-128">応答</span><span class="sxs-lookup"><span data-stu-id="9b99b-128">Response</span></span>

<span data-ttu-id="9b99b-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9b99b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b99b-131">例</span><span class="sxs-lookup"><span data-stu-id="9b99b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b99b-132">要求</span><span class="sxs-lookup"><span data-stu-id="9b99b-132">Request</span></span>

<span data-ttu-id="9b99b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b99b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
### <a name="response"></a><span data-ttu-id="9b99b-134">応答</span><span class="sxs-lookup"><span data-stu-id="9b99b-134">Response</span></span>

<span data-ttu-id="9b99b-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9b99b-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9b99b-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="9b99b-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9b99b-137">Visual</span><span class="sxs-lookup"><span data-stu-id="9b99b-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b99b-138">Java</span><span class="sxs-lookup"><span data-stu-id="9b99b-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
