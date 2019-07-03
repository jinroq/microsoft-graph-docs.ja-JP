---
title: 同期ジョブを開始する
description: 既存の同期ジョブを開始します。 ジョブが一時停止状態の場合、一時停止していた時点からの変更の処理は続行されます。 ジョブが検疫されている場合、検疫の状態はクリアされます。
localization_priority: Normal
ms.openlocfilehash: 977c38fa55de77e572e96be12f145a434caa688e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458179"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="aaa7f-105">同期ジョブを開始する</span><span class="sxs-lookup"><span data-stu-id="aaa7f-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaa7f-106">既存の同期ジョブを開始します。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-106">Start an existing synchronization job.</span></span> <span data-ttu-id="aaa7f-107">ジョブが一時停止状態の場合、一時停止していた時点からの変更の処理は続行されます。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="aaa7f-108">ジョブが検疫されている場合、検疫の状態はクリアされます。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaa7f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aaa7f-109">Permissions</span></span>
<span data-ttu-id="aaa7f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaa7f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aaa7f-112">Permission type</span></span>                        | <span data-ttu-id="aaa7f-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aaa7f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaa7f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aaa7f-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="aaa7f-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaa7f-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="aaa7f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aaa7f-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="aaa7f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-117">Not supported.</span></span> |
|<span data-ttu-id="aaa7f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aaa7f-118">Application</span></span>                            |<span data-ttu-id="aaa7f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aaa7f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aaa7f-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="aaa7f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aaa7f-121">Request headers</span></span>

| <span data-ttu-id="aaa7f-122">名前</span><span class="sxs-lookup"><span data-stu-id="aaa7f-122">Name</span></span>           | <span data-ttu-id="aaa7f-123">型</span><span class="sxs-lookup"><span data-stu-id="aaa7f-123">Type</span></span>    | <span data-ttu-id="aaa7f-124">説明</span><span class="sxs-lookup"><span data-stu-id="aaa7f-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="aaa7f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaa7f-125">Authorization</span></span>  | <span data-ttu-id="aaa7f-126">string</span><span class="sxs-lookup"><span data-stu-id="aaa7f-126">string</span></span>  | <span data-ttu-id="aaa7f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaa7f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="aaa7f-129">Request body</span></span>

<span data-ttu-id="aaa7f-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="aaa7f-131">応答</span><span class="sxs-lookup"><span data-stu-id="aaa7f-131">Response</span></span>

<span data-ttu-id="aaa7f-132">成功した場合は`204 No Content` 、応答を返します。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="aaa7f-133">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaa7f-134">例</span><span class="sxs-lookup"><span data-stu-id="aaa7f-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aaa7f-135">要求</span><span class="sxs-lookup"><span data-stu-id="aaa7f-135">Request</span></span>
<span data-ttu-id="aaa7f-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-136">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aaa7f-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aaa7f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aaa7f-138">C#</span><span class="sxs-lookup"><span data-stu-id="aaa7f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aaa7f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="aaa7f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aaa7f-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="aaa7f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aaa7f-141">応答</span><span class="sxs-lookup"><span data-stu-id="aaa7f-141">Response</span></span>
<span data-ttu-id="aaa7f-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aaa7f-142">The following is an example of a response.</span></span>
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
  ]
}
-->
