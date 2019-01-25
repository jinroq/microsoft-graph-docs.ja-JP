---
title: 'synchronizationJob: 一時停止'
description: 同期を一時的に停止します。 ジョブの状態を含むすべての進捗が保持され、ジョブが開始の呼び出しが行われる場合停止した位置から続行されます。
localization_priority: Normal
ms.openlocfilehash: 9f8cac05511b5efd17234ccf16b763999418bf2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513922"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="ee3ca-104">synchronizationJob: 一時停止</span><span class="sxs-lookup"><span data-stu-id="ee3ca-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee3ca-105">同期を一時的に停止します。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="ee3ca-106">ジョブの状態を含むすべての進捗が保持され、ジョブが[起動](../api/synchronization-synchronizationjob-start.md)の呼び出しが行われる場合停止した位置から続行されます。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee3ca-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee3ca-107">Permissions</span></span>
<span data-ttu-id="ee3ca-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee3ca-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee3ca-110">Permission type</span></span>                        | <span data-ttu-id="ee3ca-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee3ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee3ca-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee3ca-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="ee3ca-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee3ca-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ee3ca-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee3ca-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ee3ca-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-115">Not supported.</span></span>  |
|<span data-ttu-id="ee3ca-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee3ca-116">Application</span></span>                            |<span data-ttu-id="ee3ca-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ee3ca-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee3ca-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="ee3ca-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee3ca-119">Request headers</span></span>

| <span data-ttu-id="ee3ca-120">名前</span><span class="sxs-lookup"><span data-stu-id="ee3ca-120">Name</span></span>           | <span data-ttu-id="ee3ca-121">型</span><span class="sxs-lookup"><span data-stu-id="ee3ca-121">Type</span></span>    | <span data-ttu-id="ee3ca-122">説明</span><span class="sxs-lookup"><span data-stu-id="ee3ca-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ee3ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee3ca-123">Authorization</span></span>  | <span data-ttu-id="ee3ca-124">string</span><span class="sxs-lookup"><span data-stu-id="ee3ca-124">string</span></span>  | <span data-ttu-id="ee3ca-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee3ca-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee3ca-127">Request body</span></span>

<span data-ttu-id="ee3ca-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee3ca-129">応答</span><span class="sxs-lookup"><span data-stu-id="ee3ca-129">Response</span></span>

<span data-ttu-id="ee3ca-130">正常終了した場合、`204 No Content`応答します。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="ee3ca-131">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee3ca-132">例</span><span class="sxs-lookup"><span data-stu-id="ee3ca-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee3ca-133">要求</span><span class="sxs-lookup"><span data-stu-id="ee3ca-133">Request</span></span>
<span data-ttu-id="ee3ca-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="ee3ca-135">応答</span><span class="sxs-lookup"><span data-stu-id="ee3ca-135">Response</span></span>
<span data-ttu-id="ee3ca-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ee3ca-136">The following is an example of a response.</span></span>
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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
