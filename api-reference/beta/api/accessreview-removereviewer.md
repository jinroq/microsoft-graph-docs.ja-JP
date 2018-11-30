---
title: AccessReview のレビュー担当者を削除します。
description: 'Azure AD アクセスのレビュー機能では、レビュー担当者として、ユーザーを削除するのには既存の accessReview オブジェクトを更新します。  この操作のみ許可されてはまだ完了していない、アクセスの確認のためや、アクセスの確認にのみ、校閲者が明示的に指定されています。 この操作は、アクセス確認をユーザーが独自のアクセスを確認するには許可されませんし、校閲者として、グループの所有者が割り当てられている、アクセス確認のためではありません。 '
ms.openlocfilehash: 2f2e1be904b98ed4dc2b3b34088b344e05b03473
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067986"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="1f0ac-105">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-105">Remove accessReview reviewer</span></span>

> <span data-ttu-id="1f0ac-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f0ac-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f0ac-108">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、レビュー担当者として、ユーザーを削除するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="1f0ac-109">この操作のみ許可されてはまだ完了していない、アクセスの確認のためや、アクセスの確認にのみ、校閲者が明示的に指定されています。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="1f0ac-110">この操作は、アクセス確認をユーザーが独自のアクセスを確認するには許可されませんし、校閲者として、グループの所有者が割り当てられている、アクセス確認のためではありません。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="1f0ac-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f0ac-111">Permissions</span></span>
<span data-ttu-id="1f0ac-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f0ac-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f0ac-114">Permission type</span></span>                        | <span data-ttu-id="1f0ac-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f0ac-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f0ac-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f0ac-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f0ac-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f0ac-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1f0ac-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f0ac-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f0ac-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-119">Not supported.</span></span> |
|<span data-ttu-id="1f0ac-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f0ac-120">Application</span></span>                            | <span data-ttu-id="1f0ac-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f0ac-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f0ac-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="1f0ac-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f0ac-123">Request headers</span></span>
| <span data-ttu-id="1f0ac-124">名前</span><span class="sxs-lookup"><span data-stu-id="1f0ac-124">Name</span></span>         | <span data-ttu-id="1f0ac-125">型</span><span class="sxs-lookup"><span data-stu-id="1f0ac-125">Type</span></span>        | <span data-ttu-id="1f0ac-126">説明</span><span class="sxs-lookup"><span data-stu-id="1f0ac-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1f0ac-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f0ac-127">Authorization</span></span> | <span data-ttu-id="1f0ac-128">string</span><span class="sxs-lookup"><span data-stu-id="1f0ac-128">string</span></span> | <span data-ttu-id="1f0ac-129">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-129">Bearer \{token\}.</span></span> <span data-ttu-id="1f0ac-130">必須。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f0ac-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f0ac-131">Request body</span></span>
<span data-ttu-id="1f0ac-132">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-132">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="1f0ac-133">応答</span><span class="sxs-lookup"><span data-stu-id="1f0ac-133">Response</span></span>
<span data-ttu-id="1f0ac-134">成功した場合、このメソッドは、200 シリーズの応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-134">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="1f0ac-135">使用例</span><span class="sxs-lookup"><span data-stu-id="1f0ac-135">Example</span></span>

<span data-ttu-id="1f0ac-136">これは、不要なのレビュー担当者を削除するのには 1 回限り (繰り返し発生しない) アクセス レビューの更新の例です。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-136">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="1f0ac-137">要求</span><span class="sxs-lookup"><span data-stu-id="1f0ac-137">Request</span></span>
<span data-ttu-id="1f0ac-138">要求の URL では、accessReview オブジェクトの id と、ユーザー オブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f0ac-138">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="1f0ac-139">応答</span><span class="sxs-lookup"><span data-stu-id="1f0ac-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
