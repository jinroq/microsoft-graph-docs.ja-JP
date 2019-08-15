---
title: OnPremisesAgentGroup から publishedResource を削除する
description: '[OnPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトから[publishedresource](../resources/publishedresource.md)オブジェクトを削除します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d83be65fb44a68a2474ce7a6ed360960c6084a9c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412398"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="2a7d1-103">OnPremisesAgentGroup から publishedResource を削除する</span><span class="sxs-lookup"><span data-stu-id="2a7d1-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a7d1-104">[OnPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトから[publishedresource](../resources/publishedresource.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2a7d1-104">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a7d1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a7d1-105">Permissions</span></span>

<span data-ttu-id="2a7d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a7d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a7d1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a7d1-108">Permission type</span></span>                        | <span data-ttu-id="2a7d1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a7d1-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="2a7d1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a7d1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a7d1-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="2a7d1-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="2a7d1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a7d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a7d1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a7d1-113">Not supported.</span></span> |
| <span data-ttu-id="2a7d1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a7d1-114">Application</span></span>                            | <span data-ttu-id="2a7d1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a7d1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a7d1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a7d1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2a7d1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a7d1-117">Request headers</span></span>

| <span data-ttu-id="2a7d1-118">名前</span><span class="sxs-lookup"><span data-stu-id="2a7d1-118">Name</span></span>          | <span data-ttu-id="2a7d1-119">説明</span><span class="sxs-lookup"><span data-stu-id="2a7d1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2a7d1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a7d1-120">Authorization</span></span> | <span data-ttu-id="2a7d1-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="2a7d1-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a7d1-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a7d1-122">Request body</span></span>

<span data-ttu-id="2a7d1-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a7d1-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a7d1-124">応答</span><span class="sxs-lookup"><span data-stu-id="2a7d1-124">Response</span></span>

<span data-ttu-id="2a7d1-125">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2a7d1-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2a7d1-126">例</span><span class="sxs-lookup"><span data-stu-id="2a7d1-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a7d1-127">要求</span><span class="sxs-lookup"><span data-stu-id="2a7d1-127">Request</span></span>

<span data-ttu-id="2a7d1-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a7d1-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2a7d1-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2a7d1-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2a7d1-130">C#</span><span class="sxs-lookup"><span data-stu-id="2a7d1-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a7d1-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a7d1-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a7d1-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="2a7d1-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a7d1-133">応答</span><span class="sxs-lookup"><span data-stu-id="2a7d1-133">Response</span></span>

<span data-ttu-id="2a7d1-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a7d1-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
