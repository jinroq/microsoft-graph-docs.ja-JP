---
title: 'ドメイン: forcedelete'
description: 非同期操作を使用してドメインを削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a1a2b2510f0c79f2be4e70deb9efabc65f8dfc4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454933"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="5ecdd-103">ドメイン: forcedelete</span><span class="sxs-lookup"><span data-stu-id="5ecdd-103">domain: forceDelete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ecdd-104">非同期操作を使用してドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-104">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="5ecdd-105">この操作の一部として、次のアクションが実行されます。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="5ecdd-106">UPN、EmailAddress、および ProxyAddress のユーザーの名前を、削除されたドメインへの参照に変更します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-106">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="5ecdd-107">削除されたドメインへの参照を使用して、グループの EmailAddress の名前を変更します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-107">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="5ecdd-108">アプリケーションの identifieruris の名前を、削除されたドメインへの参照に変更します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-108">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="5ecdd-109">名前を変更するオブジェクトの数が1000より大きい場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="5ecdd-110">名前を変更するアプリケーションのいずれかがマルチテナントアプリの場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-110">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="5ecdd-111">ドメイン削除の完了後、削除されたドメインの API 操作は 404 HTTP 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-111">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="5ecdd-112">ドメインの削除を確認するには、 [get ドメイン](domain-get.md)を実行します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="5ecdd-113">ドメインが正常に削除された場合は、応答で 404 HTTP 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-113">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ecdd-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ecdd-114">Permissions</span></span>

<span data-ttu-id="5ecdd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5ecdd-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ecdd-117">Permission type</span></span>      | <span data-ttu-id="5ecdd-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ecdd-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ecdd-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ecdd-119">Delegated (work or school account)</span></span> | <span data-ttu-id="5ecdd-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ecdd-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ecdd-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ecdd-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ecdd-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-122">Not supported.</span></span>    |
|<span data-ttu-id="5ecdd-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ecdd-123">Application</span></span> | <span data-ttu-id="5ecdd-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ecdd-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ecdd-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ecdd-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="5ecdd-126">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ecdd-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ecdd-127">Request headers</span></span>

| <span data-ttu-id="5ecdd-128">名前</span><span class="sxs-lookup"><span data-stu-id="5ecdd-128">Name</span></span>       | <span data-ttu-id="5ecdd-129">説明</span><span class="sxs-lookup"><span data-stu-id="5ecdd-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ecdd-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ecdd-130">Authorization</span></span>  | <span data-ttu-id="5ecdd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5ecdd-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ecdd-133">Content-Type</span></span>  | <span data-ttu-id="5ecdd-134">application/json</span><span class="sxs-lookup"><span data-stu-id="5ecdd-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ecdd-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ecdd-135">Request body</span></span>

<span data-ttu-id="5ecdd-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5ecdd-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ecdd-137">Parameter</span></span>    | <span data-ttu-id="5ecdd-138">型</span><span class="sxs-lookup"><span data-stu-id="5ecdd-138">Type</span></span>   |<span data-ttu-id="5ecdd-139">説明</span><span class="sxs-lookup"><span data-stu-id="5ecdd-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ecdd-140">disableuseraccounts</span><span class="sxs-lookup"><span data-stu-id="5ecdd-140">disableUserAccounts</span></span>|<span data-ttu-id="5ecdd-141">ブール型</span><span class="sxs-lookup"><span data-stu-id="5ecdd-141">Boolean</span></span>| <span data-ttu-id="5ecdd-142">名前の変更されたユーザーアカウントを無効にするオプション。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-142">Option to disable renamed user accounts.</span></span> <span data-ttu-id="5ecdd-143">ユーザーアカウントが無効になっている場合、ユーザーはサインインすることができません。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-143">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="5ecdd-144">*True*(既定値)-この操作の一部として名前が変更されたユーザーアカウントは無効になります。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-144">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="5ecdd-145">*False* -この操作の一部として名前が変更されたユーザーアカウントは無効になりません。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-145">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="5ecdd-146">応答</span><span class="sxs-lookup"><span data-stu-id="5ecdd-146">Response</span></span>

<span data-ttu-id="5ecdd-147">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5ecdd-147">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="5ecdd-148">例</span><span class="sxs-lookup"><span data-stu-id="5ecdd-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ecdd-149">要求</span><span class="sxs-lookup"><span data-stu-id="5ecdd-149">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="5ecdd-150">応答</span><span class="sxs-lookup"><span data-stu-id="5ecdd-150">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
