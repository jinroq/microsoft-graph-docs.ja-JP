---
title: リスト onPremisesAgentGroups
description: OnPremisesAgentGroup オブジェクトのリストを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 53409381e117c0c93d4626642397f1952fabc864
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878477"
---
# <a name="list-onpremisesagentgroups"></a><span data-ttu-id="73ef5-103">リスト onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="73ef5-103">List onPremisesAgentGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73ef5-104">[OnPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="73ef5-104">Retrieve a list of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="73ef5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73ef5-105">Permissions</span></span>

<span data-ttu-id="73ef5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73ef5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73ef5-108">Permission type</span></span>                        | <span data-ttu-id="73ef5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73ef5-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="73ef5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73ef5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="73ef5-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="73ef5-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="73ef5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73ef5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73ef5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73ef5-113">Not supported.</span></span> |
| <span data-ttu-id="73ef5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73ef5-114">Application</span></span>                            | <span data-ttu-id="73ef5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73ef5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73ef5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73ef5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73ef5-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73ef5-117">Optional query parameters</span></span>

<span data-ttu-id="73ef5-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="73ef5-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73ef5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73ef5-119">Request headers</span></span>

| <span data-ttu-id="73ef5-120">名前</span><span class="sxs-lookup"><span data-stu-id="73ef5-120">Name</span></span>      |<span data-ttu-id="73ef5-121">説明</span><span class="sxs-lookup"><span data-stu-id="73ef5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73ef5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73ef5-122">Authorization</span></span> | <span data-ttu-id="73ef5-123">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="73ef5-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="73ef5-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="73ef5-124">Request body</span></span>

<span data-ttu-id="73ef5-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73ef5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73ef5-126">応答</span><span class="sxs-lookup"><span data-stu-id="73ef5-126">Response</span></span>

<span data-ttu-id="73ef5-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="73ef5-127">If successful, this method returns a `200 OK` response code and collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73ef5-128">例</span><span class="sxs-lookup"><span data-stu-id="73ef5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73ef5-129">要求</span><span class="sxs-lookup"><span data-stu-id="73ef5-129">Request</span></span>

<span data-ttu-id="73ef5-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="73ef5-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73ef5-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="73ef5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agentgroups"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups?$expand=agents,publishedResources
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73ef5-132">C#</span><span class="sxs-lookup"><span data-stu-id="73ef5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agentgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73ef5-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="73ef5-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agentgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73ef5-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="73ef5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agentgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73ef5-135">Java</span><span class="sxs-lookup"><span data-stu-id="73ef5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agentgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73ef5-136">応答</span><span class="sxs-lookup"><span data-stu-id="73ef5-136">Response</span></span>

<span data-ttu-id="73ef5-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="73ef5-137">The following is an example of the response.</span></span>

> <span data-ttu-id="73ef5-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="73ef5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
                    "displayName": "Demo Provisioning",
                    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
                    "resourceName": "domain1.contoso.com"
                }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
