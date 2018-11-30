---
title: リスト secureScoreControlProfiles
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 33d0f6059d66350c9fa763097277f83c041e96ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069668"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="5be44-104">リスト secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="5be44-104">List secureScoreControlProfiles</span></span>

 > <span data-ttu-id="5be44-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5be44-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5be44-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5be44-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5be44-107">プロパティと、 [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="5be44-107">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5be44-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5be44-108">Permissions</span></span>

<span data-ttu-id="5be44-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5be44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5be44-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5be44-111">Permission type</span></span>      | <span data-ttu-id="5be44-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5be44-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5be44-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5be44-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="5be44-114">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="5be44-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="5be44-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5be44-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5be44-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5be44-116">Not supported.</span></span>  |
|<span data-ttu-id="5be44-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5be44-117">Application</span></span> | <span data-ttu-id="5be44-118">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="5be44-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5be44-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5be44-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="5be44-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5be44-120">Request headers</span></span>

| <span data-ttu-id="5be44-121">名前</span><span class="sxs-lookup"><span data-stu-id="5be44-121">Name</span></span>      |<span data-ttu-id="5be44-122">説明</span><span class="sxs-lookup"><span data-stu-id="5be44-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5be44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5be44-123">Authorization</span></span>  | <span data-ttu-id="5be44-p104">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="5be44-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5be44-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5be44-126">Request body</span></span>

<span data-ttu-id="5be44-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5be44-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5be44-128">応答</span><span class="sxs-lookup"><span data-stu-id="5be44-128">Response</span></span>

<span data-ttu-id="5be44-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**secureScoreControlProfiles**オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5be44-129">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5be44-130">例</span><span class="sxs-lookup"><span data-stu-id="5be44-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5be44-131">要求</span><span class="sxs-lookup"><span data-stu-id="5be44-131">Request</span></span>

<span data-ttu-id="5be44-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5be44-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="5be44-133">応答</span><span class="sxs-lookup"><span data-stu-id="5be44-133">Response</span></span>

<span data-ttu-id="5be44-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5be44-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "actionType": "actionType.value",
            "actionUrl": "actionUrl.value",
            "controlCategory": "controlCategory.value",
            "title": "title.value",
            "deprecated": "deprecated.value",
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": "maxScore.value",
            "rank": "rank.value",
            "remediation": "remediation.value",
            "remediationImpact": "remediationImpact.value",
            "service": "service.value",
            "threats": [
                "threats.value"
            ],
            "tier": "tier.value",
            "userImpact": "userImpact.value",
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "controlStateUpdates": [
                {
                    "assignedTo": "assignedTo.value",
                    "comment": "comment.value",
                    "state": "state.value",
                    "updatedBy": "updatedBy.value",
                    "updatedDateTime": "updatedDateTime.value"
                }
            ],
            "vendorInformation": {
                "provider": "SecureScore",
                "providerVersion": null,
                "subProvider": null,
                "vendor": "Microsoft"
            }
         }
     ]
}
```


<!-- {
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
