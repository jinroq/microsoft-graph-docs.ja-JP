---
title: ドメインを削除する
description: テナントからドメインを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9175523580b10c6a22ac73cf88a3bc87692909f1
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655797"
---
# <a name="delete-domain"></a><span data-ttu-id="ef346-103">ドメインを削除する</span><span class="sxs-lookup"><span data-stu-id="ef346-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef346-104">テナントからドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="ef346-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="ef346-105">**重要:** 削除されたドメインは復元できません。</span><span class="sxs-lookup"><span data-stu-id="ef346-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef346-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ef346-106">Permissions</span></span>

<span data-ttu-id="ef346-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ef346-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef346-109">Permission type</span></span>      | <span data-ttu-id="ef346-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef346-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef346-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ef346-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ef346-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef346-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ef346-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef346-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef346-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef346-114">Not supported.</span></span>    |
|<span data-ttu-id="ef346-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef346-115">Application</span></span> | <span data-ttu-id="ef346-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef346-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef346-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef346-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="ef346-118">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="ef346-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef346-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef346-119">Request headers</span></span>

| <span data-ttu-id="ef346-120">名前</span><span class="sxs-lookup"><span data-stu-id="ef346-120">Name</span></span>       | <span data-ttu-id="ef346-121">説明</span><span class="sxs-lookup"><span data-stu-id="ef346-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ef346-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef346-122">Authorization</span></span>  | <span data-ttu-id="ef346-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ef346-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef346-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef346-125">Content-Type</span></span>  | <span data-ttu-id="ef346-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef346-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef346-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ef346-127">Request body</span></span>

<span data-ttu-id="ef346-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ef346-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef346-129">応答</span><span class="sxs-lookup"><span data-stu-id="ef346-129">Response</span></span>

<span data-ttu-id="ef346-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文は返されません。</span><span class="sxs-lookup"><span data-stu-id="ef346-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef346-132">例</span><span class="sxs-lookup"><span data-stu-id="ef346-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef346-133">要求</span><span class="sxs-lookup"><span data-stu-id="ef346-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="ef346-134">応答</span><span class="sxs-lookup"><span data-stu-id="ef346-134">Response</span></span>

<span data-ttu-id="ef346-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ef346-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ef346-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ef346-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ef346-138">C#</span><span class="sxs-lookup"><span data-stu-id="ef346-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef346-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef346-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
