---
title: secureScoreControlProfiles のリスト
description: Securescorecontrolprofiles のオブジェクトのプロパティとリレーションシップを取得します。
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4134aa533bf547a8b32b510e4e965139a771f3f4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347704"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="f8216-103">secureScoreControlProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="f8216-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="f8216-104">[Securescorecontrolprofiles の](../resources/securescorecontrolprofile.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="f8216-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8216-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f8216-105">Permissions</span></span>

<span data-ttu-id="f8216-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8216-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8216-108">Permission type</span></span>      | <span data-ttu-id="f8216-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8216-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8216-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8216-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f8216-111">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="f8216-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="f8216-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8216-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f8216-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8216-113">Not supported.</span></span>  |
|<span data-ttu-id="f8216-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8216-114">Application</span></span> | <span data-ttu-id="f8216-115">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="f8216-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8216-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8216-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8216-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f8216-117">Optional query parameters</span></span>

<span data-ttu-id="f8216-118">このメソッドは、応答をカスタマイズするために次の [OData クエリ パラメーター](/graph/query-parameters)をサポートします:</span><span class="sxs-lookup"><span data-stu-id="f8216-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="f8216-119">`$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="f8216-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="f8216-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8216-120">Request headers</span></span>

| <span data-ttu-id="f8216-121">名前</span><span class="sxs-lookup"><span data-stu-id="f8216-121">Name</span></span>      |<span data-ttu-id="f8216-122">説明</span><span class="sxs-lookup"><span data-stu-id="f8216-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f8216-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8216-123">Authorization</span></span>  | <span data-ttu-id="f8216-124">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="f8216-124">Bearer {code}.</span></span> <span data-ttu-id="f8216-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="f8216-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8216-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8216-126">Request body</span></span>

<span data-ttu-id="f8216-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f8216-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="f8216-128">要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="f8216-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="f8216-129">応答</span><span class="sxs-lookup"><span data-stu-id="f8216-129">Response</span></span>

<span data-ttu-id="f8216-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**securescorecontrolprofiles の**オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f8216-130">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8216-131">例</span><span class="sxs-lookup"><span data-stu-id="f8216-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8216-132">要求</span><span class="sxs-lookup"><span data-stu-id="f8216-132">Request</span></span>

<span data-ttu-id="f8216-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f8216-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f8216-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f8216-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f8216-135">C#</span><span class="sxs-lookup"><span data-stu-id="f8216-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofiles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8216-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8216-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofiles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f8216-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="f8216-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofiles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f8216-138">Java</span><span class="sxs-lookup"><span data-stu-id="f8216-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescorecontrolprofiles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8216-139">応答</span><span class="sxs-lookup"><span data-stu-id="f8216-139">Response</span></span>

<span data-ttu-id="f8216-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f8216-140">The following is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}
-->
