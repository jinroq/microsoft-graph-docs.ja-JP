---
title: 同期ジョブの削除
description: 同期ジョブを停止し、関連付けられているすべての状態を完全に削除します。 同期されたアカウントは、そのまま残ります。
localization_priority: Normal
ms.openlocfilehash: cfcce1c3a1741625d409af22e0953df0b0ac20a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458172"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="1f722-104">同期ジョブの削除</span><span class="sxs-lookup"><span data-stu-id="1f722-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f722-105">同期ジョブを停止し、関連付けられているすべての状態を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="1f722-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="1f722-106">同期されたアカウントは、そのまま残ります。</span><span class="sxs-lookup"><span data-stu-id="1f722-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f722-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f722-107">Permissions</span></span>
<span data-ttu-id="1f722-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f722-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f722-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f722-110">Permission type</span></span>                        | <span data-ttu-id="1f722-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f722-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f722-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f722-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="1f722-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f722-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1f722-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f722-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1f722-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f722-115">Not supported.</span></span>  |
|<span data-ttu-id="1f722-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f722-116">Application</span></span>                            |<span data-ttu-id="1f722-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f722-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1f722-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f722-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="1f722-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f722-119">Request headers</span></span>

| <span data-ttu-id="1f722-120">名前</span><span class="sxs-lookup"><span data-stu-id="1f722-120">Name</span></span>           | <span data-ttu-id="1f722-121">型</span><span class="sxs-lookup"><span data-stu-id="1f722-121">Type</span></span>    | <span data-ttu-id="1f722-122">説明</span><span class="sxs-lookup"><span data-stu-id="1f722-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1f722-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f722-123">Authorization</span></span>  | <span data-ttu-id="1f722-124">string</span><span class="sxs-lookup"><span data-stu-id="1f722-124">string</span></span>  | <span data-ttu-id="1f722-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1f722-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f722-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f722-127">Request body</span></span>

<span data-ttu-id="1f722-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1f722-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f722-129">応答</span><span class="sxs-lookup"><span data-stu-id="1f722-129">Response</span></span>

<span data-ttu-id="1f722-130">成功した場合は`204 No Content` 、応答を返します。</span><span class="sxs-lookup"><span data-stu-id="1f722-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="1f722-131">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1f722-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f722-132">例</span><span class="sxs-lookup"><span data-stu-id="1f722-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1f722-133">要求</span><span class="sxs-lookup"><span data-stu-id="1f722-133">Request</span></span>
<span data-ttu-id="1f722-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f722-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1f722-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1f722-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f722-136">C#</span><span class="sxs-lookup"><span data-stu-id="1f722-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f722-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="1f722-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f722-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="1f722-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1f722-139">応答</span><span class="sxs-lookup"><span data-stu-id="1f722-139">Response</span></span>
<span data-ttu-id="1f722-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f722-140">The following is an example of the response.</span></span> 

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
  ]
}
-->
