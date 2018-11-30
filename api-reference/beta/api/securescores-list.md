---
title: リスト secureScores
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: f5466e24d6b523809a72f712666063808987e530
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068071"
---
# <a name="list-securescores"></a><span data-ttu-id="e64b1-104">リスト secureScores</span><span class="sxs-lookup"><span data-stu-id="e64b1-104">List secureScores</span></span>

 > <span data-ttu-id="e64b1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e64b1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e64b1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e64b1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e64b1-107">プロパティと、 [secureScores](../resources/securescores.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="e64b1-107">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e64b1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e64b1-108">Permissions</span></span>

<span data-ttu-id="e64b1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e64b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e64b1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e64b1-111">Permission type</span></span>      | <span data-ttu-id="e64b1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e64b1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e64b1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e64b1-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e64b1-114">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="e64b1-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="e64b1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e64b1-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e64b1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e64b1-116">Not supported.</span></span>  |
|<span data-ttu-id="e64b1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e64b1-117">Application</span></span> | <span data-ttu-id="e64b1-118">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="e64b1-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e64b1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e64b1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="e64b1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e64b1-120">Request headers</span></span>

| <span data-ttu-id="e64b1-121">名前</span><span class="sxs-lookup"><span data-stu-id="e64b1-121">Name</span></span>      |<span data-ttu-id="e64b1-122">説明</span><span class="sxs-lookup"><span data-stu-id="e64b1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e64b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e64b1-123">Authorization</span></span>  | <span data-ttu-id="e64b1-p104">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="e64b1-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e64b1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e64b1-126">Request body</span></span>

<span data-ttu-id="e64b1-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e64b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e64b1-128">応答</span><span class="sxs-lookup"><span data-stu-id="e64b1-128">Response</span></span>

<span data-ttu-id="e64b1-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**secureScores**オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e64b1-129">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e64b1-130">例</span><span class="sxs-lookup"><span data-stu-id="e64b1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e64b1-131">要求</span><span class="sxs-lookup"><span data-stu-id="e64b1-131">Request</span></span>

<span data-ttu-id="e64b1-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e64b1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="e64b1-133">応答</span><span class="sxs-lookup"><span data-stu-id="e64b1-133">Response</span></span>

<span data-ttu-id="e64b1-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e64b1-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScores"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "activeUserCount": "activeUserCount.value",
            "createdDateTime": "createdDateTime.value",
            "currentScore": "currentScore.value",
            "enabledServices": "enabledServices.value",
            "licensedUserCount": "licensedUserCount.value",
            "maxScore": "maxScore.value",
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


<!-- {
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
