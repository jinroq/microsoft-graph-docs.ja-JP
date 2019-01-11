---
title: マイ accessReview の決定事項を表示します。
description: Azure AD アクセスのレビュー機能をレビュー担当者として、accessReview オブジェクトの呼び出し元のユーザーの意思決定を取得します。
localization_priority: Normal
ms.openlocfilehash: 27ae3129810b6019ecf47e23f1e4cc48362df6fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819013"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="cc615-103">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="cc615-103">List my accessReview decisions</span></span>

> <span data-ttu-id="cc615-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc615-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc615-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc615-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc615-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、レビュー担当者として、 [accessReview](../resources/accessreview.md)オブジェクトの呼び出し元のユーザーの意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc615-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="cc615-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc615-107">Permissions</span></span>
<span data-ttu-id="cc615-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc615-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc615-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc615-110">Permission type</span></span>                        | <span data-ttu-id="cc615-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc615-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc615-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc615-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc615-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="cc615-113"></span></span>  <span data-ttu-id="cc615-114">サインインしているユーザーがこの特定のアクセス確認を読み取ることもできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc615-114">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="cc615-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc615-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc615-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc615-116">Not supported.</span></span> |
|<span data-ttu-id="cc615-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc615-117">Application</span></span>                            | <span data-ttu-id="cc615-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc615-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc615-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc615-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="cc615-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc615-120">Request headers</span></span>
| <span data-ttu-id="cc615-121">名前</span><span class="sxs-lookup"><span data-stu-id="cc615-121">Name</span></span>         | <span data-ttu-id="cc615-122">種類</span><span class="sxs-lookup"><span data-stu-id="cc615-122">Type</span></span>        | <span data-ttu-id="cc615-123">説明</span><span class="sxs-lookup"><span data-stu-id="cc615-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cc615-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc615-124">Authorization</span></span> | <span data-ttu-id="cc615-125">string</span><span class="sxs-lookup"><span data-stu-id="cc615-125">string</span></span> | <span data-ttu-id="cc615-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="cc615-126">Bearer \{token\}.</span></span> <span data-ttu-id="cc615-127">必須。</span><span class="sxs-lookup"><span data-stu-id="cc615-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc615-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc615-128">Request body</span></span>
<span data-ttu-id="cc615-129">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="cc615-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="cc615-130">応答</span><span class="sxs-lookup"><span data-stu-id="cc615-130">Response</span></span>
<span data-ttu-id="cc615-131">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび呼び出し元のユーザーの割り当てのレビュー担当者の応答の本文に[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="cc615-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="cc615-132">例</span><span class="sxs-lookup"><span data-stu-id="cc615-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc615-133">要求</span><span class="sxs-lookup"><span data-stu-id="cc615-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="cc615-134">応答</span><span class="sxs-lookup"><span data-stu-id="cc615-134">Response</span></span>
><span data-ttu-id="cc615-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cc615-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="cc615-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc615-137">See also</span></span>

| <span data-ttu-id="cc615-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc615-138">Method</span></span>           | <span data-ttu-id="cc615-139">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cc615-139">Return Type</span></span>    |<span data-ttu-id="cc615-140">説明</span><span class="sxs-lookup"><span data-stu-id="cc615-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc615-141">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc615-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="cc615-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="cc615-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="cc615-143">アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc615-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="cc615-144">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="cc615-144">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="cc615-145">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc615-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="cc615-146">AccessReview のすべての意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc615-146">Retrieve all the decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
