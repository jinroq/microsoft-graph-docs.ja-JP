---
title: '同期ジョブ: 一時停止'
description: 一時的に同期を停止します。 ジョブの状態を含むすべての進行状況が持続され、開始呼び出しが行われたときにジョブは中断したところから続行されます。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a1503aa6de14f3738248020c10c3b5d53111476
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977809"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="7f43a-104">同期ジョブ: 一時停止</span><span class="sxs-lookup"><span data-stu-id="7f43a-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f43a-105">一時的に同期を停止します。</span><span class="sxs-lookup"><span data-stu-id="7f43a-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="7f43a-106">ジョブの状態を含むすべての進行状況が持続され、[開始](../api/synchronization-synchronizationjob-start.md)呼び出しが行われたときにジョブは中断したところから続行されます。</span><span class="sxs-lookup"><span data-stu-id="7f43a-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f43a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f43a-107">Permissions</span></span>
<span data-ttu-id="7f43a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f43a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f43a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f43a-110">Permission type</span></span>                        | <span data-ttu-id="7f43a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f43a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f43a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f43a-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="7f43a-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f43a-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7f43a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f43a-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7f43a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f43a-115">Not supported.</span></span>  |
|<span data-ttu-id="7f43a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f43a-116">Application</span></span>                            |<span data-ttu-id="7f43a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f43a-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7f43a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f43a-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="7f43a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f43a-119">Request headers</span></span>

| <span data-ttu-id="7f43a-120">名前</span><span class="sxs-lookup"><span data-stu-id="7f43a-120">Name</span></span>           | <span data-ttu-id="7f43a-121">型</span><span class="sxs-lookup"><span data-stu-id="7f43a-121">Type</span></span>    | <span data-ttu-id="7f43a-122">説明</span><span class="sxs-lookup"><span data-stu-id="7f43a-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7f43a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f43a-123">Authorization</span></span>  | <span data-ttu-id="7f43a-124">string</span><span class="sxs-lookup"><span data-stu-id="7f43a-124">string</span></span>  | <span data-ttu-id="7f43a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f43a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f43a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f43a-127">Request body</span></span>

<span data-ttu-id="7f43a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f43a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f43a-129">応答</span><span class="sxs-lookup"><span data-stu-id="7f43a-129">Response</span></span>

<span data-ttu-id="7f43a-130">成功した場合は`204 No Content` 、応答を返します。</span><span class="sxs-lookup"><span data-stu-id="7f43a-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="7f43a-131">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7f43a-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f43a-132">例</span><span class="sxs-lookup"><span data-stu-id="7f43a-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7f43a-133">要求</span><span class="sxs-lookup"><span data-stu-id="7f43a-133">Request</span></span>
<span data-ttu-id="7f43a-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f43a-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7f43a-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7f43a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f43a-136">C#</span><span class="sxs-lookup"><span data-stu-id="7f43a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f43a-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f43a-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f43a-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="7f43a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7f43a-139">Java</span><span class="sxs-lookup"><span data-stu-id="7f43a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f43a-140">応答</span><span class="sxs-lookup"><span data-stu-id="7f43a-140">Response</span></span>
<span data-ttu-id="7f43a-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f43a-141">The following is an example of a response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
