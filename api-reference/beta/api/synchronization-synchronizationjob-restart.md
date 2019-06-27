---
title: 同期ジョブを再開します。
description: 同期ジョブを再開して、ディレクトリ内のすべてのオブジェクトを強制的に再処理するようにします。 必要に応じて、既存の同期状態および以前のエラーをクリアします。
localization_priority: Normal
ms.openlocfilehash: a97aa458bdecb9e6755add708a5e9799e1365b74
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271366"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="4c47c-104">同期ジョブを再開します。</span><span class="sxs-lookup"><span data-stu-id="4c47c-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c47c-105">同期ジョブを再開して、ディレクトリ内のすべてのオブジェクトを強制的に再処理するようにします。</span><span class="sxs-lookup"><span data-stu-id="4c47c-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="4c47c-106">必要に応じて、既存の同期状態および以前のエラーをクリアします。</span><span class="sxs-lookup"><span data-stu-id="4c47c-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c47c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c47c-107">Permissions</span></span>
<span data-ttu-id="4c47c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c47c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c47c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c47c-110">Permission type</span></span>                        | <span data-ttu-id="4c47c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c47c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c47c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c47c-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="4c47c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c47c-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4c47c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c47c-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4c47c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c47c-115">Not supported.</span></span> |
|<span data-ttu-id="4c47c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c47c-116">Application</span></span>                            |<span data-ttu-id="4c47c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c47c-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="4c47c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c47c-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="4c47c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c47c-119">Request headers</span></span>

| <span data-ttu-id="4c47c-120">名前</span><span class="sxs-lookup"><span data-stu-id="4c47c-120">Name</span></span>           | <span data-ttu-id="4c47c-121">型</span><span class="sxs-lookup"><span data-stu-id="4c47c-121">Type</span></span>    | <span data-ttu-id="4c47c-122">説明</span><span class="sxs-lookup"><span data-stu-id="4c47c-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4c47c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c47c-123">Authorization</span></span>  | <span data-ttu-id="4c47c-124">string</span><span class="sxs-lookup"><span data-stu-id="4c47c-124">string</span></span>  | <span data-ttu-id="4c47c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c47c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c47c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c47c-127">Request body</span></span>

<span data-ttu-id="4c47c-128">要求本文で、次のパラメーターを使用して JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c47c-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="4c47c-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4c47c-129">Parameter</span></span>     | <span data-ttu-id="4c47c-130">型</span><span class="sxs-lookup"><span data-stu-id="4c47c-130">Type</span></span>      | <span data-ttu-id="4c47c-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c47c-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="4c47c-132">criteria</span><span class="sxs-lookup"><span data-stu-id="4c47c-132">criteria</span></span>       |[<span data-ttu-id="4c47c-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="4c47c-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="4c47c-134">再起動の条件</span><span class="sxs-lookup"><span data-stu-id="4c47c-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="4c47c-135">応答</span><span class="sxs-lookup"><span data-stu-id="4c47c-135">Response</span></span>

<span data-ttu-id="4c47c-136">成功した場合は`204 No Content` 、応答を返します。</span><span class="sxs-lookup"><span data-stu-id="4c47c-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="4c47c-137">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4c47c-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c47c-138">例</span><span class="sxs-lookup"><span data-stu-id="4c47c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4c47c-139">要求</span><span class="sxs-lookup"><span data-stu-id="4c47c-139">Request</span></span>
<span data-ttu-id="4c47c-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c47c-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4c47c-141">応答</span><span class="sxs-lookup"><span data-stu-id="4c47c-141">Response</span></span>
<span data-ttu-id="4c47c-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c47c-142">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c47c-143">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="4c47c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4c47c-144">C#</span><span class="sxs-lookup"><span data-stu-id="4c47c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c47c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c47c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4c47c-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="4c47c-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
