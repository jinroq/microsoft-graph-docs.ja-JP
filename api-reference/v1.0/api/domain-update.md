---
title: ドメインを更新する
description: Domain オブジェクトのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f1821abf0fa89d4f0b11d63d39f74fb231b7c22f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33617054"
---
# <a name="update-domain"></a><span data-ttu-id="f3fec-103">ドメインを更新する</span><span class="sxs-lookup"><span data-stu-id="f3fec-103">Update domain</span></span>

<span data-ttu-id="f3fec-104">Domain オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3fec-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="f3fec-105">**重要:** 確認済みのドメインのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="f3fec-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3fec-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3fec-106">Permissions</span></span>

<span data-ttu-id="f3fec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3fec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f3fec-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3fec-109">Permission type</span></span>      | <span data-ttu-id="f3fec-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3fec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3fec-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3fec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f3fec-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f3fec-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f3fec-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3fec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3fec-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3fec-114">Not supported.</span></span>    |
|<span data-ttu-id="f3fec-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3fec-115">Application</span></span> | <span data-ttu-id="f3fec-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fec-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3fec-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3fec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="f3fec-118">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="f3fec-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3fec-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3fec-119">Request headers</span></span>

| <span data-ttu-id="f3fec-120">名前</span><span class="sxs-lookup"><span data-stu-id="f3fec-120">Name</span></span>       | <span data-ttu-id="f3fec-121">説明</span><span class="sxs-lookup"><span data-stu-id="f3fec-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f3fec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3fec-122">Authorization</span></span>  | <span data-ttu-id="f3fec-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3fec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3fec-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f3fec-125">Content-Type</span></span>  | <span data-ttu-id="f3fec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3fec-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3fec-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3fec-127">Request body</span></span>

<span data-ttu-id="f3fec-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3fec-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="f3fec-129">要求本文に含まれていない既存のプロパティは、以前の値を維持するか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="f3fec-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f3fec-130">最適なパフォーマンスを得るために、変更された値のみを含めます。</span><span class="sxs-lookup"><span data-stu-id="f3fec-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="f3fec-131">応答</span><span class="sxs-lookup"><span data-stu-id="f3fec-131">Response</span></span>

<span data-ttu-id="f3fec-132">成功した場合、このメソッド`204 No Content`は応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="f3fec-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3fec-133">例</span><span class="sxs-lookup"><span data-stu-id="f3fec-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3fec-134">要求</span><span class="sxs-lookup"><span data-stu-id="f3fec-134">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="f3fec-135">応答</span><span class="sxs-lookup"><span data-stu-id="f3fec-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f3fec-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="f3fec-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f3fec-137">Visual</span><span class="sxs-lookup"><span data-stu-id="f3fec-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3fec-138">Java</span><span class="sxs-lookup"><span data-stu-id="f3fec-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
