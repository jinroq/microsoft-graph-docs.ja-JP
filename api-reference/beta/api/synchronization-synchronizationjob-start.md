---
title: SynchronizationJob を開始します。
description: 既存の同期ジョブを開始します。 ジョブが一時停止状態にある場合は、その一時停止された時点から変更の処理は続行されます。 ジョブは、検疫では、検疫の状態がクリアされます。
ms.openlocfilehash: c9f326a2c00564f25fb0ff982ede7e8454e14c8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073368"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="5a76b-105">SynchronizationJob を開始します。</span><span class="sxs-lookup"><span data-stu-id="5a76b-105">Start synchronizationJob</span></span>

> <span data-ttu-id="5a76b-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a76b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a76b-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a76b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a76b-108">既存の同期ジョブを開始します。</span><span class="sxs-lookup"><span data-stu-id="5a76b-108">Start an existing synchronization job.</span></span> <span data-ttu-id="5a76b-109">ジョブが一時停止状態にある場合は、その一時停止された時点から変更の処理は続行されます。</span><span class="sxs-lookup"><span data-stu-id="5a76b-109">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="5a76b-110">ジョブは、検疫では、検疫の状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="5a76b-110">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a76b-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a76b-111">Permissions</span></span>
<span data-ttu-id="5a76b-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a76b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a76b-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a76b-114">Permission type</span></span>                        | <span data-ttu-id="5a76b-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a76b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a76b-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a76b-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="5a76b-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a76b-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5a76b-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a76b-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5a76b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a76b-119">Not supported.</span></span> |
|<span data-ttu-id="5a76b-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a76b-120">Application</span></span>                            |<span data-ttu-id="5a76b-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a76b-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5a76b-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a76b-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="5a76b-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a76b-123">Request headers</span></span>

| <span data-ttu-id="5a76b-124">名前</span><span class="sxs-lookup"><span data-stu-id="5a76b-124">Name</span></span>           | <span data-ttu-id="5a76b-125">型</span><span class="sxs-lookup"><span data-stu-id="5a76b-125">Type</span></span>    | <span data-ttu-id="5a76b-126">説明</span><span class="sxs-lookup"><span data-stu-id="5a76b-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5a76b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a76b-127">Authorization</span></span>  | <span data-ttu-id="5a76b-128">string</span><span class="sxs-lookup"><span data-stu-id="5a76b-128">string</span></span>  | <span data-ttu-id="5a76b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a76b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a76b-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a76b-131">Request body</span></span>

<span data-ttu-id="5a76b-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5a76b-132">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="5a76b-133">応答</span><span class="sxs-lookup"><span data-stu-id="5a76b-133">Response</span></span>

<span data-ttu-id="5a76b-134">正常終了した場合、`204 No Content`応答します。</span><span class="sxs-lookup"><span data-stu-id="5a76b-134">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="5a76b-135">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="5a76b-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a76b-136">例</span><span class="sxs-lookup"><span data-stu-id="5a76b-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5a76b-137">要求</span><span class="sxs-lookup"><span data-stu-id="5a76b-137">Request</span></span>
<span data-ttu-id="5a76b-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a76b-138">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="5a76b-139">応答</span><span class="sxs-lookup"><span data-stu-id="5a76b-139">Response</span></span>
<span data-ttu-id="5a76b-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a76b-140">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
