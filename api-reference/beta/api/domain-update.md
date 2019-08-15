---
title: ドメインを更新する
description: Domain オブジェクトのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8cfc6e0215c4d4a1a4ffc5f74246423cd2f4edf0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417001"
---
# <a name="update-domain"></a><span data-ttu-id="93009-103">ドメインを更新する</span><span class="sxs-lookup"><span data-stu-id="93009-103">Update domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93009-104">Domain オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="93009-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="93009-105">**重要:** 確認済みのドメインのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="93009-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="93009-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="93009-106">Permissions</span></span>

<span data-ttu-id="93009-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="93009-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93009-109">Permission type</span></span>      | <span data-ttu-id="93009-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="93009-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93009-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93009-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93009-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93009-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93009-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93009-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93009-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93009-114">Not supported.</span></span>    |
|<span data-ttu-id="93009-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93009-115">Application</span></span> | <span data-ttu-id="93009-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93009-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93009-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93009-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="93009-118">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="93009-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93009-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93009-119">Request headers</span></span>

| <span data-ttu-id="93009-120">名前</span><span class="sxs-lookup"><span data-stu-id="93009-120">Name</span></span>       | <span data-ttu-id="93009-121">説明</span><span class="sxs-lookup"><span data-stu-id="93009-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="93009-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93009-122">Authorization</span></span>  | <span data-ttu-id="93009-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="93009-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93009-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93009-125">Content-Type</span></span>  | <span data-ttu-id="93009-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93009-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="93009-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="93009-127">Request body</span></span>

<span data-ttu-id="93009-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="93009-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="93009-129">要求本文に含まれていない既存のプロパティは、以前の値を維持するか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="93009-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="93009-130">最適なパフォーマンスを得るために、変更された値のみを含めます。</span><span class="sxs-lookup"><span data-stu-id="93009-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="93009-131">応答</span><span class="sxs-lookup"><span data-stu-id="93009-131">Response</span></span>

<span data-ttu-id="93009-132">成功した場合、このメソッド`204 No Content`は応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="93009-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="93009-133">例</span><span class="sxs-lookup"><span data-stu-id="93009-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93009-134">要求</span><span class="sxs-lookup"><span data-stu-id="93009-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93009-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="93009-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93009-136">C#</span><span class="sxs-lookup"><span data-stu-id="93009-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93009-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93009-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93009-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="93009-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="93009-139">応答</span><span class="sxs-lookup"><span data-stu-id="93009-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
