---
title: AccessReview の校閲者の一覧
description: Azure AD にアクセスが機能を確認、校閲者の accessReview オブジェクトを取得します。
ms.openlocfilehash: 24c8b3dacbbe1a5868c9ba82141f37b006dc7a75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067990"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="4a0c7-103">AccessReview の校閲者の一覧</span><span class="sxs-lookup"><span data-stu-id="4a0c7-103">List accessReview reviewers</span></span>

> <span data-ttu-id="4a0c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a0c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a0c7-106">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、校閲者の[accessReview](../resources/accessreview.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a0c7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a0c7-107">Permissions</span></span>
<span data-ttu-id="4a0c7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a0c7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a0c7-110">Permission type</span></span>                        | <span data-ttu-id="4a0c7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a0c7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a0c7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a0c7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a0c7-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="4a0c7-113"></span></span>  <span data-ttu-id="4a0c7-114">サインインしているユーザーは、ディレクトリの役割をアクセスのレビューを読むことを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="4a0c7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a0c7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a0c7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-116">Not supported.</span></span> |
|<span data-ttu-id="4a0c7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a0c7-117">Application</span></span>                            | <span data-ttu-id="4a0c7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a0c7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a0c7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="4a0c7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a0c7-120">Request headers</span></span>
| <span data-ttu-id="4a0c7-121">名前</span><span class="sxs-lookup"><span data-stu-id="4a0c7-121">Name</span></span>         | <span data-ttu-id="4a0c7-122">型</span><span class="sxs-lookup"><span data-stu-id="4a0c7-122">Type</span></span>        | <span data-ttu-id="4a0c7-123">説明</span><span class="sxs-lookup"><span data-stu-id="4a0c7-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4a0c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a0c7-124">Authorization</span></span> | <span data-ttu-id="4a0c7-125">string</span><span class="sxs-lookup"><span data-stu-id="4a0c7-125">string</span></span> | <span data-ttu-id="4a0c7-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-126">Bearer \{token\}.</span></span> <span data-ttu-id="4a0c7-127">必須。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a0c7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a0c7-128">Request body</span></span>
<span data-ttu-id="4a0c7-129">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="4a0c7-130">応答</span><span class="sxs-lookup"><span data-stu-id="4a0c7-130">Response</span></span>
<span data-ttu-id="4a0c7-131">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[割り当てられていません](../resources/useridentity.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-131">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a0c7-132">例</span><span class="sxs-lookup"><span data-stu-id="4a0c7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a0c7-133">要求</span><span class="sxs-lookup"><span data-stu-id="4a0c7-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="4a0c7-134">応答</span><span class="sxs-lookup"><span data-stu-id="4a0c7-134">Response</span></span>
><span data-ttu-id="4a0c7-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
       "id":"006111db-0810-4494-a6df-904d368bd81b"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="4a0c7-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="4a0c7-137">See also</span></span>

| <span data-ttu-id="4a0c7-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="4a0c7-138">Method</span></span>           | <span data-ttu-id="4a0c7-139">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4a0c7-139">Return Type</span></span>    |<span data-ttu-id="4a0c7-140">説明</span><span class="sxs-lookup"><span data-stu-id="4a0c7-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a0c7-141">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="4a0c7-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="4a0c7-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="4a0c7-143">アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="4a0c7-144">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-144">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="4a0c7-145">なし。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-145">None.</span></span>   |   <span data-ttu-id="4a0c7-146">AccessReview には、レビュー担当者を追加します。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-146">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="4a0c7-147">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-147">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="4a0c7-148">なし。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-148">None.</span></span> |   <span data-ttu-id="4a0c7-149">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="4a0c7-149">Remove a reviewer from an accessReview.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
