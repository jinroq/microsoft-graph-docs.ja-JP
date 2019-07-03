---
title: 自分の accessReview の決定事項を一覧表示する
description: Azure AD access レビュー機能で、呼び出し元ユーザーの accessReview オブジェクトの決定をレビュー担当者として取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9db636c0ecbbd2413e5189fd5195a6d6685ae78
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440051"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="0321d-103">自分の accessReview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0321d-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0321d-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、呼び出し元ユーザーの[accessreview](../resources/accessreview.md)オブジェクトの決定をレビュー担当者として取得します。</span><span class="sxs-lookup"><span data-stu-id="0321d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="0321d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0321d-105">Permissions</span></span>
<span data-ttu-id="0321d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0321d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0321d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0321d-108">Permission type</span></span>                        | <span data-ttu-id="0321d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0321d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0321d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0321d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0321d-111">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0321d-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="0321d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0321d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0321d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0321d-113">Not supported.</span></span> |
|<span data-ttu-id="0321d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0321d-114">Application</span></span>                            | <span data-ttu-id="0321d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0321d-115">Not supported.</span></span> |

<span data-ttu-id="0321d-116">サインインしているユーザーは、この特定のアクセスレビューを読み取ることも許可されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0321d-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="0321d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0321d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="0321d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0321d-118">Request headers</span></span>
| <span data-ttu-id="0321d-119">名前</span><span class="sxs-lookup"><span data-stu-id="0321d-119">Name</span></span>         | <span data-ttu-id="0321d-120">型</span><span class="sxs-lookup"><span data-stu-id="0321d-120">Type</span></span>        | <span data-ttu-id="0321d-121">説明</span><span class="sxs-lookup"><span data-stu-id="0321d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0321d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0321d-122">Authorization</span></span> | <span data-ttu-id="0321d-123">string</span><span class="sxs-lookup"><span data-stu-id="0321d-123">string</span></span> | <span data-ttu-id="0321d-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="0321d-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0321d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0321d-126">Request body</span></span>
<span data-ttu-id="0321d-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="0321d-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="0321d-128">応答</span><span class="sxs-lookup"><span data-stu-id="0321d-128">Response</span></span>
<span data-ttu-id="0321d-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列を返します。これは、呼び出し元ユーザーが割り当てられた校閲者です。</span><span class="sxs-lookup"><span data-stu-id="0321d-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="0321d-130">例</span><span class="sxs-lookup"><span data-stu-id="0321d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0321d-131">要求</span><span class="sxs-lookup"><span data-stu-id="0321d-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0321d-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0321d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0321d-133">C#</span><span class="sxs-lookup"><span data-stu-id="0321d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0321d-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="0321d-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0321d-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="0321d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0321d-136">応答</span><span class="sxs-lookup"><span data-stu-id="0321d-136">Response</span></span>
><span data-ttu-id="0321d-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0321d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0321d-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="0321d-139">See also</span></span>

| <span data-ttu-id="0321d-140">メソッド</span><span class="sxs-lookup"><span data-stu-id="0321d-140">Method</span></span>           | <span data-ttu-id="0321d-141">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0321d-141">Return Type</span></span>    |<span data-ttu-id="0321d-142">説明</span><span class="sxs-lookup"><span data-stu-id="0321d-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0321d-143">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="0321d-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="0321d-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="0321d-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="0321d-145">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="0321d-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="0321d-146">AccessReview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0321d-146">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="0321d-147">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0321d-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="0321d-148">AccessReview のすべての決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="0321d-148">Retrieve all the decisions of an accessReview.</span></span>|


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
