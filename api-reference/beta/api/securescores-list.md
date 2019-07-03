---
title: secureScores のリスト
description: SecureScores オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 1a4994b2e767906b0058bf85936375949f609fbd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457346"
---
# <a name="list-securescores"></a><span data-ttu-id="dcef2-103">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="dcef2-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcef2-104">[SecureScores](../resources/securescores.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="dcef2-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcef2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dcef2-105">Permissions</span></span>

<span data-ttu-id="dcef2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcef2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcef2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dcef2-108">Permission type</span></span>      | <span data-ttu-id="dcef2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dcef2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcef2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dcef2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="dcef2-111">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="dcef2-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="dcef2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcef2-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dcef2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcef2-113">Not supported.</span></span>  |
|<span data-ttu-id="dcef2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dcef2-114">Application</span></span> | <span data-ttu-id="dcef2-115">SecurityEvents。 All、SecurityEvents.。</span><span class="sxs-lookup"><span data-stu-id="dcef2-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcef2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dcef2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="dcef2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcef2-117">Request headers</span></span>

| <span data-ttu-id="dcef2-118">名前</span><span class="sxs-lookup"><span data-stu-id="dcef2-118">Name</span></span>      |<span data-ttu-id="dcef2-119">説明</span><span class="sxs-lookup"><span data-stu-id="dcef2-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcef2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcef2-120">Authorization</span></span>  | <span data-ttu-id="dcef2-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="dcef2-121">Bearer {code}.</span></span> <span data-ttu-id="dcef2-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="dcef2-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcef2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="dcef2-123">Request body</span></span>

<span data-ttu-id="dcef2-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dcef2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcef2-125">応答</span><span class="sxs-lookup"><span data-stu-id="dcef2-125">Response</span></span>

<span data-ttu-id="dcef2-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScores**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dcef2-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcef2-127">例</span><span class="sxs-lookup"><span data-stu-id="dcef2-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcef2-128">要求</span><span class="sxs-lookup"><span data-stu-id="dcef2-128">Request</span></span>

<span data-ttu-id="dcef2-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dcef2-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dcef2-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dcef2-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcef2-131">C#</span><span class="sxs-lookup"><span data-stu-id="dcef2-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescores-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcef2-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="dcef2-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescores-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcef2-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="dcef2-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescores-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dcef2-134">応答</span><span class="sxs-lookup"><span data-stu-id="dcef2-134">Response</span></span>

<span data-ttu-id="dcef2-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dcef2-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection":true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 1,
            "createdDateTime": "createdDateTime.value",
            "currentScore": 1,
            "enabledServices": "enabledServices.value",
            "licensedUserCount": 1,
            "maxScore": 1,
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value"
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "seatSizeRangeUpperValue": "seatSizeRangeUpperValue.value",
                    "categoryValue": "categoryValue.value",
                    "seatSizeRangeLowerValue": "seatSizeRangeLowerValue.value"
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "categoryValue": "categoryValue.value"
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
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
