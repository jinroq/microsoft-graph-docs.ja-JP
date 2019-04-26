---
title: 自分の accessreview の決定事項を一覧表示する
description: Azure AD access レビュー機能で、呼び出し元ユーザーの accessreview オブジェクトの決定をレビュー担当者として取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a89e611b12c9aac8006c030e264cfd3514845ea0
ms.sourcegitcommit: 4bdcb5cd3227ff009e10868f2936b3153372b87a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2019
ms.locfileid: "33299634"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="fe1c1-103">自分の accessreview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fe1c1-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe1c1-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、呼び出し元ユーザーの[accessreview](../resources/accessreview.md)オブジェクトの決定をレビュー担当者として取得します。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe1c1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe1c1-105">Permissions</span></span>
<span data-ttu-id="fe1c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe1c1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe1c1-108">Permission type</span></span>                        | <span data-ttu-id="fe1c1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe1c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe1c1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe1c1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe1c1-111">accessreview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="fe1c1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe1c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe1c1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-113">Not supported.</span></span> |
|<span data-ttu-id="fe1c1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe1c1-114">Application</span></span>                            | <span data-ttu-id="fe1c1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-115">Not supported.</span></span> |

<span data-ttu-id="fe1c1-116">サインインしているユーザーは、この特定のアクセスレビューを読み取ることも許可されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe1c1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe1c1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="fe1c1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe1c1-118">Request headers</span></span>
| <span data-ttu-id="fe1c1-119">名前</span><span class="sxs-lookup"><span data-stu-id="fe1c1-119">Name</span></span>         | <span data-ttu-id="fe1c1-120">型</span><span class="sxs-lookup"><span data-stu-id="fe1c1-120">Type</span></span>        | <span data-ttu-id="fe1c1-121">説明</span><span class="sxs-lookup"><span data-stu-id="fe1c1-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fe1c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe1c1-122">Authorization</span></span> | <span data-ttu-id="fe1c1-123">string</span><span class="sxs-lookup"><span data-stu-id="fe1c1-123">string</span></span> | <span data-ttu-id="fe1c1-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe1c1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe1c1-126">Request body</span></span>
<span data-ttu-id="fe1c1-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="fe1c1-128">応答</span><span class="sxs-lookup"><span data-stu-id="fe1c1-128">Response</span></span>
<span data-ttu-id="fe1c1-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列を返します。これは、呼び出し元ユーザーが割り当てられた校閲者です。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="fe1c1-130">例</span><span class="sxs-lookup"><span data-stu-id="fe1c1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe1c1-131">要求</span><span class="sxs-lookup"><span data-stu-id="fe1c1-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```

##### <a name="response"></a><span data-ttu-id="fe1c1-132">応答</span><span class="sxs-lookup"><span data-stu-id="fe1c1-132">Response</span></span>
><span data-ttu-id="fe1c1-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fe1c1-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="fe1c1-135">See also</span></span>

| <span data-ttu-id="fe1c1-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe1c1-136">Method</span></span>           | <span data-ttu-id="fe1c1-137">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fe1c1-137">Return Type</span></span>    |<span data-ttu-id="fe1c1-138">説明</span><span class="sxs-lookup"><span data-stu-id="fe1c1-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe1c1-139">accessreview を取得する</span><span class="sxs-lookup"><span data-stu-id="fe1c1-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="fe1c1-140">accessreview</span><span class="sxs-lookup"><span data-stu-id="fe1c1-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="fe1c1-141">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="fe1c1-142">accessreview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fe1c1-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="fe1c1-143">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fe1c1-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="fe1c1-144">accessreview のすべての決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="fe1c1-144">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
