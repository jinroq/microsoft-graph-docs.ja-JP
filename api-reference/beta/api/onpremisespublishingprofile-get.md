---
title: OnPremisesPublishingProfile を取得する
description: '[OnPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb3d6b43473ea1660976170625009ecea5c50baf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878426"
---
# <a name="get-onpremisespublishingprofile"></a><span data-ttu-id="6511d-103">OnPremisesPublishingProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="6511d-103">Get onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6511d-104">[OnPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="6511d-104">Retrieve the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6511d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6511d-105">Permissions</span></span>

<span data-ttu-id="6511d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6511d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6511d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6511d-108">Permission type</span></span>                        | <span data-ttu-id="6511d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6511d-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="6511d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6511d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6511d-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="6511d-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6511d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6511d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6511d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6511d-113">Not supported.</span></span> |
| <span data-ttu-id="6511d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6511d-114">Application</span></span>                            | <span data-ttu-id="6511d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6511d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6511d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6511d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6511d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6511d-117">Optional query parameters</span></span>

<span data-ttu-id="6511d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6511d-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6511d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6511d-119">Request headers</span></span>

| <span data-ttu-id="6511d-120">名前</span><span class="sxs-lookup"><span data-stu-id="6511d-120">Name</span></span>      |<span data-ttu-id="6511d-121">説明</span><span class="sxs-lookup"><span data-stu-id="6511d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6511d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6511d-122">Authorization</span></span> | <span data-ttu-id="6511d-123">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="6511d-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6511d-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="6511d-124">Request body</span></span>

<span data-ttu-id="6511d-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6511d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6511d-126">応答</span><span class="sxs-lookup"><span data-stu-id="6511d-126">Response</span></span>

<span data-ttu-id="6511d-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6511d-127">If successful, this method returns a `200 OK` response code and an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6511d-128">例</span><span class="sxs-lookup"><span data-stu-id="6511d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6511d-129">要求</span><span class="sxs-lookup"><span data-stu-id="6511d-129">Request</span></span>

<span data-ttu-id="6511d-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6511d-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6511d-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6511d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6511d-132">C#</span><span class="sxs-lookup"><span data-stu-id="6511d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6511d-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6511d-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6511d-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="6511d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6511d-135">Java</span><span class="sxs-lookup"><span data-stu-id="6511d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6511d-136">応答</span><span class="sxs-lookup"><span data-stu-id="6511d-136">Response</span></span>

<span data-ttu-id="6511d-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6511d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="6511d-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6511d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```json
HTTP/1.1 200 OK

{
    "publishedResources": [
        {
            "publishingType": "provisioning",
            "displayName": "Demo Provisioning",
            "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
            "resourceName": "domain1.contoso.com",
            "agentGroups": [
                {
                    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
                    "displayName": "Group 1"
                }
            ]
        }
    ],
    "agents": [
        {
            "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
            "status": "Active",
            "machineName": "server 1",
            "externalIp": "1.0.0.127",
            "agentGroups": [
                 {
                    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
                    "displayName": "Group 1"
                 }
            ]
        }
    ],
    "agentGroups": [
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
    ],
  "hybridAgentUpdaterConfiguration": {
       "deferUpdateDateTime" : "2018-08-12T12:00",
       "updateWindow" :
          {
            "updateWindowStartTime" : "0:00:00",
            "updateWindowEndTime" : "23:59:00.0000000"
          },
       "allowUpdateConfigurationOverride" : false
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesPublishingProfile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
