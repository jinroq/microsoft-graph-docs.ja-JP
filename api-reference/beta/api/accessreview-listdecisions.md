---
title: accessreview に関する決定事項を一覧表示する
description: Azure AD access レビュー機能で、accessreview オブジェクトの決定を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeaa1374bbd44cfe9556e488d25e0fc2c7594cde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459638"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="93cef-103">accessreview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="93cef-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93cef-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトの決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="93cef-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="93cef-105">定期的なアクセスレビューに`decisions`関係はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="93cef-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="93cef-106">代わりに、呼び出し元は`instance`リレーションシップを移動して、 `accessReview`アクセスレビューの現在のインスタンスまたは過去のインスタンスのオブジェクトを検索する必要があります。</span><span class="sxs-lookup"><span data-stu-id="93cef-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="93cef-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="93cef-107">Permissions</span></span>
<span data-ttu-id="93cef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93cef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93cef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93cef-110">Permission type</span></span>                        | <span data-ttu-id="93cef-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="93cef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="93cef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93cef-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="93cef-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="93cef-113"></span></span>  <span data-ttu-id="93cef-114">サインインしているユーザーは、アクセスレビューを読み取ることができるようにするために、ディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="93cef-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="93cef-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93cef-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93cef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93cef-116">Not supported.</span></span> |
|<span data-ttu-id="93cef-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93cef-117">Application</span></span>                            | <span data-ttu-id="93cef-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93cef-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93cef-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93cef-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="93cef-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93cef-120">Request headers</span></span>
| <span data-ttu-id="93cef-121">名前</span><span class="sxs-lookup"><span data-stu-id="93cef-121">Name</span></span>         | <span data-ttu-id="93cef-122">型</span><span class="sxs-lookup"><span data-stu-id="93cef-122">Type</span></span>        | <span data-ttu-id="93cef-123">説明</span><span class="sxs-lookup"><span data-stu-id="93cef-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="93cef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="93cef-124">Authorization</span></span> | <span data-ttu-id="93cef-125">string</span><span class="sxs-lookup"><span data-stu-id="93cef-125">string</span></span> | <span data-ttu-id="93cef-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="93cef-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93cef-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="93cef-128">Request body</span></span>
<span data-ttu-id="93cef-129">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="93cef-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="93cef-130">応答</span><span class="sxs-lookup"><span data-stu-id="93cef-130">Response</span></span>
<span data-ttu-id="93cef-131">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="93cef-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93cef-132">例</span><span class="sxs-lookup"><span data-stu-id="93cef-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93cef-133">要求</span><span class="sxs-lookup"><span data-stu-id="93cef-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="93cef-134">応答</span><span class="sxs-lookup"><span data-stu-id="93cef-134">Response</span></span>
><span data-ttu-id="93cef-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="93cef-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="93cef-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="93cef-137">See also</span></span>

| <span data-ttu-id="93cef-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="93cef-138">Method</span></span>           | <span data-ttu-id="93cef-139">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93cef-139">Return Type</span></span>    |<span data-ttu-id="93cef-140">説明</span><span class="sxs-lookup"><span data-stu-id="93cef-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93cef-141">accessreview を取得する</span><span class="sxs-lookup"><span data-stu-id="93cef-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="93cef-142">accessreview</span><span class="sxs-lookup"><span data-stu-id="93cef-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="93cef-143">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="93cef-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="93cef-144">自分の accessreview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="93cef-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="93cef-145">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="93cef-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="93cef-146">レビュー担当者として、accessreview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="93cef-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="93cef-147">access レビュー通知の送信</span><span class="sxs-lookup"><span data-stu-id="93cef-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="93cef-148">なし。</span><span class="sxs-lookup"><span data-stu-id="93cef-148">None.</span></span>   |   <span data-ttu-id="93cef-149">accessreview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="93cef-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="93cef-150">accessreview を停止する</span><span class="sxs-lookup"><span data-stu-id="93cef-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="93cef-151">なし。</span><span class="sxs-lookup"><span data-stu-id="93cef-151">None.</span></span>   |   <span data-ttu-id="93cef-152">accessreview を停止します。</span><span class="sxs-lookup"><span data-stu-id="93cef-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="93cef-153">accessreview の決定をリセットする</span><span class="sxs-lookup"><span data-stu-id="93cef-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="93cef-154">なし。</span><span class="sxs-lookup"><span data-stu-id="93cef-154">None.</span></span>   |   <span data-ttu-id="93cef-155">進行中の accessreview で意思決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="93cef-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="93cef-156">accessreview の決定を適用する</span><span class="sxs-lookup"><span data-stu-id="93cef-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="93cef-157">なし。</span><span class="sxs-lookup"><span data-stu-id="93cef-157">None.</span></span>   |   <span data-ttu-id="93cef-158">完了した accessreview から決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="93cef-158">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
