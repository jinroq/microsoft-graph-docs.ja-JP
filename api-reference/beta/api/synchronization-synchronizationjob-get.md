---
title: SynchronizationJob を取得します。
description: 既存の同期ジョブおよびそのプロパティを取得します。
localization_priority: Normal
ms.openlocfilehash: bb7c61192b165e5d05c0bb3434488ed2ff7ee8c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521692"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="9af72-103">SynchronizationJob を取得します。</span><span class="sxs-lookup"><span data-stu-id="9af72-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9af72-104">既存の同期ジョブおよびそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="9af72-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="9af72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9af72-105">Permissions</span></span>
<span data-ttu-id="9af72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9af72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9af72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9af72-108">Permission type</span></span>                        | <span data-ttu-id="9af72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9af72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9af72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9af72-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="9af72-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9af72-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9af72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9af72-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9af72-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9af72-113">Not supported.</span></span>  |
|<span data-ttu-id="9af72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9af72-114">Application</span></span>                            |<span data-ttu-id="9af72-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9af72-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9af72-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9af72-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="9af72-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9af72-117">Request headers</span></span>

| <span data-ttu-id="9af72-118">名前</span><span class="sxs-lookup"><span data-stu-id="9af72-118">Name</span></span>           | <span data-ttu-id="9af72-119">型</span><span class="sxs-lookup"><span data-stu-id="9af72-119">Type</span></span>    | <span data-ttu-id="9af72-120">説明</span><span class="sxs-lookup"><span data-stu-id="9af72-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="9af72-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9af72-121">Authorization</span></span>  | <span data-ttu-id="9af72-122">string</span><span class="sxs-lookup"><span data-stu-id="9af72-122">string</span></span>  | <span data-ttu-id="9af72-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9af72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9af72-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9af72-125">Request body</span></span>

<span data-ttu-id="9af72-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9af72-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9af72-127">応答</span><span class="sxs-lookup"><span data-stu-id="9af72-127">Response</span></span>

<span data-ttu-id="9af72-128">成功した場合に返されます、`200 OK`応答本体には、 [synchronizationJob](../resources/synchronization-synchronizationjob.md)に対応します。</span><span class="sxs-lookup"><span data-stu-id="9af72-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9af72-129">例</span><span class="sxs-lookup"><span data-stu-id="9af72-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9af72-130">要求</span><span class="sxs-lookup"><span data-stu-id="9af72-130">Request</span></span>
<span data-ttu-id="9af72-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9af72-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="9af72-132">応答</span><span class="sxs-lookup"><span data-stu-id="9af72-132">Response</span></span>
<span data-ttu-id="9af72-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9af72-133">The following is an example of a response.</span></span> 

><span data-ttu-id="9af72-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9af72-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2577

{
    "id": "{jobId}",
    "templateId": "BoxOutDelta",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "Paused",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "progress": [],
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
