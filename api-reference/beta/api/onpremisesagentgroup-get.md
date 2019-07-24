---
title: OnPremisesAgentGroup を取得する
description: '[OnPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4243f0e16d432d9756ec2f414aae23ad8ed4730b
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841144"
---
# <a name="get-onpremisesagentgroup"></a><span data-ttu-id="f4155-103">OnPremisesAgentGroup を取得する</span><span class="sxs-lookup"><span data-stu-id="f4155-103">Get onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4155-104">[OnPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="f4155-104">Retrieve the properties and relationships of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4155-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4155-105">Permissions</span></span>

<span data-ttu-id="f4155-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4155-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4155-108">Permission type</span></span>                        | <span data-ttu-id="f4155-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4155-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4155-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4155-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4155-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="f4155-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="f4155-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4155-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4155-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4155-113">Not supported.</span></span> |
| <span data-ttu-id="f4155-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4155-114">Application</span></span>                            | <span data-ttu-id="f4155-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4155-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4155-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4155-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4155-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4155-117">Optional query parameters</span></span>

<span data-ttu-id="f4155-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f4155-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4155-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4155-119">Request headers</span></span>

| <span data-ttu-id="f4155-120">名前</span><span class="sxs-lookup"><span data-stu-id="f4155-120">Name</span></span>      |<span data-ttu-id="f4155-121">説明</span><span class="sxs-lookup"><span data-stu-id="f4155-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4155-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4155-122">Authorization</span></span> | <span data-ttu-id="f4155-123">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="f4155-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4155-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4155-124">Request body</span></span>

<span data-ttu-id="f4155-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f4155-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4155-126">応答</span><span class="sxs-lookup"><span data-stu-id="f4155-126">Response</span></span>

<span data-ttu-id="f4155-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で要求された[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f4155-127">If successful, this method returns a `200 OK` response code and the requested [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4155-128">例</span><span class="sxs-lookup"><span data-stu-id="f4155-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4155-129">要求</span><span class="sxs-lookup"><span data-stu-id="f4155-129">Request</span></span>

<span data-ttu-id="f4155-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4155-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagentgroup"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2d55ed41-1619-4848-92bb-0576d3038682/?$expand=publishedResources,agents
```

### <a name="response"></a><span data-ttu-id="f4155-131">応答</span><span class="sxs-lookup"><span data-stu-id="f4155-131">Response</span></span>

<span data-ttu-id="f4155-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4155-132">The following is an example of the response.</span></span>

> <span data-ttu-id="f4155-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f4155-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
    "displayName": "Group 1",
    "publishingType": "provisioning",
    "isDefault": false,
    "agents": [
            {
            "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
            "status": "Active"
            }
    ],
    "publishedResources": [
        {
            "displayName": "Provisioning",
            "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
            "resourceName": "domain1.contoso.com"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
