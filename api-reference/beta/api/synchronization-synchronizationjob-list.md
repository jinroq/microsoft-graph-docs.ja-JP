---
title: 同期ジョブを一覧表示
description: 特定のアプリケーションのインスタンス (サービス主体) の既存のジョブを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 265b1f5a32239173154ef51077d59f3104ad03b3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518962"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="7e5b9-103">同期ジョブを一覧表示</span><span class="sxs-lookup"><span data-stu-id="7e5b9-103">List synchronization jobs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e5b9-104">特定のアプリケーションのインスタンス (サービス主体) の既存のジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-104">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e5b9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7e5b9-105">Permissions</span></span>
<span data-ttu-id="7e5b9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e5b9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e5b9-108">Permission type</span></span>                        | <span data-ttu-id="7e5b9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e5b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e5b9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e5b9-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="7e5b9-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e5b9-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7e5b9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e5b9-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7e5b9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-113">Not supported.</span></span> |
|<span data-ttu-id="7e5b9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e5b9-114">Application</span></span>                            |<span data-ttu-id="7e5b9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7e5b9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e5b9-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="7e5b9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e5b9-117">Request headers</span></span>

| <span data-ttu-id="7e5b9-118">名前</span><span class="sxs-lookup"><span data-stu-id="7e5b9-118">Name</span></span>           | <span data-ttu-id="7e5b9-119">型</span><span class="sxs-lookup"><span data-stu-id="7e5b9-119">Type</span></span>    | <span data-ttu-id="7e5b9-120">説明</span><span class="sxs-lookup"><span data-stu-id="7e5b9-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7e5b9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e5b9-121">Authorization</span></span>  | <span data-ttu-id="7e5b9-122">string</span><span class="sxs-lookup"><span data-stu-id="7e5b9-122">string</span></span>  | <span data-ttu-id="7e5b9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e5b9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e5b9-125">Request body</span></span>

<span data-ttu-id="7e5b9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e5b9-127">応答</span><span class="sxs-lookup"><span data-stu-id="7e5b9-127">Response</span></span>

<span data-ttu-id="7e5b9-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[synchronizationJob](../resources/synchronization-synchronizationjob.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-128">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e5b9-129">例</span><span class="sxs-lookup"><span data-stu-id="7e5b9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e5b9-130">要求</span><span class="sxs-lookup"><span data-stu-id="7e5b9-130">Request</span></span>
<span data-ttu-id="7e5b9-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="7e5b9-132">応答</span><span class="sxs-lookup"><span data-stu-id="7e5b9-132">Response</span></span>
<span data-ttu-id="7e5b9-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-133">The following is an example of a response.</span></span> 

><span data-ttu-id="7e5b9-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7e5b9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
