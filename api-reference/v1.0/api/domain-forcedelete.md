---
title: 強制的にドメインを削除する
description: 非同期の長時間実行操作を使用してドメインを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 69d95d4189f5660315365420703d3ebb954b9dda
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656651"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="f8d18-103">強制的にドメインを削除する</span><span class="sxs-lookup"><span data-stu-id="f8d18-103">Force domain deletion</span></span>

<span data-ttu-id="f8d18-104">非同期の長時間実行操作を使用してドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="f8d18-105">この操作の一部として、次のアクションが実行されます。</span><span class="sxs-lookup"><span data-stu-id="f8d18-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="f8d18-106">最初の`userPrincipalName`onmicrosoft.com `mail`ドメインを`proxyAddresses`使用する`users`ために、削除されたドメインへの参照で、、、およびのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="f8d18-107">の`mail` `groups`プロパティを、削除されたドメインへの参照で更新して、最初の onmicrosoft.com ドメインを使用します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="f8d18-108">の`identifierUris` `applications`プロパティを、削除されたドメインへの参照で更新して、最初の onmicrosoft.com ドメインを使用します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="f8d18-109">名前を変更するオブジェクトの数が1000より大きい場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="f8d18-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="f8d18-110">名前`applications`を変更する1つのがマルチテナントアプリの場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="f8d18-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="f8d18-111">ドメイン削除の完了後、削除されたドメインの API 操作は HTTP 404 状態コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="f8d18-112">ドメインの削除を確認するには、ドメインの[取得](domain-get.md)操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8d18-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f8d18-113">Permissions</span></span>

<span data-ttu-id="f8d18-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8d18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8d18-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8d18-116">Permission type</span></span>      | <span data-ttu-id="f8d18-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8d18-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8d18-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8d18-118">Delegated (work or school account)</span></span> | <span data-ttu-id="f8d18-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8d18-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8d18-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8d18-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8d18-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8d18-121">Not supported.</span></span>    |
|<span data-ttu-id="f8d18-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8d18-122">Application</span></span> | <span data-ttu-id="f8d18-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8d18-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8d18-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8d18-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="f8d18-125">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8d18-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8d18-126">Request headers</span></span>

| <span data-ttu-id="f8d18-127">名前</span><span class="sxs-lookup"><span data-stu-id="f8d18-127">Name</span></span> | <span data-ttu-id="f8d18-128">説明</span><span class="sxs-lookup"><span data-stu-id="f8d18-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f8d18-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8d18-129">Authorization</span></span>  | <span data-ttu-id="f8d18-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f8d18-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f8d18-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8d18-132">Content-Type</span></span>  | <span data-ttu-id="f8d18-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f8d18-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8d18-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8d18-134">Request body</span></span>

<span data-ttu-id="f8d18-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8d18-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f8d18-136">Parameter</span></span> | <span data-ttu-id="f8d18-137">型</span><span class="sxs-lookup"><span data-stu-id="f8d18-137">Type</span></span> | <span data-ttu-id="f8d18-138">説明</span><span class="sxs-lookup"><span data-stu-id="f8d18-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="f8d18-139">名前が変更されたユーザーアカウントを無効にするオプション。</span><span class="sxs-lookup"><span data-stu-id="f8d18-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="f8d18-140">ユーザーアカウントが無効になっている場合、ユーザーはサインインすることができません。</span><span class="sxs-lookup"><span data-stu-id="f8d18-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="f8d18-141">**True**に設定すると`users` 、この操作の一部として更新されたものは無効になります。</span><span class="sxs-lookup"><span data-stu-id="f8d18-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="f8d18-142">既定値は **true** です。</span><span class="sxs-lookup"><span data-stu-id="f8d18-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="f8d18-143">応答本文</span><span class="sxs-lookup"><span data-stu-id="f8d18-143">Response body</span></span>

<span data-ttu-id="f8d18-144">成功した場合、この`HTTP/1.1 204 OK`メソッドは状態コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f8d18-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="f8d18-145">例</span><span class="sxs-lookup"><span data-stu-id="f8d18-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8d18-146">要求</span><span class="sxs-lookup"><span data-stu-id="f8d18-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a><span data-ttu-id="f8d18-147">応答</span><span class="sxs-lookup"><span data-stu-id="f8d18-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8d18-148">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f8d18-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8d18-149">C#</span><span class="sxs-lookup"><span data-stu-id="f8d18-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8d18-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8d18-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
