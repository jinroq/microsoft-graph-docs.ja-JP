---
title: OnPremisesAgent を onPremisesAgentGroup に割り当てる
description: OnPremisesAgent を onPremisesAgentGroup に割り当てます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b33e7ab511effeab4e8d8e7576b704b092917199
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878608"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="9af7f-103">OnPremisesAgent を onPremisesAgentGroup に割り当てる</span><span class="sxs-lookup"><span data-stu-id="9af7f-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9af7f-104">[OnPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトに[onPremisesAgent](../resources/onpremisesagent.md)を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="9af7f-104">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9af7f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9af7f-105">Permissions</span></span>

<span data-ttu-id="9af7f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9af7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9af7f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9af7f-108">Permission type</span></span>                        | <span data-ttu-id="9af7f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9af7f-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9af7f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9af7f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9af7f-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="9af7f-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="9af7f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9af7f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9af7f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9af7f-113">Not supported.</span></span> |
| <span data-ttu-id="9af7f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9af7f-114">Application</span></span>                            | <span data-ttu-id="9af7f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9af7f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9af7f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9af7f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9af7f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9af7f-117">Request headers</span></span>

| <span data-ttu-id="9af7f-118">名前</span><span class="sxs-lookup"><span data-stu-id="9af7f-118">Name</span></span>          | <span data-ttu-id="9af7f-119">説明</span><span class="sxs-lookup"><span data-stu-id="9af7f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9af7f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9af7f-120">Authorization</span></span> | <span data-ttu-id="9af7f-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="9af7f-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9af7f-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="9af7f-122">Request body</span></span>

<span data-ttu-id="9af7f-123">要求本文で、 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトへの OData 参照の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9af7f-123">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9af7f-124">応答</span><span class="sxs-lookup"><span data-stu-id="9af7f-124">Response</span></span>

<span data-ttu-id="9af7f-125">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9af7f-125">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9af7f-126">例</span><span class="sxs-lookup"><span data-stu-id="9af7f-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9af7f-127">要求</span><span class="sxs-lookup"><span data-stu-id="9af7f-127">Request</span></span>

<span data-ttu-id="9af7f-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9af7f-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9af7f-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9af7f-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9af7f-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="9af7f-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9af7f-131">目的-C</span><span class="sxs-lookup"><span data-stu-id="9af7f-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="9af7f-132">要求本文で、 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトへの OData 参照の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9af7f-132">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="9af7f-133">応答</span><span class="sxs-lookup"><span data-stu-id="9af7f-133">Response</span></span>

<span data-ttu-id="9af7f-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9af7f-134">The following is an example of the response.</span></span>

> <span data-ttu-id="9af7f-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9af7f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
