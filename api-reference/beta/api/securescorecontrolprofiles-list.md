---
title: secureScoreControlProfiles のリスト
description: securescorecontrolprofiles のオブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 6627111633f54eb7bc2584af826b69fd5bd6cf49
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545634"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="d9d3d-103">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="d9d3d-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9d3d-104">[securescorecontrolprofiles の](../resources/securescorecontrolprofiles.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9d3d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9d3d-105">Permissions</span></span>

<span data-ttu-id="d9d3d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9d3d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9d3d-108">Permission type</span></span>      | <span data-ttu-id="d9d3d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9d3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9d3d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9d3d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d9d3d-111">securityevents。 all、securityevents.。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="d9d3d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9d3d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d9d3d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-113">Not supported.</span></span>  |
|<span data-ttu-id="d9d3d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9d3d-114">Application</span></span> | <span data-ttu-id="d9d3d-115">securityevents。 all、securityevents.。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9d3d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9d3d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d9d3d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9d3d-117">Request headers</span></span>

| <span data-ttu-id="d9d3d-118">名前</span><span class="sxs-lookup"><span data-stu-id="d9d3d-118">Name</span></span>      |<span data-ttu-id="d9d3d-119">説明</span><span class="sxs-lookup"><span data-stu-id="d9d3d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d9d3d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9d3d-120">Authorization</span></span>  | <span data-ttu-id="d9d3d-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-121">Bearer {code}.</span></span> <span data-ttu-id="d9d3d-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9d3d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9d3d-123">Request body</span></span>

<span data-ttu-id="d9d3d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9d3d-125">応答</span><span class="sxs-lookup"><span data-stu-id="d9d3d-125">Response</span></span>

<span data-ttu-id="d9d3d-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**securescorecontrolprofiles の**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9d3d-127">例</span><span class="sxs-lookup"><span data-stu-id="d9d3d-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9d3d-128">要求</span><span class="sxs-lookup"><span data-stu-id="d9d3d-128">Request</span></span>

<span data-ttu-id="d9d3d-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="d9d3d-130">応答</span><span class="sxs-lookup"><span data-stu-id="d9d3d-130">Response</span></span>

<span data-ttu-id="d9d3d-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9d3d-131">The following is an example of the response.</span></span>
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
