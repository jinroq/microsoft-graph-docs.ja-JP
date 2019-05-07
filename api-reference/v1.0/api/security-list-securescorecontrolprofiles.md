---
title: secureScoreControlProfiles のリスト
description: Securescorecontrolprofiles のオブジェクトのプロパティとリレーションシップを取得します。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: d7de3b6b446aa12447023d6b4f111fc2ac28b41e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629741"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="42b44-103">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="42b44-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="42b44-104">[Securescorecontrolprofiles の](../resources/securescorecontrolprofile.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="42b44-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42b44-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="42b44-105">Permissions</span></span>

<span data-ttu-id="42b44-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42b44-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42b44-108">Permission type</span></span>      | <span data-ttu-id="42b44-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="42b44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42b44-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="42b44-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="42b44-111">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="42b44-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="42b44-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42b44-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="42b44-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42b44-113">Not supported.</span></span>  |
|<span data-ttu-id="42b44-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42b44-114">Application</span></span> | <span data-ttu-id="42b44-115">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="42b44-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42b44-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42b44-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42b44-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="42b44-117">Optional query parameters</span></span>

<span data-ttu-id="42b44-118">このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](/graph/query-parameters)をサポートします:</span><span class="sxs-lookup"><span data-stu-id="42b44-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="42b44-119">`$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="42b44-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="42b44-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42b44-120">Request headers</span></span>

| <span data-ttu-id="42b44-121">名前</span><span class="sxs-lookup"><span data-stu-id="42b44-121">Name</span></span>      |<span data-ttu-id="42b44-122">説明</span><span class="sxs-lookup"><span data-stu-id="42b44-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42b44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42b44-123">Authorization</span></span>  | <span data-ttu-id="42b44-124">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="42b44-124">Bearer {code}.</span></span> <span data-ttu-id="42b44-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="42b44-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42b44-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="42b44-126">Request body</span></span>

<span data-ttu-id="42b44-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="42b44-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="42b44-128">要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="42b44-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="42b44-129">応答</span><span class="sxs-lookup"><span data-stu-id="42b44-129">Response</span></span>

<span data-ttu-id="42b44-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**securescorecontrolprofiles の**オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="42b44-130">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42b44-131">例</span><span class="sxs-lookup"><span data-stu-id="42b44-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="42b44-132">要求</span><span class="sxs-lookup"><span data-stu-id="42b44-132">Request</span></span>

<span data-ttu-id="42b44-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42b44-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="42b44-134">応答</span><span class="sxs-lookup"><span data-stu-id="42b44-134">Response</span></span>

<span data-ttu-id="42b44-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42b44-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
  "value": [
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
              "name":  "A.8.2.1",
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
  ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
