---
title: AccessReview レビュー担当者を追加する
description: 'Azure AD access レビュー機能で、既存の accessReview オブジェクトを更新して、別のユーザーをレビュー担当者として追加します。  この操作は、まだ完了していないアクセスレビューに対してのみ許可されており、レビュー担当者が明示的に指定されているアクセスレビューに対してのみ使用できます。 この操作は、ユーザーが自分のアクセスを確認するアクセスレビューでは許可されず、グループの所有者がレビュー担当者として割り当てられているアクセスレビューのためのものではありません。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2f06e6f3f7b61e62a4cab8f6a4ea06e33374e278
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408993"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="209e6-105">AccessReview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="209e6-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="209e6-106">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[accessreview](../resources/accessreview.md)オブジェクトを更新して、別のユーザーをレビュー担当者として追加します。</span><span class="sxs-lookup"><span data-stu-id="209e6-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="209e6-107">この操作は、まだ完了していないアクセスレビューに対してのみ許可されており、レビュー担当者が明示的に指定されているアクセスレビューに対してのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="209e6-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="209e6-108">この操作は、ユーザーが自分のアクセスを確認するアクセスレビューでは許可されず、グループの所有者がレビュー担当者として割り当てられているアクセスレビューのためのものではありません。</span><span class="sxs-lookup"><span data-stu-id="209e6-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="209e6-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="209e6-109">Permissions</span></span>
<span data-ttu-id="209e6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="209e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="209e6-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="209e6-112">Permission type</span></span>                        | <span data-ttu-id="209e6-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="209e6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="209e6-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="209e6-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="209e6-115">AccessReview を行って、AccessReview を行います。</span><span class="sxs-lookup"><span data-stu-id="209e6-115">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="209e6-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="209e6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="209e6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="209e6-117">Not supported.</span></span> |
|<span data-ttu-id="209e6-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="209e6-118">Application</span></span>                            | <span data-ttu-id="209e6-119">AccessReview の構成</span><span class="sxs-lookup"><span data-stu-id="209e6-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="209e6-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="209e6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="209e6-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="209e6-121">Request headers</span></span>
| <span data-ttu-id="209e6-122">名前</span><span class="sxs-lookup"><span data-stu-id="209e6-122">Name</span></span>         | <span data-ttu-id="209e6-123">型</span><span class="sxs-lookup"><span data-stu-id="209e6-123">Type</span></span>        | <span data-ttu-id="209e6-124">説明</span><span class="sxs-lookup"><span data-stu-id="209e6-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="209e6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="209e6-125">Authorization</span></span> | <span data-ttu-id="209e6-126">string</span><span class="sxs-lookup"><span data-stu-id="209e6-126">string</span></span> | <span data-ttu-id="209e6-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="209e6-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="209e6-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="209e6-129">Request body</span></span>
<span data-ttu-id="209e6-130">要求本文で、レビュー担当者になるユーザーの ID の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="209e6-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="209e6-131">次の表に、accessReview の更新時に提供できるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="209e6-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="209e6-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="209e6-132">Property</span></span>     | <span data-ttu-id="209e6-133">型</span><span class="sxs-lookup"><span data-stu-id="209e6-133">Type</span></span>        | <span data-ttu-id="209e6-134">説明</span><span class="sxs-lookup"><span data-stu-id="209e6-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="209e6-135">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="209e6-135">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="209e6-136">応答</span><span class="sxs-lookup"><span data-stu-id="209e6-136">Response</span></span>
<span data-ttu-id="209e6-137">成功した場合、このメソッド`201, Created`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="209e6-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="209e6-138">例</span><span class="sxs-lookup"><span data-stu-id="209e6-138">Example</span></span>

<span data-ttu-id="209e6-139">これは、追加のレビュー担当者との1回限り (定期的でない) アクセスレビューを更新する例です。</span><span class="sxs-lookup"><span data-stu-id="209e6-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="209e6-140">要求</span><span class="sxs-lookup"><span data-stu-id="209e6-140">Request</span></span>
<span data-ttu-id="209e6-141">要求本文で、ユーザーオブジェクトの id の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="209e6-141">In the request body, supply a JSON representation of the id of the user object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="209e6-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="209e6-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
Content-Type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="209e6-143">C#</span><span class="sxs-lookup"><span data-stu-id="209e6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="209e6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="209e6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="209e6-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="209e6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="209e6-146">応答</span><span class="sxs-lookup"><span data-stu-id="209e6-146">Response</span></span>
><span data-ttu-id="209e6-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="209e6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
