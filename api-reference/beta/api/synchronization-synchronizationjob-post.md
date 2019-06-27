---
title: 同期ジョブの作成
description: 既定の同期スキーマを使用して、新しい同期ジョブを作成します。 ジョブは無効な状態で作成されます。 Start ジョブを呼び出して同期を開始します。
localization_priority: Normal
ms.openlocfilehash: 342364d9b3a2213c2ffdb686c9349700471a84da
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271352"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="45c18-105">同期ジョブの作成</span><span class="sxs-lookup"><span data-stu-id="45c18-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45c18-106">既定の同期スキーマを使用して、新しい同期ジョブを作成します。</span><span class="sxs-lookup"><span data-stu-id="45c18-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="45c18-107">ジョブは無効な状態で作成されます。</span><span class="sxs-lookup"><span data-stu-id="45c18-107">The job is created in a disabled state.</span></span> <span data-ttu-id="45c18-108">[Start ジョブ](synchronization-synchronizationjob-start.md)を呼び出して同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="45c18-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="45c18-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="45c18-109">Permissions</span></span>
<span data-ttu-id="45c18-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45c18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c18-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45c18-112">Permission type</span></span>                        | <span data-ttu-id="45c18-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="45c18-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="45c18-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45c18-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="45c18-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c18-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="45c18-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45c18-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="45c18-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45c18-117">Not supported.</span></span>|
|<span data-ttu-id="45c18-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45c18-118">Application</span></span>                            |<span data-ttu-id="45c18-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45c18-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="45c18-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45c18-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="45c18-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45c18-121">Request headers</span></span>

| <span data-ttu-id="45c18-122">名前</span><span class="sxs-lookup"><span data-stu-id="45c18-122">Name</span></span>           | <span data-ttu-id="45c18-123">型</span><span class="sxs-lookup"><span data-stu-id="45c18-123">Type</span></span>    | <span data-ttu-id="45c18-124">説明</span><span class="sxs-lookup"><span data-stu-id="45c18-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="45c18-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="45c18-125">Authorization</span></span>  | <span data-ttu-id="45c18-126">string</span><span class="sxs-lookup"><span data-stu-id="45c18-126">string</span></span>  | <span data-ttu-id="45c18-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="45c18-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45c18-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="45c18-129">Request body</span></span>

<span data-ttu-id="45c18-130">要求本文で、作成する[同期ジョブ](../resources/synchronization-synchronizationjob.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="45c18-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="45c18-131">唯一必要なプロパティは`templateId`です。</span><span class="sxs-lookup"><span data-stu-id="45c18-131">The only required property is `templateId`.</span></span> <span data-ttu-id="45c18-132">この`templateId`プロパティは、このアプリケーション/サービスプリンシパルに対して作成されたテンプレートのいずれかと一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="45c18-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="45c18-133">利用可能なテンプレートを検索するには、[[リストテンプレート](synchronization-synchronizationtemplate-list.md)] を使用します。</span><span class="sxs-lookup"><span data-stu-id="45c18-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="45c18-134">応答</span><span class="sxs-lookup"><span data-stu-id="45c18-134">Response</span></span>

<span data-ttu-id="45c18-135">成功した場合は`201 Created` 、応答コードと、応答本文で[同期ジョブ](../resources/synchronization-synchronizationjob.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="45c18-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45c18-136">例</span><span class="sxs-lookup"><span data-stu-id="45c18-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="45c18-137">要求</span><span class="sxs-lookup"><span data-stu-id="45c18-137">Request</span></span>
<span data-ttu-id="45c18-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="45c18-138">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="45c18-139">応答</span><span class="sxs-lookup"><span data-stu-id="45c18-139">Response</span></span>
<span data-ttu-id="45c18-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="45c18-140">The following is an example of a response.</span></span> 

><span data-ttu-id="45c18-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="45c18-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="45c18-143">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="45c18-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="45c18-144">C#</span><span class="sxs-lookup"><span data-stu-id="45c18-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45c18-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="45c18-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="45c18-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="45c18-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
