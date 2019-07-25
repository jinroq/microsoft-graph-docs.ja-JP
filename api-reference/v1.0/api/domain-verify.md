---
title: 'domain: verify'
description: ドメインの所有権を検証します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ac8a1dd07b2fd426b05952f003a9bdf39f4cafab
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883237"
---
# <a name="domain-verify"></a><span data-ttu-id="63440-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="63440-103">domain: verify</span></span>

<span data-ttu-id="63440-104">ドメインの所有権を検証します。</span><span class="sxs-lookup"><span data-stu-id="63440-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="63440-p101">**重要:** 未検証のドメインにのみ適用されます。未検証のドメインでは、[domain](../resources/domain.md) の isVerified プロパティは false です。</span><span class="sxs-lookup"><span data-stu-id="63440-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="63440-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="63440-107">Permissions</span></span>

<span data-ttu-id="63440-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63440-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="63440-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="63440-110">Permission type</span></span>      | <span data-ttu-id="63440-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="63440-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63440-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="63440-112">Delegated (work or school account)</span></span> | <span data-ttu-id="63440-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="63440-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="63440-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="63440-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63440-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63440-115">Not supported.</span></span>    |
|<span data-ttu-id="63440-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="63440-116">Application</span></span> | <span data-ttu-id="63440-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63440-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63440-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="63440-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="63440-119">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="63440-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63440-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63440-120">Request headers</span></span>

| <span data-ttu-id="63440-121">名前</span><span class="sxs-lookup"><span data-stu-id="63440-121">Name</span></span>       | <span data-ttu-id="63440-122">説明</span><span class="sxs-lookup"><span data-stu-id="63440-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63440-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63440-123">Authorization</span></span>  | <span data-ttu-id="63440-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="63440-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="63440-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63440-126">Content-Type</span></span>  | <span data-ttu-id="63440-127">application/json</span><span class="sxs-lookup"><span data-stu-id="63440-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="63440-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="63440-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="63440-129">応答</span><span class="sxs-lookup"><span data-stu-id="63440-129">Response</span></span>

<span data-ttu-id="63440-130">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="63440-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63440-131">例</span><span class="sxs-lookup"><span data-stu-id="63440-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63440-132">要求</span><span class="sxs-lookup"><span data-stu-id="63440-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63440-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="63440-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="63440-134">C#</span><span class="sxs-lookup"><span data-stu-id="63440-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-verify-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63440-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="63440-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-verify-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63440-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="63440-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-verify-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="63440-137">Java</span><span class="sxs-lookup"><span data-stu-id="63440-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-verify-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="63440-138">応答</span><span class="sxs-lookup"><span data-stu-id="63440-138">Response</span></span>
<span data-ttu-id="63440-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="63440-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
