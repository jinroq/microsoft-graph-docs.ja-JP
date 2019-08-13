---
title: 同期ジョブを取得する
description: 既存の同期ジョブとそのプロパティを取得します。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 72411858f8faee96b1bdd89e8da6e170d6d16b41
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363565"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="e2603-103">同期ジョブを取得する</span><span class="sxs-lookup"><span data-stu-id="e2603-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2603-104">既存の同期ジョブとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="e2603-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2603-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2603-105">Permissions</span></span>
<span data-ttu-id="e2603-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2603-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2603-108">Permission type</span></span>                        | <span data-ttu-id="e2603-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2603-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2603-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2603-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="e2603-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2603-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e2603-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2603-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e2603-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2603-113">Not supported.</span></span>  |
|<span data-ttu-id="e2603-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2603-114">Application</span></span>                            |<span data-ttu-id="e2603-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2603-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e2603-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2603-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="e2603-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2603-117">Request headers</span></span>

| <span data-ttu-id="e2603-118">名前</span><span class="sxs-lookup"><span data-stu-id="e2603-118">Name</span></span>           | <span data-ttu-id="e2603-119">型</span><span class="sxs-lookup"><span data-stu-id="e2603-119">Type</span></span>    | <span data-ttu-id="e2603-120">説明</span><span class="sxs-lookup"><span data-stu-id="e2603-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e2603-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2603-121">Authorization</span></span>  | <span data-ttu-id="e2603-122">string</span><span class="sxs-lookup"><span data-stu-id="e2603-122">string</span></span>  | <span data-ttu-id="e2603-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2603-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2603-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2603-125">Request body</span></span>

<span data-ttu-id="e2603-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2603-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2603-127">応答</span><span class="sxs-lookup"><span data-stu-id="e2603-127">Response</span></span>

<span data-ttu-id="e2603-128">成功した場合は`200 OK` 、応答本文で[同期ジョブ](../resources/synchronization-synchronizationjob.md)を伴う応答を返します。</span><span class="sxs-lookup"><span data-stu-id="e2603-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2603-129">例</span><span class="sxs-lookup"><span data-stu-id="e2603-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2603-130">要求</span><span class="sxs-lookup"><span data-stu-id="e2603-130">Request</span></span>
<span data-ttu-id="e2603-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2603-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2603-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e2603-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2603-133">C#</span><span class="sxs-lookup"><span data-stu-id="e2603-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2603-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2603-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2603-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="e2603-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2603-136">Java</span><span class="sxs-lookup"><span data-stu-id="e2603-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e2603-137">応答</span><span class="sxs-lookup"><span data-stu-id="e2603-137">Response</span></span>
<span data-ttu-id="e2603-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2603-138">The following is an example of a response.</span></span> 

><span data-ttu-id="e2603-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e2603-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
