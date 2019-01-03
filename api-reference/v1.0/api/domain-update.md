---
title: ドメインを更新する
description: ドメイン オブジェクトのプロパティを更新します。
author: lleonard-msft
ms.openlocfilehash: d1ba59d345f172f1485dda628585fe8de549ee1d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356428"
---
# <a name="update-domain"></a><span data-ttu-id="fc52b-103">ドメインを更新する</span><span class="sxs-lookup"><span data-stu-id="fc52b-103">Update domain</span></span>

<span data-ttu-id="fc52b-104">ドメイン オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fc52b-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="fc52b-105">**重要:** 検証済みのドメインのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="fc52b-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc52b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fc52b-106">Permissions</span></span>

<span data-ttu-id="fc52b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc52b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc52b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fc52b-109">Permission type</span></span>      | <span data-ttu-id="fc52b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fc52b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc52b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fc52b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc52b-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc52b-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc52b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fc52b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc52b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc52b-114">Not supported.</span></span>    |
|<span data-ttu-id="fc52b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fc52b-115">Application</span></span> | <span data-ttu-id="fc52b-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc52b-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc52b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fc52b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="fc52b-118">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="fc52b-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc52b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc52b-119">Request headers</span></span>

| <span data-ttu-id="fc52b-120">名前</span><span class="sxs-lookup"><span data-stu-id="fc52b-120">Name</span></span>       | <span data-ttu-id="fc52b-121">説明</span><span class="sxs-lookup"><span data-stu-id="fc52b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fc52b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc52b-122">Authorization</span></span>  | <span data-ttu-id="fc52b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fc52b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc52b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc52b-125">Content-Type</span></span>  | <span data-ttu-id="fc52b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc52b-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc52b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fc52b-127">Request body</span></span>

<span data-ttu-id="fc52b-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るには、変更する値のみを含めます。</span><span class="sxs-lookup"><span data-stu-id="fc52b-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="fc52b-131">応答</span><span class="sxs-lookup"><span data-stu-id="fc52b-131">Response</span></span>

<span data-ttu-id="fc52b-132">成功した場合、このメソッドは `204 No Content` 応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="fc52b-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc52b-133">例</span><span class="sxs-lookup"><span data-stu-id="fc52b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc52b-134">要求</span><span class="sxs-lookup"><span data-stu-id="fc52b-134">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="fc52b-135">応答</span><span class="sxs-lookup"><span data-stu-id="fc52b-135">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->