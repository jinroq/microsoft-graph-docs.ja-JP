---
title: RiskDetection を取得する
description: '**Riskdetection**オブジェクトのプロパティを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f56d04901b26365fc5a63461032799c372ea456
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358313"
---
# <a name="get-riskdetection"></a><span data-ttu-id="5046f-103">RiskDetection を取得する</span><span class="sxs-lookup"><span data-stu-id="5046f-103">Get riskDetection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5046f-104">**RiskDetection**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="5046f-104">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="5046f-105">リスク検出 API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="5046f-105">You must have an Azure AD Premium P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="5046f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5046f-106">Permissions</span></span>
<span data-ttu-id="5046f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5046f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5046f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5046f-109">Permission type</span></span>      | <span data-ttu-id="5046f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5046f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5046f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5046f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5046f-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="5046f-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="5046f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5046f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5046f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5046f-114">Not supported.</span></span>    |
|<span data-ttu-id="5046f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5046f-115">Application</span></span> | <span data-ttu-id="5046f-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="5046f-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5046f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5046f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5046f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5046f-118">Request headers</span></span>
| <span data-ttu-id="5046f-119">名前</span><span class="sxs-lookup"><span data-stu-id="5046f-119">Name</span></span>      |<span data-ttu-id="5046f-120">説明</span><span class="sxs-lookup"><span data-stu-id="5046f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5046f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5046f-121">Authorization</span></span>  | <span data-ttu-id="5046f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5046f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5046f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5046f-124">Content-Type</span></span> | <span data-ttu-id="5046f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5046f-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5046f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5046f-126">Request body</span></span>
<span data-ttu-id="5046f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5046f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5046f-128">応答</span><span class="sxs-lookup"><span data-stu-id="5046f-128">Response</span></span>

<span data-ttu-id="5046f-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskDetection](../resources/riskdetection.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5046f-129">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5046f-130">例</span><span class="sxs-lookup"><span data-stu-id="5046f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5046f-131">要求</span><span class="sxs-lookup"><span data-stu-id="5046f-131">Request</span></span>
<span data-ttu-id="5046f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5046f-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5046f-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5046f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5046f-134">C#</span><span class="sxs-lookup"><span data-stu-id="5046f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5046f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5046f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5046f-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="5046f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5046f-137">Java</span><span class="sxs-lookup"><span data-stu-id="5046f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5046f-138">応答</span><span class="sxs-lookup"><span data-stu-id="5046f-138">Response</span></span>
<span data-ttu-id="5046f-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5046f-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskType": "unfamiliarFeatures",
    "riskState": "remediated",
    "riskLevel": "medium",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "source": "activeDirectory",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "Olivia Lack",
    "userPrincipalName": "olack@adatum.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskDetection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

