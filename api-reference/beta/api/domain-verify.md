---
title: 'domain: verify'
description: ドメインの所有権を検証します。
author: lleonard-msft
ms.openlocfilehash: 246d037d7f87ec463c6d68a9d9e22b4cff7cb695
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336646"
---
# <a name="domain-verify"></a><span data-ttu-id="0d697-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="0d697-103">domain: verify</span></span>

> <span data-ttu-id="0d697-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d697-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d697-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d697-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d697-106">ドメインの所有権を検証します。</span><span class="sxs-lookup"><span data-stu-id="0d697-106">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="0d697-p102">**重要:** 未検証のドメインにのみ適用されます。未検証のドメインでは、[domain](../resources/domain.md) の isVerified プロパティは false です。</span><span class="sxs-lookup"><span data-stu-id="0d697-p102">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d697-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0d697-109">Permissions</span></span>

<span data-ttu-id="0d697-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d697-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0d697-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d697-112">Permission type</span></span>      | <span data-ttu-id="0d697-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d697-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d697-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d697-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0d697-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d697-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="0d697-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d697-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d697-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d697-117">Not supported.</span></span>    |
|<span data-ttu-id="0d697-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d697-118">Application</span></span> | <span data-ttu-id="0d697-119">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d697-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d697-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d697-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="0d697-121">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="0d697-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d697-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d697-122">Request headers</span></span>

| <span data-ttu-id="0d697-123">名前</span><span class="sxs-lookup"><span data-stu-id="0d697-123">Name</span></span>       | <span data-ttu-id="0d697-124">説明</span><span class="sxs-lookup"><span data-stu-id="0d697-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d697-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d697-125">Authorization</span></span>  | <span data-ttu-id="0d697-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0d697-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0d697-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d697-128">Content-Type</span></span>  | <span data-ttu-id="0d697-129">application/json</span><span class="sxs-lookup"><span data-stu-id="0d697-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d697-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d697-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0d697-131">応答</span><span class="sxs-lookup"><span data-stu-id="0d697-131">Response</span></span>

<span data-ttu-id="0d697-132">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0d697-132">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d697-133">例</span><span class="sxs-lookup"><span data-stu-id="0d697-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d697-134">要求</span><span class="sxs-lookup"><span data-stu-id="0d697-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="0d697-135">応答</span><span class="sxs-lookup"><span data-stu-id="0d697-135">Response</span></span>
<span data-ttu-id="0d697-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d697-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->