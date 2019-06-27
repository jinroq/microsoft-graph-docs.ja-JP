---
title: AccessReview に関する決定事項を一覧表示する
description: Azure AD access レビュー機能で、accessReview オブジェクトの決定を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8958a9011fd1381fddbf811284ad70f427864f22
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258857"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="77d5f-103">AccessReview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="77d5f-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77d5f-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトの決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="77d5f-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="77d5f-105">定期的なアクセスレビューに`decisions`関係はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="77d5f-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="77d5f-106">代わりに、呼び出し元は`instance`リレーションシップを移動して、 `accessReview`アクセスレビューの現在のインスタンスまたは過去のインスタンスのオブジェクトを検索する必要があります。</span><span class="sxs-lookup"><span data-stu-id="77d5f-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="77d5f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77d5f-107">Permissions</span></span>
<span data-ttu-id="77d5f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77d5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77d5f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77d5f-110">Permission type</span></span>                        | <span data-ttu-id="77d5f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77d5f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="77d5f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77d5f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="77d5f-113">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77d5f-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="77d5f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77d5f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77d5f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77d5f-115">Not supported.</span></span> |
|<span data-ttu-id="77d5f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77d5f-116">Application</span></span>                            | <span data-ttu-id="77d5f-117">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="77d5f-117">AccessReview.Read.All</span></span> |

 <span data-ttu-id="77d5f-118">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="77d5f-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="77d5f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77d5f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="77d5f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77d5f-120">Request headers</span></span>
| <span data-ttu-id="77d5f-121">名前</span><span class="sxs-lookup"><span data-stu-id="77d5f-121">Name</span></span>         | <span data-ttu-id="77d5f-122">型</span><span class="sxs-lookup"><span data-stu-id="77d5f-122">Type</span></span>        | <span data-ttu-id="77d5f-123">説明</span><span class="sxs-lookup"><span data-stu-id="77d5f-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="77d5f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77d5f-124">Authorization</span></span> | <span data-ttu-id="77d5f-125">string</span><span class="sxs-lookup"><span data-stu-id="77d5f-125">string</span></span> | <span data-ttu-id="77d5f-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="77d5f-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77d5f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="77d5f-128">Request body</span></span>
<span data-ttu-id="77d5f-129">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="77d5f-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="77d5f-130">応答</span><span class="sxs-lookup"><span data-stu-id="77d5f-130">Response</span></span>
<span data-ttu-id="77d5f-131">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="77d5f-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77d5f-132">例</span><span class="sxs-lookup"><span data-stu-id="77d5f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77d5f-133">要求</span><span class="sxs-lookup"><span data-stu-id="77d5f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```

##### <a name="response"></a><span data-ttu-id="77d5f-134">応答</span><span class="sxs-lookup"><span data-stu-id="77d5f-134">Response</span></span>
><span data-ttu-id="77d5f-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="77d5f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="77d5f-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="77d5f-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="77d5f-138">C#</span><span class="sxs-lookup"><span data-stu-id="77d5f-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77d5f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="77d5f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="77d5f-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="77d5f-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="77d5f-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="77d5f-141">See also</span></span>

| <span data-ttu-id="77d5f-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="77d5f-142">Method</span></span>           | <span data-ttu-id="77d5f-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="77d5f-143">Return Type</span></span>    |<span data-ttu-id="77d5f-144">説明</span><span class="sxs-lookup"><span data-stu-id="77d5f-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77d5f-145">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="77d5f-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="77d5f-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="77d5f-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="77d5f-147">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="77d5f-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="77d5f-148">自分の accessReview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="77d5f-148">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="77d5f-149">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="77d5f-149">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="77d5f-150">レビュー担当者として、accessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="77d5f-150">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="77d5f-151">Access レビュー通知の送信</span><span class="sxs-lookup"><span data-stu-id="77d5f-151">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="77d5f-152">なし。</span><span class="sxs-lookup"><span data-stu-id="77d5f-152">None.</span></span>   |   <span data-ttu-id="77d5f-153">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="77d5f-153">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="77d5f-154">AccessReview を停止する</span><span class="sxs-lookup"><span data-stu-id="77d5f-154">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="77d5f-155">なし。</span><span class="sxs-lookup"><span data-stu-id="77d5f-155">None.</span></span>   |   <span data-ttu-id="77d5f-156">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="77d5f-156">Stop an accessReview.</span></span> |
|[<span data-ttu-id="77d5f-157">AccessReview の決定をリセットする</span><span class="sxs-lookup"><span data-stu-id="77d5f-157">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="77d5f-158">なし。</span><span class="sxs-lookup"><span data-stu-id="77d5f-158">None.</span></span>   |   <span data-ttu-id="77d5f-159">進行中の accessReview で意思決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="77d5f-159">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="77d5f-160">AccessReview の決定を適用する</span><span class="sxs-lookup"><span data-stu-id="77d5f-160">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="77d5f-161">なし。</span><span class="sxs-lookup"><span data-stu-id="77d5f-161">None.</span></span>   |   <span data-ttu-id="77d5f-162">完了した accessReview から決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="77d5f-162">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
