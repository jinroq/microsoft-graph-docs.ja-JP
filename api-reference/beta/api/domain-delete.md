---
title: ドメインを削除する
description: テナントからドメインを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2bde386ffec0340a2aad66d20f4cedf0ee243e4d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957508"
---
# <a name="delete-domain"></a><span data-ttu-id="b22d6-103">ドメインを削除する</span><span class="sxs-lookup"><span data-stu-id="b22d6-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b22d6-104">テナントからドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="b22d6-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="b22d6-105">**重要:** 削除されたドメインは復元できません。</span><span class="sxs-lookup"><span data-stu-id="b22d6-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="b22d6-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b22d6-106">Permissions</span></span>

<span data-ttu-id="b22d6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b22d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b22d6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b22d6-109">Permission type</span></span>      | <span data-ttu-id="b22d6-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b22d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b22d6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b22d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b22d6-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b22d6-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b22d6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b22d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b22d6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b22d6-114">Not supported.</span></span>    |
|<span data-ttu-id="b22d6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b22d6-115">Application</span></span> | <span data-ttu-id="b22d6-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b22d6-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b22d6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b22d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="b22d6-118">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="b22d6-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b22d6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b22d6-119">Request headers</span></span>

| <span data-ttu-id="b22d6-120">名前</span><span class="sxs-lookup"><span data-stu-id="b22d6-120">Name</span></span>       | <span data-ttu-id="b22d6-121">説明</span><span class="sxs-lookup"><span data-stu-id="b22d6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b22d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b22d6-122">Authorization</span></span>  | <span data-ttu-id="b22d6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b22d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b22d6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b22d6-125">Content-Type</span></span>  | <span data-ttu-id="b22d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b22d6-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b22d6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b22d6-127">Request body</span></span>

<span data-ttu-id="b22d6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b22d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b22d6-129">応答</span><span class="sxs-lookup"><span data-stu-id="b22d6-129">Response</span></span>

<span data-ttu-id="b22d6-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文は返されません。</span><span class="sxs-lookup"><span data-stu-id="b22d6-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="b22d6-132">例</span><span class="sxs-lookup"><span data-stu-id="b22d6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b22d6-133">要求</span><span class="sxs-lookup"><span data-stu-id="b22d6-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b22d6-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b22d6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b22d6-135">C#</span><span class="sxs-lookup"><span data-stu-id="b22d6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b22d6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b22d6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b22d6-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="b22d6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b22d6-138">Java</span><span class="sxs-lookup"><span data-stu-id="b22d6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b22d6-139">応答</span><span class="sxs-lookup"><span data-stu-id="b22d6-139">Response</span></span>

<span data-ttu-id="b22d6-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b22d6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
