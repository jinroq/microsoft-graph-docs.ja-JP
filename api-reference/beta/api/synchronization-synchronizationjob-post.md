---
title: SynchronizationJob を作成します。
description: 既定同期スキーマに新しい同期ジョブを作成します。 ジョブが無効の状態で作成されます。 呼び出し同期を開始するジョブを開始します。
localization_priority: Normal
ms.openlocfilehash: f41ebe87d8ca935a355c37ea53d1c7bd62b1652e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507916"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="85198-105">SynchronizationJob を作成します。</span><span class="sxs-lookup"><span data-stu-id="85198-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85198-106">既定同期スキーマに新しい同期ジョブを作成します。</span><span class="sxs-lookup"><span data-stu-id="85198-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="85198-107">ジョブが無効の状態で作成されます。</span><span class="sxs-lookup"><span data-stu-id="85198-107">The job is created in a disabled state.</span></span> <span data-ttu-id="85198-108">同期を開始する[ジョブを開始する](synchronization-synchronizationjob-start.md)を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="85198-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="85198-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="85198-109">Permissions</span></span>
<span data-ttu-id="85198-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85198-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85198-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85198-112">Permission type</span></span>                        | <span data-ttu-id="85198-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="85198-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="85198-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85198-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="85198-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85198-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="85198-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85198-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="85198-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85198-117">Not supported.</span></span>|
|<span data-ttu-id="85198-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85198-118">Application</span></span>                            |<span data-ttu-id="85198-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85198-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="85198-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85198-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="85198-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85198-121">Request headers</span></span>

| <span data-ttu-id="85198-122">名前</span><span class="sxs-lookup"><span data-stu-id="85198-122">Name</span></span>           | <span data-ttu-id="85198-123">型</span><span class="sxs-lookup"><span data-stu-id="85198-123">Type</span></span>    | <span data-ttu-id="85198-124">説明</span><span class="sxs-lookup"><span data-stu-id="85198-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="85198-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="85198-125">Authorization</span></span>  | <span data-ttu-id="85198-126">string</span><span class="sxs-lookup"><span data-stu-id="85198-126">string</span></span>  | <span data-ttu-id="85198-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="85198-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85198-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="85198-129">Request body</span></span>

<span data-ttu-id="85198-130">要求の本文には、 [synchronizationJob](../resources/synchronization-synchronizationjob.md)オブジェクトを作成するのに JSON 形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="85198-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="85198-131">唯一必要なプロパティは、 `templateId`。</span><span class="sxs-lookup"><span data-stu-id="85198-131">The only required property is `templateId`.</span></span> <span data-ttu-id="85198-132">`templateId`プロパティで、このアプリケーション、およびサービス プリンシパル用に作成されたテンプレートのいずれかと一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="85198-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="85198-133">使用可能なテンプレートを検索するには、[リスト テンプレート](synchronization-synchronizationtemplate-list.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="85198-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="85198-134">応答</span><span class="sxs-lookup"><span data-stu-id="85198-134">Response</span></span>

<span data-ttu-id="85198-135">正常終了した場合、`201 Created`応答コードおよび応答の本文に[synchronizationJob](../resources/synchronization-synchronizationjob.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="85198-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85198-136">例</span><span class="sxs-lookup"><span data-stu-id="85198-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85198-137">要求</span><span class="sxs-lookup"><span data-stu-id="85198-137">Request</span></span>
<span data-ttu-id="85198-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85198-138">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "BoxOutDelta"
}
```

##### <a name="response"></a><span data-ttu-id="85198-139">応答</span><span class="sxs-lookup"><span data-stu-id="85198-139">Response</span></span>
<span data-ttu-id="85198-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85198-140">The following is an example of a response.</span></span> 

><span data-ttu-id="85198-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="85198-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
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
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
