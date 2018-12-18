---
title: 'ドメイン: forceDelete'
description: 非同期操作を使用してドメインを削除します。
author: lleonard-msft
ms.openlocfilehash: 4af5b70fca7600538d4212768243d8de82eb79ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316213"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="f3634-103">ドメイン: forceDelete</span><span class="sxs-lookup"><span data-stu-id="f3634-103">domain: forceDelete</span></span>

> <span data-ttu-id="f3634-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3634-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3634-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3634-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3634-106">非同期操作を使用してドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="f3634-106">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="f3634-107">次の操作は、この操作の一部として実行されます。</span><span class="sxs-lookup"><span data-stu-id="f3634-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="f3634-108">UPN、EmailAddress、および削除されたドメインへの参照を持つユーザーのメタベースを変更します。</span><span class="sxs-lookup"><span data-stu-id="f3634-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="f3634-109">削除したドメインへの参照を持つグループの電子メール アドレスの名前を変更します。</span><span class="sxs-lookup"><span data-stu-id="f3634-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="f3634-110">削除したドメインへの参照を持つアプリケーションの identifierUris の名前を変更します。</span><span class="sxs-lookup"><span data-stu-id="f3634-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="f3634-111">名前を変更するオブジェクトの数が 1000 を超える場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="f3634-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="f3634-112">マルチ テナント アプリケーションの名前を変更するアプリケーションのいずれかの場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="f3634-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="f3634-113">ドメインの削除が完了すると、API の操作、削除されたドメインの HTTP 応答コード 404 が返されます。</span><span class="sxs-lookup"><span data-stu-id="f3634-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="f3634-114">ドメインの削除を確認するには、[ドメインを取得](domain-get.md)を実行できます。</span><span class="sxs-lookup"><span data-stu-id="f3634-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="f3634-115">ドメインが正常に削除された場合の応答で 404 の HTTP 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="f3634-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3634-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3634-116">Permissions</span></span>

<span data-ttu-id="f3634-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3634-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f3634-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3634-119">Permission type</span></span>      | <span data-ttu-id="f3634-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3634-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3634-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3634-121">Delegated (work or school account)</span></span> | <span data-ttu-id="f3634-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f3634-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f3634-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3634-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3634-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3634-124">Not supported.</span></span>    |
|<span data-ttu-id="f3634-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3634-125">Application</span></span> | <span data-ttu-id="f3634-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3634-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3634-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3634-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="f3634-128">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="f3634-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3634-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3634-129">Request headers</span></span>

| <span data-ttu-id="f3634-130">名前</span><span class="sxs-lookup"><span data-stu-id="f3634-130">Name</span></span>       | <span data-ttu-id="f3634-131">説明</span><span class="sxs-lookup"><span data-stu-id="f3634-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3634-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3634-132">Authorization</span></span>  | <span data-ttu-id="f3634-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3634-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f3634-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f3634-135">Content-Type</span></span>  | <span data-ttu-id="f3634-136">application/json</span><span class="sxs-lookup"><span data-stu-id="f3634-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3634-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3634-137">Request body</span></span>

<span data-ttu-id="f3634-138">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3634-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f3634-139">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f3634-139">Parameter</span></span>    | <span data-ttu-id="f3634-140">種類</span><span class="sxs-lookup"><span data-stu-id="f3634-140">Type</span></span>   |<span data-ttu-id="f3634-141">説明</span><span class="sxs-lookup"><span data-stu-id="f3634-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3634-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="f3634-142">disableUserAccounts</span></span>|<span data-ttu-id="f3634-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="f3634-143">Boolean</span></span>| <span data-ttu-id="f3634-144">名前を変更したユーザー アカウントを無効にするオプションです。</span><span class="sxs-lookup"><span data-stu-id="f3634-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="f3634-145">ユーザー アカウントを無効にすると、ユーザーはサインインするのには使用できません。</span><span class="sxs-lookup"><span data-stu-id="f3634-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="f3634-146">*場合は true。*(デフォルト) - ユーザーがこの操作の一部として名前が変更されたアカウントが無効になります。</span><span class="sxs-lookup"><span data-stu-id="f3634-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="f3634-147">*False* - この操作の一部として名前を変更するユーザー アカウントは無効になっていません。</span><span class="sxs-lookup"><span data-stu-id="f3634-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="f3634-148">応答</span><span class="sxs-lookup"><span data-stu-id="f3634-148">Response</span></span>

<span data-ttu-id="f3634-149">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f3634-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="f3634-150">例</span><span class="sxs-lookup"><span data-stu-id="f3634-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3634-151">要求</span><span class="sxs-lookup"><span data-stu-id="f3634-151">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

##### <a name="response"></a><span data-ttu-id="f3634-152">応答</span><span class="sxs-lookup"><span data-stu-id="f3634-152">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
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