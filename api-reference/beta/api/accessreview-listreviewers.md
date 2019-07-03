---
title: AccessReview レビュー担当者のリスト
description: Azure AD access レビュー機能で、accessReview オブジェクトのレビュー担当者を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9890df72f00d223f169b80ae2ba277560ccf5c72
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440044"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="54cea-103">AccessReview レビュー担当者のリスト</span><span class="sxs-lookup"><span data-stu-id="54cea-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54cea-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトのレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="54cea-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="54cea-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54cea-105">Permissions</span></span>
<span data-ttu-id="54cea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54cea-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54cea-108">Permission type</span></span>                        | <span data-ttu-id="54cea-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="54cea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="54cea-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54cea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="54cea-111">AccessReview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54cea-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="54cea-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54cea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54cea-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54cea-113">Not supported.</span></span> |
|<span data-ttu-id="54cea-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54cea-114">Application</span></span>                            | <span data-ttu-id="54cea-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="54cea-115">AccessReview.Read.All</span></span>  |


 <span data-ttu-id="54cea-116">また、サインインしているユーザーは、アクセスレビューを読み取ることができるようにするためのディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="54cea-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="54cea-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54cea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="54cea-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54cea-118">Request headers</span></span>
| <span data-ttu-id="54cea-119">名前</span><span class="sxs-lookup"><span data-stu-id="54cea-119">Name</span></span>         | <span data-ttu-id="54cea-120">型</span><span class="sxs-lookup"><span data-stu-id="54cea-120">Type</span></span>        | <span data-ttu-id="54cea-121">説明</span><span class="sxs-lookup"><span data-stu-id="54cea-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="54cea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54cea-122">Authorization</span></span> | <span data-ttu-id="54cea-123">string</span><span class="sxs-lookup"><span data-stu-id="54cea-123">string</span></span> | <span data-ttu-id="54cea-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="54cea-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54cea-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="54cea-126">Request body</span></span>
<span data-ttu-id="54cea-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="54cea-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="54cea-128">応答</span><span class="sxs-lookup"><span data-stu-id="54cea-128">Response</span></span>
<span data-ttu-id="54cea-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[useridentity](../resources/useridentity.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="54cea-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54cea-130">例</span><span class="sxs-lookup"><span data-stu-id="54cea-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54cea-131">要求</span><span class="sxs-lookup"><span data-stu-id="54cea-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="54cea-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="54cea-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="54cea-133">C#</span><span class="sxs-lookup"><span data-stu-id="54cea-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54cea-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="54cea-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54cea-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="54cea-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="54cea-136">応答</span><span class="sxs-lookup"><span data-stu-id="54cea-136">Response</span></span>
><span data-ttu-id="54cea-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="54cea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="54cea-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="54cea-139">See also</span></span>

| <span data-ttu-id="54cea-140">メソッド</span><span class="sxs-lookup"><span data-stu-id="54cea-140">Method</span></span>           | <span data-ttu-id="54cea-141">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="54cea-141">Return Type</span></span>    |<span data-ttu-id="54cea-142">説明</span><span class="sxs-lookup"><span data-stu-id="54cea-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54cea-143">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="54cea-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="54cea-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="54cea-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="54cea-145">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="54cea-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="54cea-146">AccessReview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="54cea-146">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="54cea-147">なし。</span><span class="sxs-lookup"><span data-stu-id="54cea-147">None.</span></span>   |   <span data-ttu-id="54cea-148">閲覧者を accessReview に追加します。</span><span class="sxs-lookup"><span data-stu-id="54cea-148">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="54cea-149">AccessReview レビュー担当者を削除する</span><span class="sxs-lookup"><span data-stu-id="54cea-149">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="54cea-150">なし。</span><span class="sxs-lookup"><span data-stu-id="54cea-150">None.</span></span> |   <span data-ttu-id="54cea-151">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="54cea-151">Remove a reviewer from an accessReview.</span></span> |


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
