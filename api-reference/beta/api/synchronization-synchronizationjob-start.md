---
title: SynchronizationJob を開始します。
description: 既存の同期ジョブを開始します。 ジョブが一時停止状態にある場合は、その一時停止された時点から変更の処理は続行されます。 ジョブは、検疫では、検疫の状態がクリアされます。
localization_priority: Normal
ms.openlocfilehash: 4648d9d3d889adf2cd7ec06e4fcf79b761c77132
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515371"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="943c9-105">SynchronizationJob を開始します。</span><span class="sxs-lookup"><span data-stu-id="943c9-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="943c9-106">既存の同期ジョブを開始します。</span><span class="sxs-lookup"><span data-stu-id="943c9-106">Start an existing synchronization job.</span></span> <span data-ttu-id="943c9-107">ジョブが一時停止状態にある場合は、その一時停止された時点から変更の処理は続行されます。</span><span class="sxs-lookup"><span data-stu-id="943c9-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="943c9-108">ジョブは、検疫では、検疫の状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="943c9-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="943c9-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="943c9-109">Permissions</span></span>
<span data-ttu-id="943c9-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="943c9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="943c9-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="943c9-112">Permission type</span></span>                        | <span data-ttu-id="943c9-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="943c9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="943c9-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="943c9-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="943c9-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="943c9-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="943c9-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="943c9-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="943c9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="943c9-117">Not supported.</span></span> |
|<span data-ttu-id="943c9-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="943c9-118">Application</span></span>                            |<span data-ttu-id="943c9-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="943c9-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="943c9-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="943c9-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="943c9-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="943c9-121">Request headers</span></span>

| <span data-ttu-id="943c9-122">名前</span><span class="sxs-lookup"><span data-stu-id="943c9-122">Name</span></span>           | <span data-ttu-id="943c9-123">型</span><span class="sxs-lookup"><span data-stu-id="943c9-123">Type</span></span>    | <span data-ttu-id="943c9-124">説明</span><span class="sxs-lookup"><span data-stu-id="943c9-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="943c9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="943c9-125">Authorization</span></span>  | <span data-ttu-id="943c9-126">string</span><span class="sxs-lookup"><span data-stu-id="943c9-126">string</span></span>  | <span data-ttu-id="943c9-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="943c9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="943c9-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="943c9-129">Request body</span></span>

<span data-ttu-id="943c9-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="943c9-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="943c9-131">応答</span><span class="sxs-lookup"><span data-stu-id="943c9-131">Response</span></span>

<span data-ttu-id="943c9-132">正常終了した場合、`204 No Content`応答します。</span><span class="sxs-lookup"><span data-stu-id="943c9-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="943c9-133">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="943c9-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="943c9-134">例</span><span class="sxs-lookup"><span data-stu-id="943c9-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="943c9-135">要求</span><span class="sxs-lookup"><span data-stu-id="943c9-135">Request</span></span>
<span data-ttu-id="943c9-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="943c9-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="943c9-137">応答</span><span class="sxs-lookup"><span data-stu-id="943c9-137">Response</span></span>
<span data-ttu-id="943c9-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="943c9-138">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
