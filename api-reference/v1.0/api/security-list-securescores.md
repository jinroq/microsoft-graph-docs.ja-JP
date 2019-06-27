---
title: secureScores のリスト
description: SecureScore オブジェクトのリストを取得します。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: ba63b8b6043c2079943b83be46227c31a197dce9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273172"
---
# <a name="list-securescores"></a><span data-ttu-id="130af-103">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="130af-103">List secureScores</span></span>

<span data-ttu-id="130af-104">[SecureScore](../resources/securescore.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="130af-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="130af-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="130af-105">Permissions</span></span>

<span data-ttu-id="130af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="130af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="130af-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="130af-108">Permission type</span></span>      | <span data-ttu-id="130af-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="130af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="130af-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="130af-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="130af-111">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="130af-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="130af-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="130af-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="130af-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="130af-113">Not supported.</span></span>  |
|<span data-ttu-id="130af-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="130af-114">Application</span></span> | <span data-ttu-id="130af-115">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="130af-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="130af-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="130af-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="130af-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="130af-117">Optional query parameters</span></span>

<span data-ttu-id="130af-118">このメソッドは、応答をカスタマイズするために次の [OData クエリ パラメーター](/graph/query-parameters)をサポートします:</span><span class="sxs-lookup"><span data-stu-id="130af-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="130af-119">`$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="130af-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="130af-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="130af-120">Request headers</span></span>

| <span data-ttu-id="130af-121">名前</span><span class="sxs-lookup"><span data-stu-id="130af-121">Name</span></span>      |<span data-ttu-id="130af-122">説明</span><span class="sxs-lookup"><span data-stu-id="130af-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="130af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="130af-123">Authorization</span></span>  | <span data-ttu-id="130af-124">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="130af-124">Bearer {code}.</span></span> <span data-ttu-id="130af-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="130af-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="130af-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="130af-126">Request body</span></span>

<span data-ttu-id="130af-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="130af-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="130af-128">要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="130af-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="130af-129">応答</span><span class="sxs-lookup"><span data-stu-id="130af-129">Response</span></span>

<span data-ttu-id="130af-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScores**オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="130af-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="130af-131">例</span><span class="sxs-lookup"><span data-stu-id="130af-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="130af-132">要求</span><span class="sxs-lookup"><span data-stu-id="130af-132">Request</span></span>

<span data-ttu-id="130af-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="130af-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="130af-134">応答</span><span class="sxs-lookup"><span data-stu-id="130af-134">Response</span></span>

<span data-ttu-id="130af-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="130af-135">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="130af-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="130af-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="130af-137">C#</span><span class="sxs-lookup"><span data-stu-id="130af-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securescores-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="130af-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="130af-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securescores-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="130af-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="130af-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_securescores-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
