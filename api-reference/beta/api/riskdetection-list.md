---
title: リスト riskDetection
description: '**RiskDetection**オブジェクトのコレクションのプロパティを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e019c9c9984ba7bb99b5f10266a333b8f3a07d52
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349422"
---
# <a name="list-riskdetection"></a><span data-ttu-id="f35aa-103">リスト riskDetection</span><span class="sxs-lookup"><span data-stu-id="f35aa-103">List riskDetection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f35aa-104">**RiskDetection**オブジェクトのコレクションのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="f35aa-104">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="f35aa-105">リスク検出 API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="f35aa-105">You must have an Azure AD Premium P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="f35aa-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f35aa-106">Permissions</span></span>

<span data-ttu-id="f35aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f35aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f35aa-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f35aa-109">Permission type</span></span>      | <span data-ttu-id="f35aa-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f35aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f35aa-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f35aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f35aa-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="f35aa-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="f35aa-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f35aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f35aa-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f35aa-114">Not supported.</span></span>    |
|<span data-ttu-id="f35aa-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f35aa-115">Application</span></span> | <span data-ttu-id="f35aa-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="f35aa-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f35aa-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f35aa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f35aa-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f35aa-118">Optional query parameters</span></span>

<span data-ttu-id="f35aa-119">このメソッドは`$filter` 、 `$select`クエリの応答をサポートし、カスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="f35aa-119">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="f35aa-120">このトピックの後半の例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f35aa-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="f35aa-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f35aa-121">Request headers</span></span>

| <span data-ttu-id="f35aa-122">名前</span><span class="sxs-lookup"><span data-stu-id="f35aa-122">Name</span></span>      |<span data-ttu-id="f35aa-123">説明</span><span class="sxs-lookup"><span data-stu-id="f35aa-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f35aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f35aa-124">Authorization</span></span>  | <span data-ttu-id="f35aa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f35aa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f35aa-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f35aa-127">Content-Type</span></span> | <span data-ttu-id="f35aa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f35aa-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f35aa-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f35aa-129">Request body</span></span>

<span data-ttu-id="f35aa-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f35aa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f35aa-131">応答</span><span class="sxs-lookup"><span data-stu-id="f35aa-131">Response</span></span>

<span data-ttu-id="f35aa-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskDetection](../resources/riskDetection.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f35aa-132">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskDetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f35aa-133">例</span><span class="sxs-lookup"><span data-stu-id="f35aa-133">Examples</span></span>

### <a name="example-1-list-risk-detections"></a><span data-ttu-id="f35aa-134">例 1: リスクの検出を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f35aa-134">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="f35aa-135">要求</span><span class="sxs-lookup"><span data-stu-id="f35aa-135">Request</span></span>

<span data-ttu-id="f35aa-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f35aa-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```http
GET https://graph.microsoft.com/beta/riskDetections
```

#### <a name="response"></a><span data-ttu-id="f35aa-137">応答</span><span class="sxs-lookup"><span data-stu-id="f35aa-137">Response</span></span>

<span data-ttu-id="f35aa-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f35aa-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
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
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

### <a name="example-2-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="f35aa-139">例 2: リスクを検出して結果をフィルター処理する</span><span class="sxs-lookup"><span data-stu-id="f35aa-139">Example 2: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="f35aa-140">要求</span><span class="sxs-lookup"><span data-stu-id="f35aa-140">Request</span></span>

<span data-ttu-id="f35aa-141">次の例は、を使用`$filter`してリスクレベルが中、またはリスクイベントの種類が unfamilarFeatures であるというリスクの検出のコレクションを取得する方法を示しています。これは、未知または異常な場所にサインインしていたことを示します。</span><span class="sxs-lookup"><span data-stu-id="f35aa-141">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```http
GET https://graph.microsoft.com/beta/riskDetections?$filter=riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```

#### <a name="response"></a><span data-ttu-id="f35aa-142">応答</span><span class="sxs-lookup"><span data-stu-id="f35aa-142">Response</span></span>

<span data-ttu-id="f35aa-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f35aa-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
    "id": "1d68fc3d60d012ff80ad4b16818bf304df1bde295fdf1db31fa5389ba9532cd1",
    "requestId": "3295073e-04b1-4871-9d15-c1f871b41100",
    "correlationId": "f141d8e5-93e9-4fd0-9eb0-c40e5f8fc092",
    "riskType": "unfamiliarFeatures",
    "riskState": "atRisk",
    "riskLevel": "medium",
    "riskDetail": "none",
    "source": "Identity Protection",
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
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskDetections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
