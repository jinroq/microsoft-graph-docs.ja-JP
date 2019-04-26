---
title: secureScores のリスト
description: secureScores オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: baa4e2e887eb739160105f2ded149481f8a8d0d4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335991"
---
# <a name="list-securescores"></a><span data-ttu-id="7468d-103">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="7468d-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7468d-104">[secureScores](../resources/securescores.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="7468d-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7468d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7468d-105">Permissions</span></span>

<span data-ttu-id="7468d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7468d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7468d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7468d-108">Permission type</span></span>      | <span data-ttu-id="7468d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7468d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7468d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7468d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7468d-111">securityevents。 all、securityevents.。</span><span class="sxs-lookup"><span data-stu-id="7468d-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="7468d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7468d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7468d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7468d-113">Not supported.</span></span>  |
|<span data-ttu-id="7468d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7468d-114">Application</span></span> | <span data-ttu-id="7468d-115">securityevents。 all、securityevents.。</span><span class="sxs-lookup"><span data-stu-id="7468d-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7468d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7468d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="7468d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7468d-117">Request headers</span></span>

| <span data-ttu-id="7468d-118">名前</span><span class="sxs-lookup"><span data-stu-id="7468d-118">Name</span></span>      |<span data-ttu-id="7468d-119">説明</span><span class="sxs-lookup"><span data-stu-id="7468d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7468d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7468d-120">Authorization</span></span>  | <span data-ttu-id="7468d-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="7468d-121">Bearer {code}.</span></span> <span data-ttu-id="7468d-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="7468d-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7468d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7468d-123">Request body</span></span>

<span data-ttu-id="7468d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7468d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7468d-125">応答</span><span class="sxs-lookup"><span data-stu-id="7468d-125">Response</span></span>

<span data-ttu-id="7468d-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**secureScores**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7468d-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7468d-127">例</span><span class="sxs-lookup"><span data-stu-id="7468d-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="7468d-128">要求</span><span class="sxs-lookup"><span data-stu-id="7468d-128">Request</span></span>

<span data-ttu-id="7468d-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7468d-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="7468d-130">応答</span><span class="sxs-lookup"><span data-stu-id="7468d-130">Response</span></span>

<span data-ttu-id="7468d-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7468d-131">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
