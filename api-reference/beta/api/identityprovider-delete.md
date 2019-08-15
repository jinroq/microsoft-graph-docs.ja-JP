---
title: identityProvider を削除する
description: 既存の identityProvider を削除します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: cceaea97f613c33ea2a104a7cf0b4d09077949e6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420558"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="088de-103">identityProvider を削除する</span><span class="sxs-lookup"><span data-stu-id="088de-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="088de-104">既存の [identityProvider](../resources/identityprovider.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="088de-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="088de-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="088de-105">Permissions</span></span>

<span data-ttu-id="088de-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="088de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="088de-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="088de-108">Permission type</span></span>      | <span data-ttu-id="088de-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="088de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="088de-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="088de-110">Delegated (work or school account)</span></span>|<span data-ttu-id="088de-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="088de-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="088de-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="088de-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="088de-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="088de-113">Not supported.</span></span>|
|<span data-ttu-id="088de-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="088de-114">Application</span></span>|<span data-ttu-id="088de-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="088de-115">Not supported.</span></span>|

<span data-ttu-id="088de-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="088de-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="088de-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="088de-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="088de-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="088de-118">Request headers</span></span>

|<span data-ttu-id="088de-119">名前</span><span class="sxs-lookup"><span data-stu-id="088de-119">Name</span></span>|<span data-ttu-id="088de-120">説明</span><span class="sxs-lookup"><span data-stu-id="088de-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="088de-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="088de-121">Authorization</span></span>|<span data-ttu-id="088de-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="088de-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="088de-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="088de-124">Request body</span></span>

<span data-ttu-id="088de-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="088de-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="088de-126">応答</span><span class="sxs-lookup"><span data-stu-id="088de-126">Response</span></span>

<span data-ttu-id="088de-127">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="088de-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="088de-128">例</span><span class="sxs-lookup"><span data-stu-id="088de-128">Example</span></span>

<span data-ttu-id="088de-129">次の例では、**identityProvider** を削除します。</span><span class="sxs-lookup"><span data-stu-id="088de-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="088de-130">要求</span><span class="sxs-lookup"><span data-stu-id="088de-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="088de-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="088de-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="088de-132">C#</span><span class="sxs-lookup"><span data-stu-id="088de-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="088de-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="088de-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="088de-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="088de-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="088de-135">応答</span><span class="sxs-lookup"><span data-stu-id="088de-135">Response</span></span>

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
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
