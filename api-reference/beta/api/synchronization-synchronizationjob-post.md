---
title: SynchronizationJob を作成します。
description: 既定同期スキーマに新しい同期ジョブを作成します。 ジョブが無効の状態で作成されます。 呼び出し同期を開始するジョブを開始します。
localization_priority: Normal
ms.openlocfilehash: 04b8e383c923968b150067c9d2c3a65ce32bd9c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842225"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="483a3-105">SynchronizationJob を作成します。</span><span class="sxs-lookup"><span data-stu-id="483a3-105">Create synchronizationJob</span></span>

> <span data-ttu-id="483a3-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="483a3-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="483a3-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="483a3-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="483a3-108">既定同期スキーマに新しい同期ジョブを作成します。</span><span class="sxs-lookup"><span data-stu-id="483a3-108">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="483a3-109">ジョブが無効の状態で作成されます。</span><span class="sxs-lookup"><span data-stu-id="483a3-109">The job is created in a disabled state.</span></span> <span data-ttu-id="483a3-110">同期を開始する[ジョブを開始する](synchronization-synchronizationjob-start.md)を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="483a3-110">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="483a3-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="483a3-111">Permissions</span></span>
<span data-ttu-id="483a3-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="483a3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="483a3-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="483a3-114">Permission type</span></span>                        | <span data-ttu-id="483a3-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="483a3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="483a3-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="483a3-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="483a3-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483a3-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="483a3-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="483a3-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="483a3-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="483a3-119">Not supported.</span></span>|
|<span data-ttu-id="483a3-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="483a3-120">Application</span></span>                            |<span data-ttu-id="483a3-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="483a3-121">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="483a3-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="483a3-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="483a3-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="483a3-123">Request headers</span></span>

| <span data-ttu-id="483a3-124">名前</span><span class="sxs-lookup"><span data-stu-id="483a3-124">Name</span></span>           | <span data-ttu-id="483a3-125">種類</span><span class="sxs-lookup"><span data-stu-id="483a3-125">Type</span></span>    | <span data-ttu-id="483a3-126">説明</span><span class="sxs-lookup"><span data-stu-id="483a3-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="483a3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="483a3-127">Authorization</span></span>  | <span data-ttu-id="483a3-128">string</span><span class="sxs-lookup"><span data-stu-id="483a3-128">string</span></span>  | <span data-ttu-id="483a3-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="483a3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="483a3-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="483a3-131">Request body</span></span>

<span data-ttu-id="483a3-132">要求の本文には、 [synchronizationJob](../resources/synchronization-synchronizationjob.md)オブジェクトを作成するのに JSON 形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="483a3-132">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="483a3-133">唯一必要なプロパティは、 `templateId`。</span><span class="sxs-lookup"><span data-stu-id="483a3-133">The only required property is `templateId`.</span></span> <span data-ttu-id="483a3-134">`templateId`プロパティで、このアプリケーション、およびサービス プリンシパル用に作成されたテンプレートのいずれかと一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="483a3-134">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="483a3-135">使用可能なテンプレートを検索するには、[リスト テンプレート](synchronization-synchronizationtemplate-list.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="483a3-135">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="483a3-136">応答</span><span class="sxs-lookup"><span data-stu-id="483a3-136">Response</span></span>

<span data-ttu-id="483a3-137">正常終了した場合、`201 Created`応答コードおよび応答の本文に[synchronizationJob](../resources/synchronization-synchronizationjob.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="483a3-137">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="483a3-138">例</span><span class="sxs-lookup"><span data-stu-id="483a3-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="483a3-139">要求</span><span class="sxs-lookup"><span data-stu-id="483a3-139">Request</span></span>
<span data-ttu-id="483a3-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="483a3-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="483a3-141">応答</span><span class="sxs-lookup"><span data-stu-id="483a3-141">Response</span></span>
<span data-ttu-id="483a3-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="483a3-142">The following is an example of a response.</span></span> 

><span data-ttu-id="483a3-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="483a3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
