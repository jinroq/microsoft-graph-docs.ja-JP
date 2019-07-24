---
title: OnPremisesAgentGroup を作成する
description: 新しい**onPremisesAgentGroup**オブジェクトを作成します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 752081e6b50460e8185f4bddddce603bf54e5d86
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841095"
---
# <a name="create-onpremisesagentgroup"></a><span data-ttu-id="98661-103">OnPremisesAgentGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="98661-103">Create onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98661-104">新しい[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="98661-104">Create a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="98661-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98661-105">Permissions</span></span>

<span data-ttu-id="98661-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98661-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98661-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98661-108">Permission type</span></span>                        | <span data-ttu-id="98661-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98661-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="98661-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98661-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="98661-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="98661-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="98661-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98661-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98661-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98661-113">Not supported.</span></span> |
| <span data-ttu-id="98661-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98661-114">Application</span></span>                            | <span data-ttu-id="98661-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98661-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98661-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98661-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}/agents
```

## <a name="request-headers"></a><span data-ttu-id="98661-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98661-117">Request headers</span></span>

| <span data-ttu-id="98661-118">名前</span><span class="sxs-lookup"><span data-stu-id="98661-118">Name</span></span>          | <span data-ttu-id="98661-119">説明</span><span class="sxs-lookup"><span data-stu-id="98661-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="98661-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="98661-120">Authorization</span></span> | <span data-ttu-id="98661-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="98661-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="98661-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="98661-122">Request body</span></span>

<span data-ttu-id="98661-123">要求本文で、 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="98661-123">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

## <a name="response"></a><span data-ttu-id="98661-124">応答</span><span class="sxs-lookup"><span data-stu-id="98661-124">Response</span></span>

<span data-ttu-id="98661-125">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="98661-125">If successful, this method returns a `201 Created` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98661-126">例</span><span class="sxs-lookup"><span data-stu-id="98661-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98661-127">要求</span><span class="sxs-lookup"><span data-stu-id="98661-127">Request</span></span>

<span data-ttu-id="98661-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98661-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_onpremisesagentgroup"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups
```

<span data-ttu-id="98661-129">要求本文で、 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="98661-129">In the request body, supply a JSON representation of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

### <a name="response"></a><span data-ttu-id="98661-130">応答</span><span class="sxs-lookup"><span data-stu-id="98661-130">Response</span></span>

<span data-ttu-id="98661-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98661-131">The following is an example of the response.</span></span>

> <span data-ttu-id="98661-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="98661-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "displayName": "New Group",
    "publishingType": "provisioning",
    "isDefault": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
