---
title: リストの accessReview の決定
description: Azure AD のレビュー機能にアクセス、accessReview オブジェクトの決定を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f89fdbce1c87ce9ef8a6ba8c5b7f9b7be410617
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927010"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="5f947-103">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="5f947-103">List accessReview decisions</span></span>

> <span data-ttu-id="5f947-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f947-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f947-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f947-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f947-106">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [accessReview](../resources/accessreview.md)オブジェクトの決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="5f947-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="5f947-107">定期的なアクセス確認がないことに注意を`decisions`の関係。</span><span class="sxs-lookup"><span data-stu-id="5f947-107">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="5f947-108">代わりに、呼び出し元が移動する必要があります、`instance`を検索するには、顧客間関係、`accessReview`アクセス レビューの現在または過去のインスタンスのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5f947-108">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f947-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f947-109">Permissions</span></span>
<span data-ttu-id="5f947-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f947-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f947-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f947-112">Permission type</span></span>                        | <span data-ttu-id="5f947-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f947-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f947-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f947-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f947-115">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="5f947-115"></span></span>  <span data-ttu-id="5f947-116">サインインしているユーザーは、ディレクトリの役割をアクセスのレビューを読むことを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f947-116">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="5f947-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f947-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f947-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f947-118">Not supported.</span></span> |
|<span data-ttu-id="5f947-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f947-119">Application</span></span>                            | <span data-ttu-id="5f947-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f947-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f947-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f947-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="5f947-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f947-122">Request headers</span></span>
| <span data-ttu-id="5f947-123">名前</span><span class="sxs-lookup"><span data-stu-id="5f947-123">Name</span></span>         | <span data-ttu-id="5f947-124">型</span><span class="sxs-lookup"><span data-stu-id="5f947-124">Type</span></span>        | <span data-ttu-id="5f947-125">説明</span><span class="sxs-lookup"><span data-stu-id="5f947-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5f947-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f947-126">Authorization</span></span> | <span data-ttu-id="5f947-127">string</span><span class="sxs-lookup"><span data-stu-id="5f947-127">string</span></span> | <span data-ttu-id="5f947-128">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="5f947-128">Bearer \{token\}.</span></span> <span data-ttu-id="5f947-129">必須。</span><span class="sxs-lookup"><span data-stu-id="5f947-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f947-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f947-130">Request body</span></span>
<span data-ttu-id="5f947-131">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="5f947-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="5f947-132">応答</span><span class="sxs-lookup"><span data-stu-id="5f947-132">Response</span></span>
<span data-ttu-id="5f947-133">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="5f947-133">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f947-134">例</span><span class="sxs-lookup"><span data-stu-id="5f947-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f947-135">要求</span><span class="sxs-lookup"><span data-stu-id="5f947-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="5f947-136">応答</span><span class="sxs-lookup"><span data-stu-id="5f947-136">Response</span></span>
><span data-ttu-id="5f947-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5f947-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5f947-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f947-139">See also</span></span>

| <span data-ttu-id="5f947-140">メソッド</span><span class="sxs-lookup"><span data-stu-id="5f947-140">Method</span></span>           | <span data-ttu-id="5f947-141">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5f947-141">Return Type</span></span>    |<span data-ttu-id="5f947-142">説明</span><span class="sxs-lookup"><span data-stu-id="5f947-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f947-143">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="5f947-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="5f947-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="5f947-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="5f947-145">アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="5f947-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="5f947-146">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="5f947-146">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="5f947-147">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5f947-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="5f947-148">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="5f947-148">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="5f947-149">AccessReview アラームを送信します。</span><span class="sxs-lookup"><span data-stu-id="5f947-149">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="5f947-150">なし。</span><span class="sxs-lookup"><span data-stu-id="5f947-150">None.</span></span>   |   <span data-ttu-id="5f947-151">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="5f947-151">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="5f947-152">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="5f947-152">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="5f947-153">なし。</span><span class="sxs-lookup"><span data-stu-id="5f947-153">None.</span></span>   |   <span data-ttu-id="5f947-154">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="5f947-154">Stop an accessReview.</span></span> |
|[<span data-ttu-id="5f947-155">リセット accessReview 決定</span><span class="sxs-lookup"><span data-stu-id="5f947-155">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="5f947-156">なし。</span><span class="sxs-lookup"><span data-stu-id="5f947-156">None.</span></span>   |   <span data-ttu-id="5f947-157">進行中の accessReview の決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="5f947-157">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="5f947-158">AccessReview の決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="5f947-158">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="5f947-159">なし。</span><span class="sxs-lookup"><span data-stu-id="5f947-159">None.</span></span>   |   <span data-ttu-id="5f947-160">完了した accessReview からの決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="5f947-160">Apply the decisions from a completed accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
