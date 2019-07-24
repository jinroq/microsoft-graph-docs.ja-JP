---
title: OnPremisesPublishingProfile を取得する
description: '[OnPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92e2800d03cb2e9aab59c119b7a9b7e9f09682d7
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841074"
---
# <a name="get-onpremisespublishingprofile"></a><span data-ttu-id="e6423-103">OnPremisesPublishingProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="e6423-103">Get onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6423-104">[OnPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="e6423-104">Retrieve the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6423-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e6423-105">Permissions</span></span>

<span data-ttu-id="e6423-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6423-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6423-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6423-108">Permission type</span></span>                        | <span data-ttu-id="e6423-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6423-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="e6423-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6423-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6423-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="e6423-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="e6423-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6423-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6423-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6423-113">Not supported.</span></span> |
| <span data-ttu-id="e6423-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6423-114">Application</span></span>                            | <span data-ttu-id="e6423-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6423-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6423-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6423-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6423-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e6423-117">Optional query parameters</span></span>

<span data-ttu-id="e6423-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e6423-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6423-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6423-119">Request headers</span></span>

| <span data-ttu-id="e6423-120">名前</span><span class="sxs-lookup"><span data-stu-id="e6423-120">Name</span></span>      |<span data-ttu-id="e6423-121">説明</span><span class="sxs-lookup"><span data-stu-id="e6423-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6423-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6423-122">Authorization</span></span> | <span data-ttu-id="e6423-123">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="e6423-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6423-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6423-124">Request body</span></span>

<span data-ttu-id="e6423-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e6423-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6423-126">応答</span><span class="sxs-lookup"><span data-stu-id="e6423-126">Response</span></span>

<span data-ttu-id="e6423-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e6423-127">If successful, this method returns a `200 OK` response code and an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6423-128">例</span><span class="sxs-lookup"><span data-stu-id="e6423-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6423-129">要求</span><span class="sxs-lookup"><span data-stu-id="e6423-129">Request</span></span>

<span data-ttu-id="e6423-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e6423-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```

### <a name="response"></a><span data-ttu-id="e6423-131">応答</span><span class="sxs-lookup"><span data-stu-id="e6423-131">Response</span></span>

<span data-ttu-id="e6423-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e6423-132">The following is an example of the response.</span></span>

> <span data-ttu-id="e6423-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e6423-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
