---
title: SynchronizationJob を取得します。
description: 既存の同期ジョブおよびそのプロパティを取得します。
ms.openlocfilehash: c0c999d5b9ce168ba3f21af20ec5cff026d68f8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073972"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="74eaf-103">SynchronizationJob を取得します。</span><span class="sxs-lookup"><span data-stu-id="74eaf-103">Get synchronizationJob</span></span>

> <span data-ttu-id="74eaf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="74eaf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74eaf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74eaf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74eaf-106">既存の同期ジョブおよびそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="74eaf-106">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="74eaf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74eaf-107">Permissions</span></span>
<span data-ttu-id="74eaf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74eaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74eaf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74eaf-110">Permission type</span></span>                        | <span data-ttu-id="74eaf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74eaf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="74eaf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74eaf-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="74eaf-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74eaf-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="74eaf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74eaf-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="74eaf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74eaf-115">Not supported.</span></span>  |
|<span data-ttu-id="74eaf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74eaf-116">Application</span></span>                            |<span data-ttu-id="74eaf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74eaf-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="74eaf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74eaf-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="74eaf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74eaf-119">Request headers</span></span>

| <span data-ttu-id="74eaf-120">名前</span><span class="sxs-lookup"><span data-stu-id="74eaf-120">Name</span></span>           | <span data-ttu-id="74eaf-121">型</span><span class="sxs-lookup"><span data-stu-id="74eaf-121">Type</span></span>    | <span data-ttu-id="74eaf-122">説明</span><span class="sxs-lookup"><span data-stu-id="74eaf-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="74eaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74eaf-123">Authorization</span></span>  | <span data-ttu-id="74eaf-124">string</span><span class="sxs-lookup"><span data-stu-id="74eaf-124">string</span></span>  | <span data-ttu-id="74eaf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74eaf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74eaf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="74eaf-127">Request body</span></span>

<span data-ttu-id="74eaf-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="74eaf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74eaf-129">応答</span><span class="sxs-lookup"><span data-stu-id="74eaf-129">Response</span></span>

<span data-ttu-id="74eaf-130">成功した場合に返されます、`200 OK`応答本体には、 [synchronizationJob](../resources/synchronization-synchronizationjob.md)に対応します。</span><span class="sxs-lookup"><span data-stu-id="74eaf-130">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74eaf-131">例</span><span class="sxs-lookup"><span data-stu-id="74eaf-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="74eaf-132">要求</span><span class="sxs-lookup"><span data-stu-id="74eaf-132">Request</span></span>
<span data-ttu-id="74eaf-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74eaf-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="74eaf-134">応答</span><span class="sxs-lookup"><span data-stu-id="74eaf-134">Response</span></span>
<span data-ttu-id="74eaf-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74eaf-135">The following is an example of a response.</span></span> 

><span data-ttu-id="74eaf-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="74eaf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->