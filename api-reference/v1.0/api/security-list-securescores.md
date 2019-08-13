---
title: secureScores のリスト
description: SecureScore オブジェクトのリストを取得します。
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8210f96b4db8a05efc2fa1c82c384ec822c4afb1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307876"
---
# <a name="list-securescores"></a><span data-ttu-id="7f8fc-103">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="7f8fc-103">List secureScores</span></span>

<span data-ttu-id="7f8fc-104">[SecureScore](../resources/securescore.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f8fc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f8fc-105">Permissions</span></span>

<span data-ttu-id="7f8fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f8fc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f8fc-108">Permission type</span></span>      | <span data-ttu-id="7f8fc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f8fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f8fc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f8fc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7f8fc-111">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="7f8fc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f8fc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7f8fc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-113">Not supported.</span></span>  |
|<span data-ttu-id="7f8fc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f8fc-114">Application</span></span> | <span data-ttu-id="7f8fc-115">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f8fc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f8fc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f8fc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f8fc-117">Optional query parameters</span></span>

<span data-ttu-id="7f8fc-118">このメソッドは、応答をカスタマイズするために次の [OData クエリ パラメーター](/graph/query-parameters)をサポートします:</span><span class="sxs-lookup"><span data-stu-id="7f8fc-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="7f8fc-119">`$top` は、各セキュリティ API プロバイダーから集計された上位の結果を返します。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="7f8fc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f8fc-120">Request headers</span></span>

| <span data-ttu-id="7f8fc-121">名前</span><span class="sxs-lookup"><span data-stu-id="7f8fc-121">Name</span></span>      |<span data-ttu-id="7f8fc-122">説明</span><span class="sxs-lookup"><span data-stu-id="7f8fc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f8fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f8fc-123">Authorization</span></span>  | <span data-ttu-id="7f8fc-124">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-124">Bearer {code}.</span></span> <span data-ttu-id="7f8fc-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f8fc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f8fc-126">Request body</span></span>

<span data-ttu-id="7f8fc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="7f8fc-128">要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="7f8fc-129">応答</span><span class="sxs-lookup"><span data-stu-id="7f8fc-129">Response</span></span>

<span data-ttu-id="7f8fc-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScores**オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f8fc-131">例</span><span class="sxs-lookup"><span data-stu-id="7f8fc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f8fc-132">要求</span><span class="sxs-lookup"><span data-stu-id="7f8fc-132">Request</span></span>

<span data-ttu-id="7f8fc-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7f8fc-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7f8fc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f8fc-135">C#</span><span class="sxs-lookup"><span data-stu-id="7f8fc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f8fc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f8fc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f8fc-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="7f8fc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7f8fc-138">Java</span><span class="sxs-lookup"><span data-stu-id="7f8fc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescores-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f8fc-139">応答</span><span class="sxs-lookup"><span data-stu-id="7f8fc-139">Response</span></span>

<span data-ttu-id="7f8fc-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f8fc-140">The following is an example of the response.</span></span>
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
