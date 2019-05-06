---
title: 'domain: verify'
description: ドメインの所有権を検証します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2d3139a9911be2f6e813f7e40051bd2286f0349e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589460"
---
# <a name="domain-verify"></a><span data-ttu-id="ad77e-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="ad77e-103">domain: verify</span></span>

<span data-ttu-id="ad77e-104">ドメインの所有権を検証します。</span><span class="sxs-lookup"><span data-stu-id="ad77e-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="ad77e-p101">**重要:** 未検証のドメインにのみ適用されます。未検証のドメインでは、[domain](../resources/domain.md) の isVerified プロパティは false です。</span><span class="sxs-lookup"><span data-stu-id="ad77e-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad77e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad77e-107">Permissions</span></span>

<span data-ttu-id="ad77e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad77e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad77e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad77e-110">Permission type</span></span>      | <span data-ttu-id="ad77e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad77e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad77e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad77e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad77e-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad77e-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="ad77e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad77e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad77e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad77e-115">Not supported.</span></span>    |
|<span data-ttu-id="ad77e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad77e-116">Application</span></span> | <span data-ttu-id="ad77e-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad77e-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad77e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad77e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="ad77e-119">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="ad77e-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad77e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad77e-120">Request headers</span></span>

| <span data-ttu-id="ad77e-121">名前</span><span class="sxs-lookup"><span data-stu-id="ad77e-121">Name</span></span>       | <span data-ttu-id="ad77e-122">説明</span><span class="sxs-lookup"><span data-stu-id="ad77e-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad77e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad77e-123">Authorization</span></span>  | <span data-ttu-id="ad77e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad77e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ad77e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad77e-126">Content-Type</span></span>  | <span data-ttu-id="ad77e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ad77e-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad77e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad77e-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ad77e-129">応答</span><span class="sxs-lookup"><span data-stu-id="ad77e-129">Response</span></span>

<span data-ttu-id="ad77e-130">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad77e-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad77e-131">例</span><span class="sxs-lookup"><span data-stu-id="ad77e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad77e-132">要求</span><span class="sxs-lookup"><span data-stu-id="ad77e-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```

##### <a name="response"></a><span data-ttu-id="ad77e-133">応答</span><span class="sxs-lookup"><span data-stu-id="ad77e-133">Response</span></span>
<span data-ttu-id="ad77e-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad77e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad77e-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="ad77e-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad77e-137">Visual</span><span class="sxs-lookup"><span data-stu-id="ad77e-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_verify-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad77e-138">Java</span><span class="sxs-lookup"><span data-stu-id="ad77e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_verify-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
