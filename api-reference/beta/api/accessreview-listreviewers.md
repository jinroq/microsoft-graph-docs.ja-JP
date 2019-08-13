---
title: AccessReview レビュー担当者のリスト
description: Azure AD access レビュー機能で、accessReview オブジェクトのレビュー担当者を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f0267adad98ea94b5f92342da92350b5c2693969
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319154"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="41678-103">AccessReview レビュー担当者のリスト</span><span class="sxs-lookup"><span data-stu-id="41678-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41678-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトのレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="41678-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="41678-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41678-105">Permissions</span></span>
<span data-ttu-id="41678-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41678-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41678-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41678-108">Permission type</span></span>                        | <span data-ttu-id="41678-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="41678-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="41678-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41678-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="41678-111">Accessreview を参照してください。この後、accessreview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41678-111">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="41678-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41678-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41678-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41678-113">Not supported.</span></span> |
|<span data-ttu-id="41678-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41678-114">Application</span></span>                            | <span data-ttu-id="41678-115">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41678-115">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="41678-116">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="41678-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="41678-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41678-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="41678-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41678-118">Request headers</span></span>
| <span data-ttu-id="41678-119">名前</span><span class="sxs-lookup"><span data-stu-id="41678-119">Name</span></span>         | <span data-ttu-id="41678-120">型</span><span class="sxs-lookup"><span data-stu-id="41678-120">Type</span></span>        | <span data-ttu-id="41678-121">説明</span><span class="sxs-lookup"><span data-stu-id="41678-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="41678-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41678-122">Authorization</span></span> | <span data-ttu-id="41678-123">string</span><span class="sxs-lookup"><span data-stu-id="41678-123">string</span></span> | <span data-ttu-id="41678-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="41678-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41678-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="41678-126">Request body</span></span>
<span data-ttu-id="41678-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="41678-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="41678-128">応答</span><span class="sxs-lookup"><span data-stu-id="41678-128">Response</span></span>
<span data-ttu-id="41678-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[useridentity](../resources/useridentity.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="41678-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41678-130">例</span><span class="sxs-lookup"><span data-stu-id="41678-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41678-131">要求</span><span class="sxs-lookup"><span data-stu-id="41678-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="41678-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="41678-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41678-133">C#</span><span class="sxs-lookup"><span data-stu-id="41678-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41678-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41678-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41678-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="41678-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41678-136">Java</span><span class="sxs-lookup"><span data-stu-id="41678-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-reviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="41678-137">応答</span><span class="sxs-lookup"><span data-stu-id="41678-137">Response</span></span>
><span data-ttu-id="41678-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="41678-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "value":
    [
        {
            "id":"006111db-0810-4494-a6df-904d368bd81b"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="41678-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="41678-140">See also</span></span>

| <span data-ttu-id="41678-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="41678-141">Method</span></span>           | <span data-ttu-id="41678-142">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="41678-142">Return Type</span></span>    |<span data-ttu-id="41678-143">説明</span><span class="sxs-lookup"><span data-stu-id="41678-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41678-144">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="41678-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="41678-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="41678-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="41678-146">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="41678-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="41678-147">AccessReview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="41678-147">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="41678-148">なし。</span><span class="sxs-lookup"><span data-stu-id="41678-148">None.</span></span>   |   <span data-ttu-id="41678-149">閲覧者を accessReview に追加します。</span><span class="sxs-lookup"><span data-stu-id="41678-149">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="41678-150">AccessReview レビュー担当者を削除する</span><span class="sxs-lookup"><span data-stu-id="41678-150">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="41678-151">なし。</span><span class="sxs-lookup"><span data-stu-id="41678-151">None.</span></span> |   <span data-ttu-id="41678-152">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="41678-152">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
