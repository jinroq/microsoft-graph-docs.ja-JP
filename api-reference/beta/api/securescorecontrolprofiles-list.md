---
title: secureScoreControlProfiles のリスト
description: securescorecontrolprofiles のオブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 29efa2c9bedaa295304eb82190a64fbc4a863cd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331563"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="e2e02-103">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="e2e02-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2e02-104">テナントの[secureScoreControlProfile](../resources/securescorecontrolprofiles.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e2e02-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2e02-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2e02-105">Permissions</span></span>

<span data-ttu-id="e2e02-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2e02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2e02-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2e02-108">Permission type</span></span>      | <span data-ttu-id="e2e02-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2e02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2e02-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2e02-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e2e02-111">securityevents。 all、securityevents.。</span><span class="sxs-lookup"><span data-stu-id="e2e02-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="e2e02-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2e02-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e2e02-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2e02-113">Not supported.</span></span>  |
|<span data-ttu-id="e2e02-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2e02-114">Application</span></span> | <span data-ttu-id="e2e02-115">securityevents。 all、securityevents.。</span><span class="sxs-lookup"><span data-stu-id="e2e02-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2e02-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2e02-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e2e02-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2e02-117">Request headers</span></span>

| <span data-ttu-id="e2e02-118">名前</span><span class="sxs-lookup"><span data-stu-id="e2e02-118">Name</span></span>      |<span data-ttu-id="e2e02-119">説明</span><span class="sxs-lookup"><span data-stu-id="e2e02-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2e02-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2e02-120">Authorization</span></span>  | <span data-ttu-id="e2e02-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="e2e02-121">Bearer {code}.</span></span> <span data-ttu-id="e2e02-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="e2e02-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2e02-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2e02-123">Request body</span></span>

<span data-ttu-id="e2e02-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2e02-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2e02-125">応答</span><span class="sxs-lookup"><span data-stu-id="e2e02-125">Response</span></span>

<span data-ttu-id="e2e02-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScoreControlProfile**オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e2e02-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2e02-127">例</span><span class="sxs-lookup"><span data-stu-id="e2e02-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2e02-128">要求</span><span class="sxs-lookup"><span data-stu-id="e2e02-128">Request</span></span>

<span data-ttu-id="e2e02-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2e02-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="e2e02-130">応答</span><span class="sxs-lookup"><span data-stu-id="e2e02-130">Response</span></span>

<span data-ttu-id="e2e02-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2e02-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
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
            "deprecated": true,
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": 1020.13,
            "rank": 100,
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
