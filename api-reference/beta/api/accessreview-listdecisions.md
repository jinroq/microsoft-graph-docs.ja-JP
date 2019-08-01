---
title: AccessReview に関する決定事項を一覧表示する
description: Azure AD access レビュー機能で、accessReview オブジェクトの決定を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 466bf38854f50e2896388af02928641dd9180edf
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049611"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="682bc-103">AccessReview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="682bc-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="682bc-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトの決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="682bc-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="682bc-105">定期的なアクセスレビューに`decisions`関係はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="682bc-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="682bc-106">代わりに、呼び出し元は`instance`リレーションシップを移動して、 `accessReview`アクセスレビューの現在のインスタンスまたは過去のインスタンスのオブジェクトを検索する必要があります。</span><span class="sxs-lookup"><span data-stu-id="682bc-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="682bc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="682bc-107">Permissions</span></span>
<span data-ttu-id="682bc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="682bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="682bc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="682bc-110">Permission type</span></span>                        | <span data-ttu-id="682bc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="682bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="682bc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="682bc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="682bc-113">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="682bc-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="682bc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="682bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="682bc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="682bc-115">Not supported.</span></span> |
|<span data-ttu-id="682bc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="682bc-116">Application</span></span>                            | <span data-ttu-id="682bc-117">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="682bc-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="682bc-118">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="682bc-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="682bc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="682bc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="682bc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="682bc-120">Request headers</span></span>
| <span data-ttu-id="682bc-121">名前</span><span class="sxs-lookup"><span data-stu-id="682bc-121">Name</span></span>         | <span data-ttu-id="682bc-122">型</span><span class="sxs-lookup"><span data-stu-id="682bc-122">Type</span></span>        | <span data-ttu-id="682bc-123">説明</span><span class="sxs-lookup"><span data-stu-id="682bc-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="682bc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="682bc-124">Authorization</span></span> | <span data-ttu-id="682bc-125">string</span><span class="sxs-lookup"><span data-stu-id="682bc-125">string</span></span> | <span data-ttu-id="682bc-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="682bc-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="682bc-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="682bc-128">Request body</span></span>
<span data-ttu-id="682bc-129">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="682bc-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="682bc-130">応答</span><span class="sxs-lookup"><span data-stu-id="682bc-130">Response</span></span>
<span data-ttu-id="682bc-131">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="682bc-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="682bc-132">例</span><span class="sxs-lookup"><span data-stu-id="682bc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="682bc-133">要求</span><span class="sxs-lookup"><span data-stu-id="682bc-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="682bc-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="682bc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="682bc-135">C#</span><span class="sxs-lookup"><span data-stu-id="682bc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="682bc-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="682bc-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="682bc-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="682bc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="682bc-138">Java</span><span class="sxs-lookup"><span data-stu-id="682bc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="682bc-139">応答</span><span class="sxs-lookup"><span data-stu-id="682bc-139">Response</span></span>
><span data-ttu-id="682bc-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="682bc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="682bc-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="682bc-142">See also</span></span>

| <span data-ttu-id="682bc-143">メソッド</span><span class="sxs-lookup"><span data-stu-id="682bc-143">Method</span></span>           | <span data-ttu-id="682bc-144">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="682bc-144">Return Type</span></span>    |<span data-ttu-id="682bc-145">説明</span><span class="sxs-lookup"><span data-stu-id="682bc-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="682bc-146">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="682bc-146">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="682bc-147">accessReview</span><span class="sxs-lookup"><span data-stu-id="682bc-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="682bc-148">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="682bc-148">Retrieve an access review.</span></span> |
|[<span data-ttu-id="682bc-149">自分の accessReview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="682bc-149">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="682bc-150">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="682bc-150">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="682bc-151">レビュー担当者として、accessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="682bc-151">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="682bc-152">Access レビュー通知の送信</span><span class="sxs-lookup"><span data-stu-id="682bc-152">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="682bc-153">なし。</span><span class="sxs-lookup"><span data-stu-id="682bc-153">None.</span></span>   |   <span data-ttu-id="682bc-154">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="682bc-154">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="682bc-155">AccessReview を停止する</span><span class="sxs-lookup"><span data-stu-id="682bc-155">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="682bc-156">なし。</span><span class="sxs-lookup"><span data-stu-id="682bc-156">None.</span></span>   |   <span data-ttu-id="682bc-157">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="682bc-157">Stop an accessReview.</span></span> |
|[<span data-ttu-id="682bc-158">AccessReview の決定をリセットする</span><span class="sxs-lookup"><span data-stu-id="682bc-158">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="682bc-159">なし。</span><span class="sxs-lookup"><span data-stu-id="682bc-159">None.</span></span>   |   <span data-ttu-id="682bc-160">進行中の accessReview で意思決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="682bc-160">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="682bc-161">AccessReview の決定を適用する</span><span class="sxs-lookup"><span data-stu-id="682bc-161">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="682bc-162">なし。</span><span class="sxs-lookup"><span data-stu-id="682bc-162">None.</span></span>   |   <span data-ttu-id="682bc-163">完了した accessReview から決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="682bc-163">Apply the decisions from a completed accessReview.</span></span>|


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
