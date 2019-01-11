---
title: 'domain: verify'
description: ドメインの所有権を検証します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 359a266acf854e4353bce4eda0f65191ca2783c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814834"
---
# <a name="domain-verify"></a><span data-ttu-id="8d5cb-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="8d5cb-103">domain: verify</span></span>

<span data-ttu-id="8d5cb-104">ドメインの所有権を検証します。</span><span class="sxs-lookup"><span data-stu-id="8d5cb-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="8d5cb-p101">**重要:** 未検証のドメインにのみ適用されます。未検証のドメインでは、[domain](../resources/domain.md) の isVerified プロパティは false です。</span><span class="sxs-lookup"><span data-stu-id="8d5cb-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d5cb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d5cb-107">Permissions</span></span>

<span data-ttu-id="8d5cb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d5cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8d5cb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d5cb-110">Permission type</span></span>      | <span data-ttu-id="8d5cb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d5cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d5cb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d5cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d5cb-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d5cb-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="8d5cb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d5cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d5cb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d5cb-115">Not supported.</span></span>    |
|<span data-ttu-id="8d5cb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d5cb-116">Application</span></span> | <span data-ttu-id="8d5cb-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d5cb-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d5cb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d5cb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="8d5cb-119">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="8d5cb-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d5cb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d5cb-120">Request headers</span></span>

| <span data-ttu-id="8d5cb-121">名前</span><span class="sxs-lookup"><span data-stu-id="8d5cb-121">Name</span></span>       | <span data-ttu-id="8d5cb-122">説明</span><span class="sxs-lookup"><span data-stu-id="8d5cb-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d5cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d5cb-123">Authorization</span></span>  | <span data-ttu-id="8d5cb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8d5cb-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8d5cb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d5cb-126">Content-Type</span></span>  | <span data-ttu-id="8d5cb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8d5cb-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d5cb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d5cb-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8d5cb-129">応答</span><span class="sxs-lookup"><span data-stu-id="8d5cb-129">Response</span></span>

<span data-ttu-id="8d5cb-130">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d5cb-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d5cb-131">例</span><span class="sxs-lookup"><span data-stu-id="8d5cb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d5cb-132">要求</span><span class="sxs-lookup"><span data-stu-id="8d5cb-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```

##### <a name="response"></a><span data-ttu-id="8d5cb-133">応答</span><span class="sxs-lookup"><span data-stu-id="8d5cb-133">Response</span></span>
<span data-ttu-id="8d5cb-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d5cb-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
