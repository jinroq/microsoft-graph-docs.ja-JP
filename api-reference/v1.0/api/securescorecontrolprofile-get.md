---
title: secureScoreControlProfile の取得
description: SecureScoreControlProfile オブジェクトのプロパティとリレーションシップを取得します。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 5a596f51aa64a935fefcfcf85f725d3235f12238
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448296"
---
# <a name="get-securescorecontrolprofile"></a><span data-ttu-id="d3fdc-103">secureScoreControlProfile の取得</span><span class="sxs-lookup"><span data-stu-id="d3fdc-103">Get secureScoreControlProfile</span></span>

<span data-ttu-id="d3fdc-104">[Securescorecontrolprofile](../resources/securescorecontrolprofile.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-104">Retrieve the properties and relationships of an [securescorecontrolprofile](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3fdc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d3fdc-105">Permissions</span></span>

<span data-ttu-id="d3fdc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3fdc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3fdc-108">Permission type</span></span>      | <span data-ttu-id="d3fdc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3fdc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3fdc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3fdc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d3fdc-111">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3fdc-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="d3fdc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3fdc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d3fdc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-113">Not supported.</span></span>  |
|<span data-ttu-id="d3fdc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3fdc-114">Application</span></span> | <span data-ttu-id="d3fdc-115">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3fdc-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3fdc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3fdc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securescorecontrolprofiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d3fdc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3fdc-117">Request headers</span></span>

| <span data-ttu-id="d3fdc-118">名前</span><span class="sxs-lookup"><span data-stu-id="d3fdc-118">Name</span></span>      |<span data-ttu-id="d3fdc-119">説明</span><span class="sxs-lookup"><span data-stu-id="d3fdc-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3fdc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3fdc-120">Authorization</span></span>  | <span data-ttu-id="d3fdc-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-121">Bearer {code}.</span></span> <span data-ttu-id="d3fdc-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3fdc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3fdc-123">Request body</span></span>

<span data-ttu-id="d3fdc-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3fdc-125">応答</span><span class="sxs-lookup"><span data-stu-id="d3fdc-125">Response</span></span>

<span data-ttu-id="d3fdc-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScoreControlProfile**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfile** object in the response body.</span></span> <span data-ttu-id="d3fdc-127">プロバイダーから 2xx または 404 以外の状態コードが返されるか、プロバイダーがタイムアウトした場合、応答は、警告ヘッダー内のプロバイダーの応答と共に状態コード `206 Partial Content` になります。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="d3fdc-128">詳細については、「[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="d3fdc-129">例</span><span class="sxs-lookup"><span data-stu-id="d3fdc-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3fdc-130">要求</span><span class="sxs-lookup"><span data-stu-id="d3fdc-130">Request</span></span>

<span data-ttu-id="d3fdc-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d3fdc-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d3fdc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3fdc-133">C#</span><span class="sxs-lookup"><span data-stu-id="d3fdc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3fdc-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3fdc-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3fdc-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="d3fdc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3fdc-136">応答</span><span class="sxs-lookup"><span data-stu-id="d3fdc-136">Response</span></span>

<span data-ttu-id="d3fdc-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3fdc-137">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "DLPEnabled",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Config",
  "actionUrl": "https://compliance.microsoft.com/#/policies",
  "controlCategory": "Data",
  "title": "Apply Data Loss Prevention policies", 
  "deprecated": false,
  "implementationCost": "Moderate",
  "lastModifiedDateTime": null,
  "maxScore": 20.0,
  "rank": 55,
  "remediation": "You can create and manage data loss prevention policies in the Policies page of the compliance portal.",
  "remediationImpact": "This change will have a moderate impact on your users.",
  "service": "IP",
  "threats": [
    "Data Exfiltration",
    "Data Spillage"
  ],
  "tier": "Advanced",
  "userImpact": "Moderate",
  "complianceInformation": [
    {
      "certificationName": "ISO 27001:2013",
      "certificationControls": [
        {
          "name": "A.8.2.1",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": null,
      "comment": null,
      "state": "Default",
      "updatedBy": null,
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "get secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
