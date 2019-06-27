---
title: 同期ジョブを一覧表示する
description: 特定のアプリケーションインスタンス (サービスプリンシパル) の既存のジョブを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 8c6f03805ce359669870c61c608a8181f7bf7338
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271373"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="443e0-103">同期ジョブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="443e0-103">List synchronization jobs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="443e0-104">特定のアプリケーションインスタンス (サービスプリンシパル) の既存のジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="443e0-104">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="443e0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="443e0-105">Permissions</span></span>
<span data-ttu-id="443e0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="443e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="443e0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="443e0-108">Permission type</span></span>                        | <span data-ttu-id="443e0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="443e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="443e0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="443e0-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="443e0-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="443e0-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="443e0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="443e0-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="443e0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="443e0-113">Not supported.</span></span> |
|<span data-ttu-id="443e0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="443e0-114">Application</span></span>                            |<span data-ttu-id="443e0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="443e0-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="443e0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="443e0-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="443e0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="443e0-117">Request headers</span></span>

| <span data-ttu-id="443e0-118">名前</span><span class="sxs-lookup"><span data-stu-id="443e0-118">Name</span></span>           | <span data-ttu-id="443e0-119">型</span><span class="sxs-lookup"><span data-stu-id="443e0-119">Type</span></span>    | <span data-ttu-id="443e0-120">説明</span><span class="sxs-lookup"><span data-stu-id="443e0-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="443e0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="443e0-121">Authorization</span></span>  | <span data-ttu-id="443e0-122">string</span><span class="sxs-lookup"><span data-stu-id="443e0-122">string</span></span>  | <span data-ttu-id="443e0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="443e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="443e0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="443e0-125">Request body</span></span>

<span data-ttu-id="443e0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="443e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="443e0-127">応答</span><span class="sxs-lookup"><span data-stu-id="443e0-127">Response</span></span>

<span data-ttu-id="443e0-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期ジョブ](../resources/synchronization-synchronizationjob.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="443e0-128">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443e0-129">例</span><span class="sxs-lookup"><span data-stu-id="443e0-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="443e0-130">要求</span><span class="sxs-lookup"><span data-stu-id="443e0-130">Request</span></span>
<span data-ttu-id="443e0-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="443e0-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="443e0-132">応答</span><span class="sxs-lookup"><span data-stu-id="443e0-132">Response</span></span>
<span data-ttu-id="443e0-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="443e0-133">The following is an example of a response.</span></span> 

><span data-ttu-id="443e0-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="443e0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="443e0-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="443e0-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="443e0-137">C#</span><span class="sxs-lookup"><span data-stu-id="443e0-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_jobs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="443e0-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="443e0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_jobs-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="443e0-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="443e0-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_jobs-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
