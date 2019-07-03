---
title: AccessReview に関する決定事項を一覧表示する
description: Azure AD access レビュー機能で、accessReview オブジェクトの決定を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 479699d55741830b542038dd43184a9ce7e1d535
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440058"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="6136a-103">AccessReview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6136a-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6136a-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトの決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="6136a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="6136a-105">定期的なアクセスレビューに`decisions`関係はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6136a-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="6136a-106">代わりに、呼び出し元は`instance`リレーションシップを移動して、 `accessReview`アクセスレビューの現在のインスタンスまたは過去のインスタンスのオブジェクトを検索する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6136a-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="6136a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6136a-107">Permissions</span></span>
<span data-ttu-id="6136a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6136a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6136a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6136a-110">Permission type</span></span>                        | <span data-ttu-id="6136a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6136a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6136a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6136a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6136a-113">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6136a-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="6136a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6136a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6136a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6136a-115">Not supported.</span></span> |
|<span data-ttu-id="6136a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6136a-116">Application</span></span>                            | <span data-ttu-id="6136a-117">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="6136a-117">AccessReview.Read.All</span></span> |

 <span data-ttu-id="6136a-118">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="6136a-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="6136a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6136a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="6136a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6136a-120">Request headers</span></span>
| <span data-ttu-id="6136a-121">名前</span><span class="sxs-lookup"><span data-stu-id="6136a-121">Name</span></span>         | <span data-ttu-id="6136a-122">型</span><span class="sxs-lookup"><span data-stu-id="6136a-122">Type</span></span>        | <span data-ttu-id="6136a-123">説明</span><span class="sxs-lookup"><span data-stu-id="6136a-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6136a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6136a-124">Authorization</span></span> | <span data-ttu-id="6136a-125">string</span><span class="sxs-lookup"><span data-stu-id="6136a-125">string</span></span> | <span data-ttu-id="6136a-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="6136a-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6136a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6136a-128">Request body</span></span>
<span data-ttu-id="6136a-129">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="6136a-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="6136a-130">応答</span><span class="sxs-lookup"><span data-stu-id="6136a-130">Response</span></span>
<span data-ttu-id="6136a-131">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="6136a-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6136a-132">例</span><span class="sxs-lookup"><span data-stu-id="6136a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6136a-133">要求</span><span class="sxs-lookup"><span data-stu-id="6136a-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6136a-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6136a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6136a-135">C#</span><span class="sxs-lookup"><span data-stu-id="6136a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6136a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="6136a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6136a-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="6136a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6136a-138">応答</span><span class="sxs-lookup"><span data-stu-id="6136a-138">Response</span></span>
><span data-ttu-id="6136a-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6136a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6136a-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="6136a-141">See also</span></span>

| <span data-ttu-id="6136a-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="6136a-142">Method</span></span>           | <span data-ttu-id="6136a-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6136a-143">Return Type</span></span>    |<span data-ttu-id="6136a-144">説明</span><span class="sxs-lookup"><span data-stu-id="6136a-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6136a-145">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="6136a-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="6136a-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="6136a-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="6136a-147">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="6136a-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="6136a-148">自分の accessReview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6136a-148">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="6136a-149">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6136a-149">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="6136a-150">レビュー担当者として、accessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="6136a-150">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="6136a-151">Access レビュー通知の送信</span><span class="sxs-lookup"><span data-stu-id="6136a-151">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="6136a-152">なし。</span><span class="sxs-lookup"><span data-stu-id="6136a-152">None.</span></span>   |   <span data-ttu-id="6136a-153">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="6136a-153">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="6136a-154">AccessReview を停止する</span><span class="sxs-lookup"><span data-stu-id="6136a-154">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="6136a-155">なし。</span><span class="sxs-lookup"><span data-stu-id="6136a-155">None.</span></span>   |   <span data-ttu-id="6136a-156">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="6136a-156">Stop an accessReview.</span></span> |
|[<span data-ttu-id="6136a-157">AccessReview の決定をリセットする</span><span class="sxs-lookup"><span data-stu-id="6136a-157">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="6136a-158">なし。</span><span class="sxs-lookup"><span data-stu-id="6136a-158">None.</span></span>   |   <span data-ttu-id="6136a-159">進行中の accessReview で意思決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="6136a-159">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="6136a-160">AccessReview の決定を適用する</span><span class="sxs-lookup"><span data-stu-id="6136a-160">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="6136a-161">なし。</span><span class="sxs-lookup"><span data-stu-id="6136a-161">None.</span></span>   |   <span data-ttu-id="6136a-162">完了した accessReview から決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="6136a-162">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
