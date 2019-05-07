---
title: secureScores のリスト
description: SecureScore オブジェクトのリストを取得します。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: 85fd63ed4bad46df8de7ebf802b6008361d992fd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629734"
---
# <a name="list-securescores"></a><span data-ttu-id="dab84-103">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="dab84-103">List secureScores</span></span>

<span data-ttu-id="dab84-104">[SecureScore](../resources/securescore.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="dab84-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="dab84-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dab84-105">Permissions</span></span>

<span data-ttu-id="dab84-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dab84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dab84-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dab84-108">Permission type</span></span>      | <span data-ttu-id="dab84-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dab84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dab84-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dab84-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="dab84-111">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="dab84-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="dab84-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dab84-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dab84-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dab84-113">Not supported.</span></span>  |
|<span data-ttu-id="dab84-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dab84-114">Application</span></span> | <span data-ttu-id="dab84-115">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="dab84-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dab84-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dab84-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dab84-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dab84-117">Optional query parameters</span></span>

<span data-ttu-id="dab84-118">このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](/graph/query-parameters)をサポートします:</span><span class="sxs-lookup"><span data-stu-id="dab84-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="dab84-119">`$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="dab84-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="dab84-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dab84-120">Request headers</span></span>

| <span data-ttu-id="dab84-121">名前</span><span class="sxs-lookup"><span data-stu-id="dab84-121">Name</span></span>      |<span data-ttu-id="dab84-122">説明</span><span class="sxs-lookup"><span data-stu-id="dab84-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dab84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dab84-123">Authorization</span></span>  | <span data-ttu-id="dab84-124">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="dab84-124">Bearer {code}.</span></span> <span data-ttu-id="dab84-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="dab84-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dab84-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dab84-126">Request body</span></span>

<span data-ttu-id="dab84-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dab84-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="dab84-128">要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="dab84-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="dab84-129">応答</span><span class="sxs-lookup"><span data-stu-id="dab84-129">Response</span></span>

<span data-ttu-id="dab84-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScores**オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="dab84-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dab84-131">例</span><span class="sxs-lookup"><span data-stu-id="dab84-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dab84-132">要求</span><span class="sxs-lookup"><span data-stu-id="dab84-132">Request</span></span>

<span data-ttu-id="dab84-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dab84-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="dab84-134">応答</span><span class="sxs-lookup"><span data-stu-id="dab84-134">Response</span></span>

<span data-ttu-id="dab84-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dab84-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScore",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "00000001-0001-0001-0001-000000000001c_2019-03-19",
            "azureTenantId": "00000001-0001-0001-0001-000000000001c",
            "activeUserCount": 0,
            "createdDateTime": "2019-03-19T15:21:00Z",
            "currentScore": 387.0,
            "enabledServices": [
                "HasExchange",
                "HasSharePoint",
                "HasInTune"
            ],
            "licensedUserCount": 100,
            "maxScore": 697.0,
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": 37.0
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": 46.0
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": 109.0
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "Identity",
                    "controlName": "AdminMFA",
                    "description": "Requiring multi-factor authentication (MFA) for all Azure Active Directory accounts with privileged roles",
                    "score": 35.0
                },
                {
                    "controlCategory": "Data",
                    "controlName": "DLPEnabled",
                    "description": "Data Loss Prevention (DLP) policies can be used to comply with business standards and industry regulations.",
                    "score": 20.0
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
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->