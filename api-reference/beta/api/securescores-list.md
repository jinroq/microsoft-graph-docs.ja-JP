---
title: secureScores のリスト
description: プロパティと、secureScores オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: e574c3e52eb60f29dac89e2795b04666c7a1f02b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521482"
---
# <a name="list-securescores"></a><span data-ttu-id="a9c96-103">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="a9c96-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9c96-104">プロパティと、 [secureScores](../resources/securescores.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="a9c96-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9c96-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9c96-105">Permissions</span></span>

<span data-ttu-id="a9c96-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9c96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9c96-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9c96-108">Permission type</span></span>      | <span data-ttu-id="a9c96-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9c96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9c96-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9c96-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a9c96-111">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="a9c96-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="a9c96-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9c96-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a9c96-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9c96-113">Not supported.</span></span>  |
|<span data-ttu-id="a9c96-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9c96-114">Application</span></span> | <span data-ttu-id="a9c96-115">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="a9c96-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9c96-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9c96-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="a9c96-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9c96-117">Request headers</span></span>

| <span data-ttu-id="a9c96-118">名前</span><span class="sxs-lookup"><span data-stu-id="a9c96-118">Name</span></span>      |<span data-ttu-id="a9c96-119">説明</span><span class="sxs-lookup"><span data-stu-id="a9c96-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9c96-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9c96-120">Authorization</span></span>  | <span data-ttu-id="a9c96-p102">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="a9c96-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9c96-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9c96-123">Request body</span></span>

<span data-ttu-id="a9c96-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a9c96-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9c96-125">応答</span><span class="sxs-lookup"><span data-stu-id="a9c96-125">Response</span></span>

<span data-ttu-id="a9c96-126">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**secureScores**オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a9c96-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9c96-127">例</span><span class="sxs-lookup"><span data-stu-id="a9c96-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9c96-128">要求</span><span class="sxs-lookup"><span data-stu-id="a9c96-128">Request</span></span>

<span data-ttu-id="a9c96-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a9c96-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="a9c96-130">応答</span><span class="sxs-lookup"><span data-stu-id="a9c96-130">Response</span></span>

<span data-ttu-id="a9c96-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a9c96-131">The following is an example of the response.</span></span>
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
