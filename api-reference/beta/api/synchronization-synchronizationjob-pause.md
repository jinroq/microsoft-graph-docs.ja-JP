---
title: 'synchronizationJob: 一時停止'
description: 同期を一時的に停止します。 ジョブの状態を含むすべての進捗が保持され、ジョブが開始の呼び出しが行われる場合停止した位置から続行されます。
ms.openlocfilehash: dd46f5760d7ddcfff1e254d7c000e1cd80304f07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068981"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="b6a61-104">synchronizationJob: 一時停止</span><span class="sxs-lookup"><span data-stu-id="b6a61-104">synchronizationJob: pause</span></span>

> <span data-ttu-id="b6a61-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b6a61-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6a61-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6a61-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6a61-107">同期を一時的に停止します。</span><span class="sxs-lookup"><span data-stu-id="b6a61-107">Temporarily stop synchronization.</span></span> <span data-ttu-id="b6a61-108">ジョブの状態を含むすべての進捗が保持され、ジョブが[起動](../api/synchronization-synchronizationjob-start.md)の呼び出しが行われる場合停止した位置から続行されます。</span><span class="sxs-lookup"><span data-stu-id="b6a61-108">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6a61-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6a61-109">Permissions</span></span>
<span data-ttu-id="b6a61-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6a61-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6a61-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6a61-112">Permission type</span></span>                        | <span data-ttu-id="b6a61-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6a61-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6a61-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6a61-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="b6a61-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a61-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b6a61-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6a61-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b6a61-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6a61-117">Not supported.</span></span>  |
|<span data-ttu-id="b6a61-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6a61-118">Application</span></span>                            |<span data-ttu-id="b6a61-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6a61-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b6a61-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6a61-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="b6a61-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6a61-121">Request headers</span></span>

| <span data-ttu-id="b6a61-122">名前</span><span class="sxs-lookup"><span data-stu-id="b6a61-122">Name</span></span>           | <span data-ttu-id="b6a61-123">型</span><span class="sxs-lookup"><span data-stu-id="b6a61-123">Type</span></span>    | <span data-ttu-id="b6a61-124">説明</span><span class="sxs-lookup"><span data-stu-id="b6a61-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b6a61-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6a61-125">Authorization</span></span>  | <span data-ttu-id="b6a61-126">string</span><span class="sxs-lookup"><span data-stu-id="b6a61-126">string</span></span>  | <span data-ttu-id="b6a61-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b6a61-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6a61-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6a61-129">Request body</span></span>

<span data-ttu-id="b6a61-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6a61-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6a61-131">応答</span><span class="sxs-lookup"><span data-stu-id="b6a61-131">Response</span></span>

<span data-ttu-id="b6a61-132">正常終了した場合、`204 No Content`応答します。</span><span class="sxs-lookup"><span data-stu-id="b6a61-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="b6a61-133">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="b6a61-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6a61-134">例</span><span class="sxs-lookup"><span data-stu-id="b6a61-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b6a61-135">要求</span><span class="sxs-lookup"><span data-stu-id="b6a61-135">Request</span></span>
<span data-ttu-id="b6a61-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6a61-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="b6a61-137">応答</span><span class="sxs-lookup"><span data-stu-id="b6a61-137">Response</span></span>
<span data-ttu-id="b6a61-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6a61-138">The following is an example of a response.</span></span>
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