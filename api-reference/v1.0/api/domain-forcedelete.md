---
title: 強制的にドメインの削除
description: 非同期実行時間の長い操作を使用してドメインを削除します。
author: lleonard-msft
ms.openlocfilehash: 85839d8bf7d36925661d0202c053574288763dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309115"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="9e660-103">強制的にドメインの削除</span><span class="sxs-lookup"><span data-stu-id="9e660-103">Force domain deletion</span></span>

<span data-ttu-id="9e660-104">非同期実行時間の長い操作を使用してドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="9e660-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="9e660-105">次の操作は、この操作の一部として実行されます。</span><span class="sxs-lookup"><span data-stu-id="9e660-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="9e660-106">更新、 `userPrincipalName`、 `mail`、および`proxyAddresses`のプロパティ`users`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。</span><span class="sxs-lookup"><span data-stu-id="9e660-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="9e660-107">更新、`mail`の`groups`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。</span><span class="sxs-lookup"><span data-stu-id="9e660-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="9e660-108">更新、`identifierUris`の`applications`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。</span><span class="sxs-lookup"><span data-stu-id="9e660-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="9e660-109">名前を変更するオブジェクトの数が 1000 を超える場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="9e660-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="9e660-110">1 つの場合の`applications`は、マルチ テナント アプリケーションの名前を変更するのには、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="9e660-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="9e660-111">ドメインの削除が完了すると、削除されたドメインの API 操作は HTTP 404 ステータス コードを返します。</span><span class="sxs-lookup"><span data-stu-id="9e660-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="9e660-112">ドメインの削除を確認するには、[ドメインの取得](domain-get.md)の操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="9e660-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e660-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9e660-113">Permissions</span></span>

<span data-ttu-id="9e660-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e660-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e660-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e660-116">Permission type</span></span>      | <span data-ttu-id="9e660-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e660-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e660-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e660-118">Delegated (work or school account)</span></span> | <span data-ttu-id="9e660-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e660-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e660-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e660-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e660-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e660-121">Not supported.</span></span>    |
|<span data-ttu-id="9e660-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e660-122">Application</span></span> | <span data-ttu-id="9e660-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e660-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e660-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e660-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="9e660-125">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="9e660-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e660-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e660-126">Request headers</span></span>

| <span data-ttu-id="9e660-127">名前</span><span class="sxs-lookup"><span data-stu-id="9e660-127">Name</span></span> | <span data-ttu-id="9e660-128">説明</span><span class="sxs-lookup"><span data-stu-id="9e660-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9e660-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e660-129">Authorization</span></span>  | <span data-ttu-id="9e660-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9e660-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9e660-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e660-132">Content-Type</span></span>  | <span data-ttu-id="9e660-133">application/json</span><span class="sxs-lookup"><span data-stu-id="9e660-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e660-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e660-134">Request body</span></span>

<span data-ttu-id="9e660-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9e660-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9e660-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9e660-136">Parameter</span></span> | <span data-ttu-id="9e660-137">種類</span><span class="sxs-lookup"><span data-stu-id="9e660-137">Type</span></span> | <span data-ttu-id="9e660-138">説明</span><span class="sxs-lookup"><span data-stu-id="9e660-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="9e660-139">名前を変更するユーザー アカウントを無効にするオプションです。</span><span class="sxs-lookup"><span data-stu-id="9e660-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="9e660-140">ユーザー アカウントを無効にすると、ユーザーはサインインするのには使用できません。</span><span class="sxs-lookup"><span data-stu-id="9e660-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="9e660-141">場合**は true**に設定、`users`この操作の一部が無効にするたびに更新します。</span><span class="sxs-lookup"><span data-stu-id="9e660-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="9e660-142">既定値は**true**です。</span><span class="sxs-lookup"><span data-stu-id="9e660-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="9e660-143">応答本文</span><span class="sxs-lookup"><span data-stu-id="9e660-143">Response body</span></span>

<span data-ttu-id="9e660-144">かどうかは成功すると、このメソッドを返します`HTTP/1.1 204 OK`ステータス コードです。</span><span class="sxs-lookup"><span data-stu-id="9e660-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="9e660-145">例</span><span class="sxs-lookup"><span data-stu-id="9e660-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e660-146">要求</span><span class="sxs-lookup"><span data-stu-id="9e660-146">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="9e660-147">応答</span><span class="sxs-lookup"><span data-stu-id="9e660-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->