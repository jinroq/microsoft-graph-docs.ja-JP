---
title: secureScoreControlProfiles のリスト
description: Securescorecontrolprofiles のオブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 220051afcb0d53b8e24482f8531a8442289357c5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269056"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="e8c1b-103">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="e8c1b-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8c1b-104">テナントの[secureScoreControlProfile](../resources/securescorecontrolprofiles.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8c1b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8c1b-105">Permissions</span></span>

<span data-ttu-id="e8c1b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8c1b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8c1b-108">Permission type</span></span>      | <span data-ttu-id="e8c1b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8c1b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8c1b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8c1b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e8c1b-111">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="e8c1b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8c1b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e8c1b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-113">Not supported.</span></span>  |
|<span data-ttu-id="e8c1b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8c1b-114">Application</span></span> | <span data-ttu-id="e8c1b-115">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8c1b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8c1b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e8c1b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8c1b-117">Request headers</span></span>

| <span data-ttu-id="e8c1b-118">名前</span><span class="sxs-lookup"><span data-stu-id="e8c1b-118">Name</span></span>      |<span data-ttu-id="e8c1b-119">説明</span><span class="sxs-lookup"><span data-stu-id="e8c1b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8c1b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8c1b-120">Authorization</span></span>  | <span data-ttu-id="e8c1b-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-121">Bearer {code}.</span></span> <span data-ttu-id="e8c1b-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8c1b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8c1b-123">Request body</span></span>

<span data-ttu-id="e8c1b-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8c1b-125">応答</span><span class="sxs-lookup"><span data-stu-id="e8c1b-125">Response</span></span>

<span data-ttu-id="e8c1b-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScoreControlProfile**オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8c1b-127">例</span><span class="sxs-lookup"><span data-stu-id="e8c1b-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8c1b-128">要求</span><span class="sxs-lookup"><span data-stu-id="e8c1b-128">Request</span></span>

<span data-ttu-id="e8c1b-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="e8c1b-130">応答</span><span class="sxs-lookup"><span data-stu-id="e8c1b-130">Response</span></span>

<span data-ttu-id="e8c1b-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8c1b-131">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8c1b-132">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e8c1b-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8c1b-133">C#</span><span class="sxs-lookup"><span data-stu-id="e8c1b-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8c1b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8c1b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e8c1b-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="e8c1b-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
