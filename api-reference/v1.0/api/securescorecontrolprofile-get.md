---
title: SecureScoreControlProfile を取得する
description: SecureScoreControlProfile オブジェクトのプロパティとリレーションシップを取得します。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 6accac07ab66a57303dd3881b47daae82deb2a9f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629755"
---
# <a name="get-securescorecontrolprofile"></a><span data-ttu-id="0235b-103">SecureScoreControlProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="0235b-103">Get secureScoreControlProfile</span></span>

<span data-ttu-id="0235b-104">[Securescorecontrolprofile](../resources/securescorecontrolprofile.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="0235b-104">Retrieve the properties and relationships of an [securescorecontrolprofile](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0235b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0235b-105">Permissions</span></span>

<span data-ttu-id="0235b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0235b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0235b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0235b-108">Permission type</span></span>      | <span data-ttu-id="0235b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0235b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0235b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0235b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0235b-111">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0235b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="0235b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0235b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0235b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0235b-113">Not supported.</span></span>  |
|<span data-ttu-id="0235b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0235b-114">Application</span></span> | <span data-ttu-id="0235b-115">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0235b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0235b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0235b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securescorecontrolprofiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0235b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0235b-117">Request headers</span></span>

| <span data-ttu-id="0235b-118">名前</span><span class="sxs-lookup"><span data-stu-id="0235b-118">Name</span></span>      |<span data-ttu-id="0235b-119">説明</span><span class="sxs-lookup"><span data-stu-id="0235b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0235b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0235b-120">Authorization</span></span>  | <span data-ttu-id="0235b-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="0235b-121">Bearer {code}.</span></span> <span data-ttu-id="0235b-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="0235b-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0235b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0235b-123">Request body</span></span>

<span data-ttu-id="0235b-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0235b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0235b-125">応答</span><span class="sxs-lookup"><span data-stu-id="0235b-125">Response</span></span>

<span data-ttu-id="0235b-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScoreControlProfile**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0235b-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfile** object in the response body.</span></span> <span data-ttu-id="0235b-127">プロバイダーから 2xx または 404 以外の状態コードが返されるか、プロバイダーがタイムアウトした場合、応答は、警告ヘッダー内のプロバイダーの応答と共に`206 Partial Content` 状態コードになります。</span><span class="sxs-lookup"><span data-stu-id="0235b-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="0235b-128">詳細については、[Microsoft グラフ セキュリティ API のエラー応答](../resources/security-error-codes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0235b-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="0235b-129">例</span><span class="sxs-lookup"><span data-stu-id="0235b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0235b-130">要求</span><span class="sxs-lookup"><span data-stu-id="0235b-130">Request</span></span>

<span data-ttu-id="0235b-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0235b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}
```

### <a name="response"></a><span data-ttu-id="0235b-132">応答</span><span class="sxs-lookup"><span data-stu-id="0235b-132">Response</span></span>

<span data-ttu-id="0235b-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0235b-133">The following is an example of the response.</span></span>
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
  "tocPath": ""
}
-->
