---
title: リストの accessReview の決定
description: Azure AD のレビュー機能にアクセス、accessReview オブジェクトの決定を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeaa1374bbd44cfe9556e488d25e0fc2c7594cde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521797"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="00ded-103">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="00ded-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00ded-104">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [accessReview](../resources/accessreview.md)オブジェクトの決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="00ded-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="00ded-105">定期的なアクセス確認がないことに注意を`decisions`の関係。</span><span class="sxs-lookup"><span data-stu-id="00ded-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="00ded-106">代わりに、呼び出し元が移動する必要があります、`instance`を検索するには、顧客間関係、`accessReview`アクセス レビューの現在または過去のインスタンスのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="00ded-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="00ded-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00ded-107">Permissions</span></span>
<span data-ttu-id="00ded-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00ded-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ded-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00ded-110">Permission type</span></span>                        | <span data-ttu-id="00ded-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00ded-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="00ded-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00ded-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="00ded-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="00ded-113"></span></span>  <span data-ttu-id="00ded-114">サインインしているユーザーは、ディレクトリの役割をアクセスのレビューを読むことを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="00ded-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="00ded-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00ded-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00ded-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00ded-116">Not supported.</span></span> |
|<span data-ttu-id="00ded-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00ded-117">Application</span></span>                            | <span data-ttu-id="00ded-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00ded-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00ded-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00ded-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="00ded-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00ded-120">Request headers</span></span>
| <span data-ttu-id="00ded-121">名前</span><span class="sxs-lookup"><span data-stu-id="00ded-121">Name</span></span>         | <span data-ttu-id="00ded-122">型</span><span class="sxs-lookup"><span data-stu-id="00ded-122">Type</span></span>        | <span data-ttu-id="00ded-123">説明</span><span class="sxs-lookup"><span data-stu-id="00ded-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="00ded-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="00ded-124">Authorization</span></span> | <span data-ttu-id="00ded-125">string</span><span class="sxs-lookup"><span data-stu-id="00ded-125">string</span></span> | <span data-ttu-id="00ded-126">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="00ded-126">Bearer \{token\}.</span></span> <span data-ttu-id="00ded-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="00ded-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00ded-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="00ded-128">Request body</span></span>
<span data-ttu-id="00ded-129">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="00ded-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="00ded-130">応答</span><span class="sxs-lookup"><span data-stu-id="00ded-130">Response</span></span>
<span data-ttu-id="00ded-131">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="00ded-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00ded-132">例</span><span class="sxs-lookup"><span data-stu-id="00ded-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00ded-133">要求</span><span class="sxs-lookup"><span data-stu-id="00ded-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="00ded-134">応答</span><span class="sxs-lookup"><span data-stu-id="00ded-134">Response</span></span>
><span data-ttu-id="00ded-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="00ded-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="00ded-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="00ded-137">See also</span></span>

| <span data-ttu-id="00ded-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="00ded-138">Method</span></span>           | <span data-ttu-id="00ded-139">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="00ded-139">Return Type</span></span>    |<span data-ttu-id="00ded-140">説明</span><span class="sxs-lookup"><span data-stu-id="00ded-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="00ded-141">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="00ded-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="00ded-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="00ded-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="00ded-143">アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="00ded-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="00ded-144">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="00ded-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="00ded-145">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="00ded-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="00ded-146">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="00ded-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="00ded-147">AccessReview アラームを送信します。</span><span class="sxs-lookup"><span data-stu-id="00ded-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="00ded-148">なし。</span><span class="sxs-lookup"><span data-stu-id="00ded-148">None.</span></span>   |   <span data-ttu-id="00ded-149">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="00ded-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="00ded-150">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="00ded-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="00ded-151">なし。</span><span class="sxs-lookup"><span data-stu-id="00ded-151">None.</span></span>   |   <span data-ttu-id="00ded-152">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="00ded-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="00ded-153">リセット accessReview 決定</span><span class="sxs-lookup"><span data-stu-id="00ded-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="00ded-154">なし。</span><span class="sxs-lookup"><span data-stu-id="00ded-154">None.</span></span>   |   <span data-ttu-id="00ded-155">進行中の accessReview の決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="00ded-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="00ded-156">AccessReview の決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="00ded-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="00ded-157">なし。</span><span class="sxs-lookup"><span data-stu-id="00ded-157">None.</span></span>   |   <span data-ttu-id="00ded-158">完了した accessReview からの決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="00ded-158">Apply the decisions from a completed accessReview.</span></span>|


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
