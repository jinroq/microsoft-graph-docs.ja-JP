---
title: PublishedResource を onPremisesAgentGroup に割り当てます。
description: '**Publishedresource**オブジェクトを**onPremisesAgentGroup**オブジェクトに割り当てます。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ec20b1208906129e5559307fc347e9d39c6dd7e
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840969"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="7dc0d-103">PublishedResource を onPremisesAgentGroup に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-103">Assign publishedResource to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dc0d-104">[Publishedresource](../resources/publishedresource.md)オブジェクトを[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-104">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dc0d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7dc0d-105">Permissions</span></span>

<span data-ttu-id="7dc0d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7dc0d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7dc0d-108">Permission type</span></span>                        | <span data-ttu-id="7dc0d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7dc0d-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="7dc0d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7dc0d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7dc0d-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="7dc0d-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="7dc0d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7dc0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dc0d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-113">Not supported.</span></span> |
| <span data-ttu-id="7dc0d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7dc0d-114">Application</span></span>                            | <span data-ttu-id="7dc0d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dc0d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7dc0d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7dc0d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dc0d-117">Request headers</span></span>

| <span data-ttu-id="7dc0d-118">名前</span><span class="sxs-lookup"><span data-stu-id="7dc0d-118">Name</span></span>          | <span data-ttu-id="7dc0d-119">説明</span><span class="sxs-lookup"><span data-stu-id="7dc0d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7dc0d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dc0d-120">Authorization</span></span> | <span data-ttu-id="7dc0d-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="7dc0d-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dc0d-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="7dc0d-122">Request body</span></span>

<span data-ttu-id="7dc0d-123">要求本文で、 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-123">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7dc0d-124">応答</span><span class="sxs-lookup"><span data-stu-id="7dc0d-124">Response</span></span>

<span data-ttu-id="7dc0d-125">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[publishedresource](../resources/publishedresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-125">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7dc0d-126">例</span><span class="sxs-lookup"><span data-stu-id="7dc0d-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7dc0d-127">要求</span><span class="sxs-lookup"><span data-stu-id="7dc0d-127">Request</span></span>

<span data-ttu-id="7dc0d-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
Content-type: application/json

```http
{
 "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2B032383-897C-42BA-917E-700B6890BDC3/"
}
```

### <a name="response"></a><span data-ttu-id="7dc0d-129">応答</span><span class="sxs-lookup"><span data-stu-id="7dc0d-129">Response</span></span>

<span data-ttu-id="7dc0d-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-130">The following is an example of the response.</span></span>

> <span data-ttu-id="7dc0d-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7dc0d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204
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
