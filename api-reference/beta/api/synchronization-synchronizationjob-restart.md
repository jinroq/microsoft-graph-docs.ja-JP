---
title: SynchronizationJob を再起動します。
description: ディレクトリ内のすべてのオブジェクトを再処理することを強制する、同期ジョブを再起動します。 必要に応じて既存の同期の状態と以前のエラーをクリアします。
ms.openlocfilehash: 0b7ebfcd7b13400225d9ea149442207ecd994a8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072718"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="361e7-104">SynchronizationJob を再起動します。</span><span class="sxs-lookup"><span data-stu-id="361e7-104">Restart synchronizationJob</span></span>

> <span data-ttu-id="361e7-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="361e7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="361e7-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="361e7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="361e7-107">ディレクトリ内のすべてのオブジェクトを再処理することを強制する、同期ジョブを再起動します。</span><span class="sxs-lookup"><span data-stu-id="361e7-107">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="361e7-108">必要に応じて既存の同期の状態と以前のエラーをクリアします。</span><span class="sxs-lookup"><span data-stu-id="361e7-108">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="361e7-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="361e7-109">Permissions</span></span>
<span data-ttu-id="361e7-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="361e7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="361e7-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="361e7-112">Permission type</span></span>                        | <span data-ttu-id="361e7-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="361e7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="361e7-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="361e7-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="361e7-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="361e7-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="361e7-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="361e7-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="361e7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="361e7-117">Not supported.</span></span> |
|<span data-ttu-id="361e7-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="361e7-118">Application</span></span>                            |<span data-ttu-id="361e7-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="361e7-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="361e7-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="361e7-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="361e7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="361e7-121">Request headers</span></span>

| <span data-ttu-id="361e7-122">名前</span><span class="sxs-lookup"><span data-stu-id="361e7-122">Name</span></span>           | <span data-ttu-id="361e7-123">型</span><span class="sxs-lookup"><span data-stu-id="361e7-123">Type</span></span>    | <span data-ttu-id="361e7-124">説明</span><span class="sxs-lookup"><span data-stu-id="361e7-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="361e7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="361e7-125">Authorization</span></span>  | <span data-ttu-id="361e7-126">string</span><span class="sxs-lookup"><span data-stu-id="361e7-126">string</span></span>  | <span data-ttu-id="361e7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="361e7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="361e7-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="361e7-129">Request body</span></span>

<span data-ttu-id="361e7-130">要求の本文には、次のパラメーターを使用して JSON オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="361e7-130">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="361e7-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="361e7-131">Parameter</span></span>     | <span data-ttu-id="361e7-132">型</span><span class="sxs-lookup"><span data-stu-id="361e7-132">Type</span></span>      | <span data-ttu-id="361e7-133">説明</span><span class="sxs-lookup"><span data-stu-id="361e7-133">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="361e7-134">criteria</span><span class="sxs-lookup"><span data-stu-id="361e7-134">criteria</span></span>       |[<span data-ttu-id="361e7-135">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="361e7-135">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="361e7-136">条件を再起動します。</span><span class="sxs-lookup"><span data-stu-id="361e7-136">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="361e7-137">応答</span><span class="sxs-lookup"><span data-stu-id="361e7-137">Response</span></span>

<span data-ttu-id="361e7-138">正常終了した場合、`204 No Content`応答します。</span><span class="sxs-lookup"><span data-stu-id="361e7-138">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="361e7-139">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="361e7-139">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="361e7-140">例</span><span class="sxs-lookup"><span data-stu-id="361e7-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="361e7-141">要求</span><span class="sxs-lookup"><span data-stu-id="361e7-141">Request</span></span>
<span data-ttu-id="361e7-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="361e7-142">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_restart"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
Authorization: Bearer <token>
Content-type: application/json

{
   "criteria": {
       "resetScope": "ConnectorDataStore, Escrows, QuarantineState"
   }
}
```

##### <a name="response"></a><span data-ttu-id="361e7-143">応答</span><span class="sxs-lookup"><span data-stu-id="361e7-143">Response</span></span>
<span data-ttu-id="361e7-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="361e7-144">The following is an example of a response.</span></span>

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
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
