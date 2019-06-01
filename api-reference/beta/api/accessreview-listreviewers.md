---
title: AccessReview レビュー担当者のリスト
description: Azure AD access レビュー機能で、accessReview オブジェクトのレビュー担当者を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 36bf733ca0502ba00d5848b362125e5e3058ab9a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655524"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="a2b8c-103">AccessReview レビュー担当者のリスト</span><span class="sxs-lookup"><span data-stu-id="a2b8c-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2b8c-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトのレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2b8c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2b8c-105">Permissions</span></span>
<span data-ttu-id="a2b8c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2b8c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2b8c-108">Permission type</span></span>                        | <span data-ttu-id="a2b8c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2b8c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2b8c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2b8c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2b8c-111">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a2b8c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2b8c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2b8c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-113">Not supported.</span></span> |
|<span data-ttu-id="a2b8c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2b8c-114">Application</span></span>                            | <span data-ttu-id="a2b8c-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b8c-115">AccessReview.Read.All</span></span>  |


 <span data-ttu-id="a2b8c-116">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="a2b8c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2b8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="a2b8c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2b8c-118">Request headers</span></span>
| <span data-ttu-id="a2b8c-119">名前</span><span class="sxs-lookup"><span data-stu-id="a2b8c-119">Name</span></span>         | <span data-ttu-id="a2b8c-120">型</span><span class="sxs-lookup"><span data-stu-id="a2b8c-120">Type</span></span>        | <span data-ttu-id="a2b8c-121">説明</span><span class="sxs-lookup"><span data-stu-id="a2b8c-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a2b8c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b8c-122">Authorization</span></span> | <span data-ttu-id="a2b8c-123">string</span><span class="sxs-lookup"><span data-stu-id="a2b8c-123">string</span></span> | <span data-ttu-id="a2b8c-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2b8c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2b8c-126">Request body</span></span>
<span data-ttu-id="a2b8c-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="a2b8c-128">応答</span><span class="sxs-lookup"><span data-stu-id="a2b8c-128">Response</span></span>
<span data-ttu-id="a2b8c-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[useridentity](../resources/useridentity.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b8c-130">例</span><span class="sxs-lookup"><span data-stu-id="a2b8c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2b8c-131">要求</span><span class="sxs-lookup"><span data-stu-id="a2b8c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```

##### <a name="response"></a><span data-ttu-id="a2b8c-132">応答</span><span class="sxs-lookup"><span data-stu-id="a2b8c-132">Response</span></span>
><span data-ttu-id="a2b8c-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a2b8c-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a2b8c-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a2b8c-136">C#</span><span class="sxs-lookup"><span data-stu-id="a2b8c-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2b8c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2b8c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="a2b8c-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="a2b8c-138">See also</span></span>

| <span data-ttu-id="a2b8c-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2b8c-139">Method</span></span>           | <span data-ttu-id="a2b8c-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a2b8c-140">Return Type</span></span>    |<span data-ttu-id="a2b8c-141">説明</span><span class="sxs-lookup"><span data-stu-id="a2b8c-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2b8c-142">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="a2b8c-142">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="a2b8c-143">accessReview</span><span class="sxs-lookup"><span data-stu-id="a2b8c-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="a2b8c-144">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-144">Retrieve an access review.</span></span> |
|[<span data-ttu-id="a2b8c-145">AccessReview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="a2b8c-145">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="a2b8c-146">なし。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-146">None.</span></span>   |   <span data-ttu-id="a2b8c-147">閲覧者を accessReview に追加します。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-147">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="a2b8c-148">AccessReview レビュー担当者を削除する</span><span class="sxs-lookup"><span data-stu-id="a2b8c-148">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="a2b8c-149">なし。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-149">None.</span></span> |   <span data-ttu-id="a2b8c-150">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="a2b8c-150">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
