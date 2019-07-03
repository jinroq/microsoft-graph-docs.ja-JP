---
title: secureScores のリスト
description: SecureScore オブジェクトのリストを取得します。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: a632a0abdf15d91fc37a511ab75b50d8233d5a4c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441626"
---
# <a name="list-securescores"></a><span data-ttu-id="674f6-103">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="674f6-103">List secureScores</span></span>

<span data-ttu-id="674f6-104">[SecureScore](../resources/securescore.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="674f6-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="674f6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="674f6-105">Permissions</span></span>

<span data-ttu-id="674f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="674f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="674f6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="674f6-108">Permission type</span></span>      | <span data-ttu-id="674f6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="674f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="674f6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="674f6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="674f6-111">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="674f6-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="674f6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="674f6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="674f6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="674f6-113">Not supported.</span></span>  |
|<span data-ttu-id="674f6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="674f6-114">Application</span></span> | <span data-ttu-id="674f6-115">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="674f6-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="674f6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="674f6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="674f6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="674f6-117">Optional query parameters</span></span>

<span data-ttu-id="674f6-118">このメソッドは、応答をカスタマイズするために次の [OData クエリ パラメーター](/graph/query-parameters)をサポートします:</span><span class="sxs-lookup"><span data-stu-id="674f6-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="674f6-119">`$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="674f6-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="674f6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="674f6-120">Request headers</span></span>

| <span data-ttu-id="674f6-121">名前</span><span class="sxs-lookup"><span data-stu-id="674f6-121">Name</span></span>      |<span data-ttu-id="674f6-122">説明</span><span class="sxs-lookup"><span data-stu-id="674f6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="674f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="674f6-123">Authorization</span></span>  | <span data-ttu-id="674f6-124">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="674f6-124">Bearer {code}.</span></span> <span data-ttu-id="674f6-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="674f6-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="674f6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="674f6-126">Request body</span></span>

<span data-ttu-id="674f6-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="674f6-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="674f6-128">要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="674f6-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="674f6-129">応答</span><span class="sxs-lookup"><span data-stu-id="674f6-129">Response</span></span>

<span data-ttu-id="674f6-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScores**オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="674f6-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="674f6-131">例</span><span class="sxs-lookup"><span data-stu-id="674f6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="674f6-132">要求</span><span class="sxs-lookup"><span data-stu-id="674f6-132">Request</span></span>

<span data-ttu-id="674f6-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="674f6-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="674f6-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="674f6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="674f6-135">C#</span><span class="sxs-lookup"><span data-stu-id="674f6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="674f6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="674f6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="674f6-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="674f6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="674f6-138">応答</span><span class="sxs-lookup"><span data-stu-id="674f6-138">Response</span></span>

<span data-ttu-id="674f6-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="674f6-139">The following is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}
-->
