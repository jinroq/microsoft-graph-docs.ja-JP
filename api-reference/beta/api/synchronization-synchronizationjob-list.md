---
title: 同期ジョブを一覧表示
description: 特定のアプリケーションのインスタンス (サービス主体) の既存のジョブを一覧表示します。
ms.openlocfilehash: 179a6906936fddbfc31ffc7b016de05908f2383a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072898"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="1e90c-103">同期ジョブを一覧表示</span><span class="sxs-lookup"><span data-stu-id="1e90c-103">List synchronization jobs</span></span>

> <span data-ttu-id="1e90c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e90c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e90c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e90c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e90c-106">特定のアプリケーションのインスタンス (サービス主体) の既存のジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1e90c-106">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e90c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e90c-107">Permissions</span></span>
<span data-ttu-id="1e90c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e90c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e90c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e90c-110">Permission type</span></span>                        | <span data-ttu-id="1e90c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e90c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e90c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e90c-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="1e90c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e90c-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1e90c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e90c-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1e90c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e90c-115">Not supported.</span></span> |
|<span data-ttu-id="1e90c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e90c-116">Application</span></span>                            |<span data-ttu-id="1e90c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e90c-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1e90c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e90c-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="1e90c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e90c-119">Request headers</span></span>

| <span data-ttu-id="1e90c-120">名前</span><span class="sxs-lookup"><span data-stu-id="1e90c-120">Name</span></span>           | <span data-ttu-id="1e90c-121">型</span><span class="sxs-lookup"><span data-stu-id="1e90c-121">Type</span></span>    | <span data-ttu-id="1e90c-122">説明</span><span class="sxs-lookup"><span data-stu-id="1e90c-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1e90c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e90c-123">Authorization</span></span>  | <span data-ttu-id="1e90c-124">string</span><span class="sxs-lookup"><span data-stu-id="1e90c-124">string</span></span>  | <span data-ttu-id="1e90c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e90c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e90c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e90c-127">Request body</span></span>

<span data-ttu-id="1e90c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e90c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e90c-129">応答</span><span class="sxs-lookup"><span data-stu-id="1e90c-129">Response</span></span>

<span data-ttu-id="1e90c-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[synchronizationJob](../resources/synchronization-synchronizationjob.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1e90c-130">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e90c-131">例</span><span class="sxs-lookup"><span data-stu-id="1e90c-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1e90c-132">要求</span><span class="sxs-lookup"><span data-stu-id="1e90c-132">Request</span></span>
<span data-ttu-id="1e90c-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e90c-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="1e90c-134">応答</span><span class="sxs-lookup"><span data-stu-id="1e90c-134">Response</span></span>
<span data-ttu-id="1e90c-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e90c-135">The following is an example of a response.</span></span> 

><span data-ttu-id="1e90c-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e90c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2958

{
    "value": [
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
                "lastSuccessfulExecutionWithExports": null,
                "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
                "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
                "quarantine": null,
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->