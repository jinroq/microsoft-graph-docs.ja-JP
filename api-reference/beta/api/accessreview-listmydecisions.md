---
title: マイ accessReview の決定事項を表示します。
description: Azure AD アクセスのレビュー機能をレビュー担当者として、accessReview オブジェクトの呼び出し元のユーザーの意思決定を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e19e3b0581c995f1b0ef52369d3a3e7545696d1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525326"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="ebb9c-103">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebb9c-104">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、レビュー担当者として、 [accessReview](../resources/accessreview.md)オブジェクトの呼び出し元のユーザーの意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebb9c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ebb9c-105">Permissions</span></span>
<span data-ttu-id="ebb9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebb9c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebb9c-108">Permission type</span></span>                        | <span data-ttu-id="ebb9c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebb9c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebb9c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebb9c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebb9c-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="ebb9c-111"></span></span>  <span data-ttu-id="ebb9c-112">サインインしているユーザーがこの特定のアクセス確認を読み取ることもできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-112">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="ebb9c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebb9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebb9c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-114">Not supported.</span></span> |
|<span data-ttu-id="ebb9c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebb9c-115">Application</span></span>                            | <span data-ttu-id="ebb9c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebb9c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebb9c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="ebb9c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebb9c-118">Request headers</span></span>
| <span data-ttu-id="ebb9c-119">名前</span><span class="sxs-lookup"><span data-stu-id="ebb9c-119">Name</span></span>         | <span data-ttu-id="ebb9c-120">型</span><span class="sxs-lookup"><span data-stu-id="ebb9c-120">Type</span></span>        | <span data-ttu-id="ebb9c-121">説明</span><span class="sxs-lookup"><span data-stu-id="ebb9c-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ebb9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebb9c-122">Authorization</span></span> | <span data-ttu-id="ebb9c-123">string</span><span class="sxs-lookup"><span data-stu-id="ebb9c-123">string</span></span> | <span data-ttu-id="ebb9c-124">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="ebb9c-124">Bearer \{token\}.</span></span> <span data-ttu-id="ebb9c-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebb9c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebb9c-126">Request body</span></span>
<span data-ttu-id="ebb9c-127">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="ebb9c-128">応答</span><span class="sxs-lookup"><span data-stu-id="ebb9c-128">Response</span></span>
<span data-ttu-id="ebb9c-129">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび呼び出し元のユーザーの割り当てのレビュー担当者の応答の本文に[accessReviewDecision](../resources/accessreviewdecision.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="ebb9c-130">例</span><span class="sxs-lookup"><span data-stu-id="ebb9c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebb9c-131">要求</span><span class="sxs-lookup"><span data-stu-id="ebb9c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="ebb9c-132">応答</span><span class="sxs-lookup"><span data-stu-id="ebb9c-132">Response</span></span>
><span data-ttu-id="ebb9c-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ebb9c-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="ebb9c-135">See also</span></span>

| <span data-ttu-id="ebb9c-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="ebb9c-136">Method</span></span>           | <span data-ttu-id="ebb9c-137">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ebb9c-137">Return Type</span></span>    |<span data-ttu-id="ebb9c-138">説明</span><span class="sxs-lookup"><span data-stu-id="ebb9c-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ebb9c-139">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="ebb9c-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="ebb9c-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="ebb9c-141">アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="ebb9c-142">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="ebb9c-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="ebb9c-143">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ebb9c-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="ebb9c-144">AccessReview のすべての意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="ebb9c-144">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
