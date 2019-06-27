---
title: 'domain: verify'
description: ドメインの所有権を検証します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ea935488a20505b76c8afa2e5d1eeb246b861263
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260383"
---
# <a name="domain-verify"></a><span data-ttu-id="89fef-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="89fef-103">domain: verify</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89fef-104">ドメインの所有権を検証します。</span><span class="sxs-lookup"><span data-stu-id="89fef-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="89fef-p101">**重要:** 未検証のドメインにのみ適用されます。未検証のドメインでは、[domain](../resources/domain.md) の isVerified プロパティは false です。</span><span class="sxs-lookup"><span data-stu-id="89fef-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="89fef-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89fef-107">Permissions</span></span>

<span data-ttu-id="89fef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89fef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="89fef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89fef-110">Permission type</span></span>      | <span data-ttu-id="89fef-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89fef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89fef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89fef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89fef-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="89fef-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="89fef-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89fef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89fef-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89fef-115">Not supported.</span></span>    |
|<span data-ttu-id="89fef-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89fef-116">Application</span></span> | <span data-ttu-id="89fef-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89fef-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89fef-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89fef-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="89fef-119">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="89fef-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89fef-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89fef-120">Request headers</span></span>

| <span data-ttu-id="89fef-121">名前</span><span class="sxs-lookup"><span data-stu-id="89fef-121">Name</span></span>       | <span data-ttu-id="89fef-122">説明</span><span class="sxs-lookup"><span data-stu-id="89fef-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89fef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89fef-123">Authorization</span></span>  | <span data-ttu-id="89fef-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="89fef-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="89fef-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89fef-126">Content-Type</span></span>  | <span data-ttu-id="89fef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89fef-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="89fef-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="89fef-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="89fef-129">応答</span><span class="sxs-lookup"><span data-stu-id="89fef-129">Response</span></span>

<span data-ttu-id="89fef-130">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89fef-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89fef-131">例</span><span class="sxs-lookup"><span data-stu-id="89fef-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89fef-132">要求</span><span class="sxs-lookup"><span data-stu-id="89fef-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="89fef-133">応答</span><span class="sxs-lookup"><span data-stu-id="89fef-133">Response</span></span>
<span data-ttu-id="89fef-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89fef-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="89fef-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="89fef-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="89fef-137">C#</span><span class="sxs-lookup"><span data-stu-id="89fef-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_verify-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89fef-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="89fef-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_verify-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="89fef-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="89fef-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/domain_verify-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
