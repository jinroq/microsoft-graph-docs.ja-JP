---
title: 'synchronizationJob: 一時停止'
description: 同期を一時的に停止します。 ジョブの状態を含むすべての進捗が保持され、ジョブが開始の呼び出しが行われる場合停止した位置から続行されます。
localization_priority: Normal
ms.openlocfilehash: f39b3a700b31169ea15f089da8873b517b50dc15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804880"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="8d396-104">synchronizationJob: 一時停止</span><span class="sxs-lookup"><span data-stu-id="8d396-104">synchronizationJob: pause</span></span>

> <span data-ttu-id="8d396-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8d396-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d396-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d396-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d396-107">同期を一時的に停止します。</span><span class="sxs-lookup"><span data-stu-id="8d396-107">Temporarily stop synchronization.</span></span> <span data-ttu-id="8d396-108">ジョブの状態を含むすべての進捗が保持され、ジョブが[起動](../api/synchronization-synchronizationjob-start.md)の呼び出しが行われる場合停止した位置から続行されます。</span><span class="sxs-lookup"><span data-stu-id="8d396-108">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d396-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d396-109">Permissions</span></span>
<span data-ttu-id="8d396-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d396-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d396-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d396-112">Permission type</span></span>                        | <span data-ttu-id="8d396-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d396-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d396-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d396-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="8d396-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d396-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8d396-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d396-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8d396-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d396-117">Not supported.</span></span>  |
|<span data-ttu-id="8d396-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d396-118">Application</span></span>                            |<span data-ttu-id="8d396-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d396-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8d396-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d396-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="8d396-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d396-121">Request headers</span></span>

| <span data-ttu-id="8d396-122">名前</span><span class="sxs-lookup"><span data-stu-id="8d396-122">Name</span></span>           | <span data-ttu-id="8d396-123">種類</span><span class="sxs-lookup"><span data-stu-id="8d396-123">Type</span></span>    | <span data-ttu-id="8d396-124">説明</span><span class="sxs-lookup"><span data-stu-id="8d396-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8d396-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d396-125">Authorization</span></span>  | <span data-ttu-id="8d396-126">string</span><span class="sxs-lookup"><span data-stu-id="8d396-126">string</span></span>  | <span data-ttu-id="8d396-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8d396-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d396-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d396-129">Request body</span></span>

<span data-ttu-id="8d396-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8d396-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d396-131">応答</span><span class="sxs-lookup"><span data-stu-id="8d396-131">Response</span></span>

<span data-ttu-id="8d396-132">正常終了した場合、`204 No Content`応答します。</span><span class="sxs-lookup"><span data-stu-id="8d396-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="8d396-133">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="8d396-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d396-134">例</span><span class="sxs-lookup"><span data-stu-id="8d396-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8d396-135">要求</span><span class="sxs-lookup"><span data-stu-id="8d396-135">Request</span></span>
<span data-ttu-id="8d396-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d396-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="8d396-137">応答</span><span class="sxs-lookup"><span data-stu-id="8d396-137">Response</span></span>
<span data-ttu-id="8d396-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d396-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
