---
title: ドメインを削除する
description: テナントからドメインを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: efef594979cecc17f740d6be683ad08f091bdf71
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889978"
---
# <a name="delete-domain"></a><span data-ttu-id="cabf8-103">ドメインを削除する</span><span class="sxs-lookup"><span data-stu-id="cabf8-103">Delete domain</span></span>

<span data-ttu-id="cabf8-104">テナントからドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="cabf8-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="cabf8-105">**重要:**</span><span class="sxs-lookup"><span data-stu-id="cabf8-105">**Important:**</span></span>
> - <span data-ttu-id="cabf8-106">削除されたドメインは回復できません。</span><span class="sxs-lookup"><span data-stu-id="cabf8-106">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="cabf8-p101">ドメインにまだ依存しているリソースまたはオブジェクトがある場合、削除の試行は失敗します。[List domainNameReferences](domain-list-domainnamereferences.md) API を使用して、すべての依存リソースを探すことができます。</span><span class="sxs-lookup"><span data-stu-id="cabf8-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="cabf8-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cabf8-109">Permissions</span></span>

<span data-ttu-id="cabf8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cabf8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cabf8-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cabf8-112">Permission type</span></span>      | <span data-ttu-id="cabf8-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cabf8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cabf8-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cabf8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cabf8-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cabf8-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cabf8-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cabf8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cabf8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cabf8-117">Not supported.</span></span>    |
|<span data-ttu-id="cabf8-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cabf8-118">Application</span></span> | <span data-ttu-id="cabf8-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cabf8-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cabf8-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cabf8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="cabf8-121">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="cabf8-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cabf8-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cabf8-122">Request headers</span></span>

| <span data-ttu-id="cabf8-123">名前</span><span class="sxs-lookup"><span data-stu-id="cabf8-123">Name</span></span>       | <span data-ttu-id="cabf8-124">説明</span><span class="sxs-lookup"><span data-stu-id="cabf8-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cabf8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cabf8-125">Authorization</span></span>  | <span data-ttu-id="cabf8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cabf8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cabf8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cabf8-128">Content-Type</span></span>  | <span data-ttu-id="cabf8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="cabf8-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cabf8-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="cabf8-130">Request body</span></span>

<span data-ttu-id="cabf8-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cabf8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cabf8-132">応答</span><span class="sxs-lookup"><span data-stu-id="cabf8-132">Response</span></span>

<span data-ttu-id="cabf8-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文は返されません。</span><span class="sxs-lookup"><span data-stu-id="cabf8-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="cabf8-135">例</span><span class="sxs-lookup"><span data-stu-id="cabf8-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cabf8-136">要求</span><span class="sxs-lookup"><span data-stu-id="cabf8-136">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cabf8-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cabf8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cabf8-138">C#</span><span class="sxs-lookup"><span data-stu-id="cabf8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cabf8-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="cabf8-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cabf8-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="cabf8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cabf8-141">Java</span><span class="sxs-lookup"><span data-stu-id="cabf8-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cabf8-142">応答</span><span class="sxs-lookup"><span data-stu-id="cabf8-142">Response</span></span>

<span data-ttu-id="cabf8-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cabf8-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
