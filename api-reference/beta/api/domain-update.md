---
title: ドメインを更新する
description: Domain オブジェクトのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 05819b5e0a33fdf92072f64442c5ceb30a30b085
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260397"
---
# <a name="update-domain"></a><span data-ttu-id="9852c-103">ドメインを更新する</span><span class="sxs-lookup"><span data-stu-id="9852c-103">Update domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9852c-104">Domain オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9852c-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="9852c-105">**重要:** 確認済みのドメインのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="9852c-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="9852c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9852c-106">Permissions</span></span>

<span data-ttu-id="9852c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9852c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9852c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9852c-109">Permission type</span></span>      | <span data-ttu-id="9852c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9852c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9852c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9852c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9852c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9852c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9852c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9852c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9852c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9852c-114">Not supported.</span></span>    |
|<span data-ttu-id="9852c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9852c-115">Application</span></span> | <span data-ttu-id="9852c-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9852c-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9852c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9852c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="9852c-118">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="9852c-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9852c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9852c-119">Request headers</span></span>

| <span data-ttu-id="9852c-120">名前</span><span class="sxs-lookup"><span data-stu-id="9852c-120">Name</span></span>       | <span data-ttu-id="9852c-121">説明</span><span class="sxs-lookup"><span data-stu-id="9852c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9852c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9852c-122">Authorization</span></span>  | <span data-ttu-id="9852c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9852c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9852c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9852c-125">Content-Type</span></span>  | <span data-ttu-id="9852c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9852c-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9852c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9852c-127">Request body</span></span>

<span data-ttu-id="9852c-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9852c-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="9852c-129">要求本文に含まれていない既存のプロパティは、以前の値を維持するか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="9852c-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9852c-130">最適なパフォーマンスを得るために、変更された値のみを含めます。</span><span class="sxs-lookup"><span data-stu-id="9852c-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="9852c-131">応答</span><span class="sxs-lookup"><span data-stu-id="9852c-131">Response</span></span>

<span data-ttu-id="9852c-132">成功した場合、このメソッド`204 No Content`は応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="9852c-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="9852c-133">例</span><span class="sxs-lookup"><span data-stu-id="9852c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9852c-134">要求</span><span class="sxs-lookup"><span data-stu-id="9852c-134">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="9852c-135">応答</span><span class="sxs-lookup"><span data-stu-id="9852c-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9852c-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9852c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9852c-137">C#</span><span class="sxs-lookup"><span data-stu-id="9852c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9852c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="9852c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_domain-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9852c-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="9852c-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_domain-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
