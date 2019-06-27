---
title: '同期ジョブ: 一時停止'
description: 一時的に同期を停止します。 ジョブの状態を含むすべての進行状況が持続され、開始呼び出しが行われたときにジョブは中断したところから続行されます。
localization_priority: Normal
ms.openlocfilehash: e80e629f7d592517ccb680610d16ce9433967baa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271359"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="80b3a-104">同期ジョブ: 一時停止</span><span class="sxs-lookup"><span data-stu-id="80b3a-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80b3a-105">一時的に同期を停止します。</span><span class="sxs-lookup"><span data-stu-id="80b3a-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="80b3a-106">ジョブの状態を含むすべての進行状況が持続され、[開始](../api/synchronization-synchronizationjob-start.md)呼び出しが行われたときにジョブは中断したところから続行されます。</span><span class="sxs-lookup"><span data-stu-id="80b3a-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="80b3a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80b3a-107">Permissions</span></span>
<span data-ttu-id="80b3a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80b3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80b3a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80b3a-110">Permission type</span></span>                        | <span data-ttu-id="80b3a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80b3a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="80b3a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80b3a-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="80b3a-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80b3a-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="80b3a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80b3a-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="80b3a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80b3a-115">Not supported.</span></span>  |
|<span data-ttu-id="80b3a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80b3a-116">Application</span></span>                            |<span data-ttu-id="80b3a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80b3a-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="80b3a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80b3a-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="80b3a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80b3a-119">Request headers</span></span>

| <span data-ttu-id="80b3a-120">名前</span><span class="sxs-lookup"><span data-stu-id="80b3a-120">Name</span></span>           | <span data-ttu-id="80b3a-121">型</span><span class="sxs-lookup"><span data-stu-id="80b3a-121">Type</span></span>    | <span data-ttu-id="80b3a-122">説明</span><span class="sxs-lookup"><span data-stu-id="80b3a-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="80b3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80b3a-123">Authorization</span></span>  | <span data-ttu-id="80b3a-124">string</span><span class="sxs-lookup"><span data-stu-id="80b3a-124">string</span></span>  | <span data-ttu-id="80b3a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="80b3a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80b3a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="80b3a-127">Request body</span></span>

<span data-ttu-id="80b3a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="80b3a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80b3a-129">応答</span><span class="sxs-lookup"><span data-stu-id="80b3a-129">Response</span></span>

<span data-ttu-id="80b3a-130">成功した場合は`204 No Content` 、応答を返します。</span><span class="sxs-lookup"><span data-stu-id="80b3a-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="80b3a-131">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="80b3a-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80b3a-132">例</span><span class="sxs-lookup"><span data-stu-id="80b3a-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="80b3a-133">要求</span><span class="sxs-lookup"><span data-stu-id="80b3a-133">Request</span></span>
<span data-ttu-id="80b3a-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="80b3a-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="80b3a-135">応答</span><span class="sxs-lookup"><span data-stu-id="80b3a-135">Response</span></span>
<span data-ttu-id="80b3a-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="80b3a-136">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="80b3a-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="80b3a-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="80b3a-138">C#</span><span class="sxs-lookup"><span data-stu-id="80b3a-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_pause-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80b3a-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="80b3a-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_pause-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="80b3a-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="80b3a-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/synchronizationjob_pause-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
