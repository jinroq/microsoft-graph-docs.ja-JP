---
title: AccessReview を停止する
description: Azure AD access レビュー機能で、現在アクティブな accessReview を停止します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  (定期的なアクセスレビューが今後のインスタンスを開始しないようにするには、それを更新して、スケジュールされた終了日を変更します)。  アクセスレビューが停止すると、レビュー担当者は入力を行うことができなくなり、アクセスレビューの決定を適用できるようになります。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d919c42a5817b7c33dbc51fcc8c46fd4f443e067
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655391"
---
# <a name="stop-accessreview"></a><span data-ttu-id="e2bfb-106">AccessReview を停止する</span><span class="sxs-lookup"><span data-stu-id="e2bfb-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2bfb-107">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、現在アクティブな[accessreview](../resources/accessreview.md)を停止します。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="e2bfb-108">ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="e2bfb-109">(定期的なアクセスレビューが今後のインスタンスを開始しないようにするには、[それを更新して](accessreview-update.md)、スケジュールされた終了日を変更します)。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="e2bfb-110">アクセスレビューが停止すると、レビュー担当者は入力を行うことができなくなり、アクセスレビューの決定を適用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2bfb-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2bfb-111">Permissions</span></span>
<span data-ttu-id="e2bfb-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2bfb-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2bfb-114">Permission type</span></span>                        | <span data-ttu-id="e2bfb-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2bfb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2bfb-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2bfb-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2bfb-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2bfb-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="e2bfb-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2bfb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2bfb-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-119">Not supported.</span></span> |
|<span data-ttu-id="e2bfb-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2bfb-120">Application</span></span>                            | <span data-ttu-id="e2bfb-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e2bfb-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2bfb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="e2bfb-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2bfb-123">Request headers</span></span>
| <span data-ttu-id="e2bfb-124">名前</span><span class="sxs-lookup"><span data-stu-id="e2bfb-124">Name</span></span>         | <span data-ttu-id="e2bfb-125">型</span><span class="sxs-lookup"><span data-stu-id="e2bfb-125">Type</span></span>        | <span data-ttu-id="e2bfb-126">説明</span><span class="sxs-lookup"><span data-stu-id="e2bfb-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e2bfb-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2bfb-127">Authorization</span></span> | <span data-ttu-id="e2bfb-128">string</span><span class="sxs-lookup"><span data-stu-id="e2bfb-128">string</span></span> | <span data-ttu-id="e2bfb-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2bfb-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2bfb-131">Request body</span></span>
<span data-ttu-id="e2bfb-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e2bfb-133">応答</span><span class="sxs-lookup"><span data-stu-id="e2bfb-133">Response</span></span>
<span data-ttu-id="e2bfb-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2bfb-136">例</span><span class="sxs-lookup"><span data-stu-id="e2bfb-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2bfb-137">要求</span><span class="sxs-lookup"><span data-stu-id="e2bfb-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
##### <a name="response"></a><span data-ttu-id="e2bfb-138">応答</span><span class="sxs-lookup"><span data-stu-id="e2bfb-138">Response</span></span>
><span data-ttu-id="e2bfb-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e2bfb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e2bfb-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e2bfb-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e2bfb-142">C#</span><span class="sxs-lookup"><span data-stu-id="e2bfb-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/stop_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2bfb-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="e2bfb-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/stop_accessReview-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
