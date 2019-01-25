---
title: SynchronizationJob を削除します。
description: 同期ジョブを停止し、それに関連付けられているすべての状態を完全に削除します。 同期されたアカウントのままには。
localization_priority: Normal
ms.openlocfilehash: 29083413c5b24a5ed07b671adfa048f58d437f0d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521685"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="da104-104">SynchronizationJob を削除します。</span><span class="sxs-lookup"><span data-stu-id="da104-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da104-105">同期ジョブを停止し、それに関連付けられているすべての状態を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="da104-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="da104-106">同期されたアカウントのままには。</span><span class="sxs-lookup"><span data-stu-id="da104-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="da104-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da104-107">Permissions</span></span>
<span data-ttu-id="da104-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da104-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da104-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da104-110">Permission type</span></span>                        | <span data-ttu-id="da104-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da104-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="da104-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da104-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="da104-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da104-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="da104-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da104-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="da104-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da104-115">Not supported.</span></span>  |
|<span data-ttu-id="da104-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da104-116">Application</span></span>                            |<span data-ttu-id="da104-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da104-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="da104-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da104-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="da104-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da104-119">Request headers</span></span>

| <span data-ttu-id="da104-120">名前</span><span class="sxs-lookup"><span data-stu-id="da104-120">Name</span></span>           | <span data-ttu-id="da104-121">型</span><span class="sxs-lookup"><span data-stu-id="da104-121">Type</span></span>    | <span data-ttu-id="da104-122">説明</span><span class="sxs-lookup"><span data-stu-id="da104-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="da104-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da104-123">Authorization</span></span>  | <span data-ttu-id="da104-124">string</span><span class="sxs-lookup"><span data-stu-id="da104-124">string</span></span>  | <span data-ttu-id="da104-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="da104-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da104-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="da104-127">Request body</span></span>

<span data-ttu-id="da104-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="da104-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da104-129">応答</span><span class="sxs-lookup"><span data-stu-id="da104-129">Response</span></span>

<span data-ttu-id="da104-130">正常終了した場合、`204 No Content`応答します。</span><span class="sxs-lookup"><span data-stu-id="da104-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="da104-131">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="da104-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da104-132">例</span><span class="sxs-lookup"><span data-stu-id="da104-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="da104-133">要求</span><span class="sxs-lookup"><span data-stu-id="da104-133">Request</span></span>
<span data-ttu-id="da104-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da104-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="da104-135">応答</span><span class="sxs-lookup"><span data-stu-id="da104-135">Response</span></span>
<span data-ttu-id="da104-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da104-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
