---
title: 同期ジョブの作成
description: 既定の同期スキーマを使用して、新しい同期ジョブを作成します。 ジョブは無効な状態で作成されます。 Start ジョブを呼び出して同期を開始します。
localization_priority: Normal
ms.openlocfilehash: fa0c3e539d73ff9496a0d4d0e3af8ebeda75e839
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638033"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="d11e0-105">同期ジョブの作成</span><span class="sxs-lookup"><span data-stu-id="d11e0-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d11e0-106">既定の同期スキーマを使用して、新しい同期ジョブを作成します。</span><span class="sxs-lookup"><span data-stu-id="d11e0-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="d11e0-107">ジョブは無効な状態で作成されます。</span><span class="sxs-lookup"><span data-stu-id="d11e0-107">The job is created in a disabled state.</span></span> <span data-ttu-id="d11e0-108">[Start ジョブ](synchronization-synchronizationjob-start.md)を呼び出して同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="d11e0-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="d11e0-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d11e0-109">Permissions</span></span>
<span data-ttu-id="d11e0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d11e0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d11e0-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d11e0-112">Permission type</span></span>                        | <span data-ttu-id="d11e0-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d11e0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d11e0-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d11e0-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="d11e0-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d11e0-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d11e0-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d11e0-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d11e0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d11e0-117">Not supported.</span></span>|
|<span data-ttu-id="d11e0-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d11e0-118">Application</span></span>                            |<span data-ttu-id="d11e0-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d11e0-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="d11e0-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d11e0-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="d11e0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d11e0-121">Request headers</span></span>

| <span data-ttu-id="d11e0-122">名前</span><span class="sxs-lookup"><span data-stu-id="d11e0-122">Name</span></span>           | <span data-ttu-id="d11e0-123">型</span><span class="sxs-lookup"><span data-stu-id="d11e0-123">Type</span></span>    | <span data-ttu-id="d11e0-124">説明</span><span class="sxs-lookup"><span data-stu-id="d11e0-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d11e0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d11e0-125">Authorization</span></span>  | <span data-ttu-id="d11e0-126">string</span><span class="sxs-lookup"><span data-stu-id="d11e0-126">string</span></span>  | <span data-ttu-id="d11e0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d11e0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d11e0-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d11e0-129">Request body</span></span>

<span data-ttu-id="d11e0-130">要求本文で、作成する[同期ジョブ](../resources/synchronization-synchronizationjob.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d11e0-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="d11e0-131">唯一必要なプロパティは`templateId`です。</span><span class="sxs-lookup"><span data-stu-id="d11e0-131">The only required property is `templateId`.</span></span> <span data-ttu-id="d11e0-132">この`templateId`プロパティは、このアプリケーション/サービスプリンシパルに対して作成されたテンプレートのいずれかと一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="d11e0-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="d11e0-133">利用可能なテンプレートを検索するには、[[リストテンプレート](synchronization-synchronizationtemplate-list.md)] を使用します。</span><span class="sxs-lookup"><span data-stu-id="d11e0-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="d11e0-134">応答</span><span class="sxs-lookup"><span data-stu-id="d11e0-134">Response</span></span>

<span data-ttu-id="d11e0-135">成功した場合は`201 Created` 、応答コードと、応答本文で[同期ジョブ](../resources/synchronization-synchronizationjob.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d11e0-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d11e0-136">例</span><span class="sxs-lookup"><span data-stu-id="d11e0-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d11e0-137">要求</span><span class="sxs-lookup"><span data-stu-id="d11e0-137">Request</span></span>
<span data-ttu-id="d11e0-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d11e0-138">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d11e0-139">応答</span><span class="sxs-lookup"><span data-stu-id="d11e0-139">Response</span></span>
<span data-ttu-id="d11e0-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d11e0-140">The following is an example of a response.</span></span> 

><span data-ttu-id="d11e0-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d11e0-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d11e0-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d11e0-142">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d11e0-143">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="d11e0-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d11e0-144">Visual</span><span class="sxs-lookup"><span data-stu-id="d11e0-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d11e0-145">Java</span><span class="sxs-lookup"><span data-stu-id="d11e0-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
