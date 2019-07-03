---
title: identityProvider を削除する
description: 既存の identityProvider を削除します。
localization_priority: Normal
ms.openlocfilehash: 74acf6b790ca9039944bc2d9bc687b74fced1d1b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442581"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="67bc0-103">identityProvider を削除する</span><span class="sxs-lookup"><span data-stu-id="67bc0-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67bc0-104">既存の [identityProvider](../resources/identityprovider.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="67bc0-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="67bc0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67bc0-105">Permissions</span></span>

<span data-ttu-id="67bc0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67bc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67bc0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67bc0-108">Permission type</span></span>      | <span data-ttu-id="67bc0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67bc0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67bc0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67bc0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="67bc0-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67bc0-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="67bc0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67bc0-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="67bc0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67bc0-113">Not supported.</span></span>|
|<span data-ttu-id="67bc0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67bc0-114">Application</span></span>|<span data-ttu-id="67bc0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67bc0-115">Not supported.</span></span>|

<span data-ttu-id="67bc0-116">職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。</span><span class="sxs-lookup"><span data-stu-id="67bc0-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="67bc0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67bc0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="67bc0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67bc0-118">Request headers</span></span>

|<span data-ttu-id="67bc0-119">名前</span><span class="sxs-lookup"><span data-stu-id="67bc0-119">Name</span></span>|<span data-ttu-id="67bc0-120">説明</span><span class="sxs-lookup"><span data-stu-id="67bc0-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="67bc0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67bc0-121">Authorization</span></span>|<span data-ttu-id="67bc0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="67bc0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67bc0-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="67bc0-124">Request body</span></span>

<span data-ttu-id="67bc0-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="67bc0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67bc0-126">応答</span><span class="sxs-lookup"><span data-stu-id="67bc0-126">Response</span></span>

<span data-ttu-id="67bc0-127">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="67bc0-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="67bc0-128">例</span><span class="sxs-lookup"><span data-stu-id="67bc0-128">Example</span></span>

<span data-ttu-id="67bc0-129">次の例では、**identityProvider** を削除します。</span><span class="sxs-lookup"><span data-stu-id="67bc0-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="67bc0-130">要求</span><span class="sxs-lookup"><span data-stu-id="67bc0-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="67bc0-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="67bc0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67bc0-132">C#</span><span class="sxs-lookup"><span data-stu-id="67bc0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67bc0-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="67bc0-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67bc0-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="67bc0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="67bc0-135">応答</span><span class="sxs-lookup"><span data-stu-id="67bc0-135">Response</span></span>

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
