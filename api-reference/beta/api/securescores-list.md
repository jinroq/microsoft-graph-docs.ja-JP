---
title: secureScores のリスト
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 6bf0a1e1964c93043bad4a81ab812786627ea737
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831816"
---
# <a name="list-securescores"></a><span data-ttu-id="b33b3-104">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="b33b3-104">List secureScores</span></span>

 > <span data-ttu-id="b33b3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b33b3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b33b3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b33b3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b33b3-107">プロパティと、 [secureScores](../resources/securescores.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="b33b3-107">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b33b3-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b33b3-108">Permissions</span></span>

<span data-ttu-id="b33b3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b33b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b33b3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b33b3-111">Permission type</span></span>      | <span data-ttu-id="b33b3-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b33b3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b33b3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b33b3-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b33b3-114">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="b33b3-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="b33b3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b33b3-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b33b3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b33b3-116">Not supported.</span></span>  |
|<span data-ttu-id="b33b3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b33b3-117">Application</span></span> | <span data-ttu-id="b33b3-118">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="b33b3-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b33b3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b33b3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="b33b3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b33b3-120">Request headers</span></span>

| <span data-ttu-id="b33b3-121">名前</span><span class="sxs-lookup"><span data-stu-id="b33b3-121">Name</span></span>      |<span data-ttu-id="b33b3-122">説明</span><span class="sxs-lookup"><span data-stu-id="b33b3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b33b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b33b3-123">Authorization</span></span>  | <span data-ttu-id="b33b3-p104">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="b33b3-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b33b3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b33b3-126">Request body</span></span>

<span data-ttu-id="b33b3-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b33b3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b33b3-128">応答</span><span class="sxs-lookup"><span data-stu-id="b33b3-128">Response</span></span>

<span data-ttu-id="b33b3-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**secureScores**オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b33b3-129">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b33b3-130">例</span><span class="sxs-lookup"><span data-stu-id="b33b3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b33b3-131">要求</span><span class="sxs-lookup"><span data-stu-id="b33b3-131">Request</span></span>

<span data-ttu-id="b33b3-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b33b3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="b33b3-133">応答</span><span class="sxs-lookup"><span data-stu-id="b33b3-133">Response</span></span>

<span data-ttu-id="b33b3-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b33b3-134">The following is an example of the response.</span></span>
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
