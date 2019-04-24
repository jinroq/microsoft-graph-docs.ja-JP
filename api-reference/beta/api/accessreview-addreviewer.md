---
title: accessreview レビュー担当者を追加する
description: 'Azure AD access レビュー機能で、既存の accessreview オブジェクトを更新して、別のユーザーをレビュー担当者として追加します。  この操作は、まだ完了していないアクセスレビューに対してのみ許可されており、レビュー担当者が明示的に指定されているアクセスレビューに対してのみ使用できます。 この操作は、ユーザーが自分のアクセスを確認するアクセスレビューでは許可されず、グループの所有者がレビュー担当者として割り当てられているアクセスレビューのためのものではありません。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a526451330321c7fbbfd1d5287dd5ad892eee84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456858"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="7d26b-105">accessreview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="7d26b-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d26b-106">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[accessreview](../resources/accessreview.md)オブジェクトを更新して、別のユーザーをレビュー担当者として追加します。</span><span class="sxs-lookup"><span data-stu-id="7d26b-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="7d26b-107">この操作は、まだ完了していないアクセスレビューに対してのみ許可されており、レビュー担当者が明示的に指定されているアクセスレビューに対してのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="7d26b-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="7d26b-108">この操作は、ユーザーが自分のアクセスを確認するアクセスレビューでは許可されず、グループの所有者がレビュー担当者として割り当てられているアクセスレビューのためのものではありません。</span><span class="sxs-lookup"><span data-stu-id="7d26b-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7d26b-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d26b-109">Permissions</span></span>
<span data-ttu-id="7d26b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d26b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d26b-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d26b-112">Permission type</span></span>                        | <span data-ttu-id="7d26b-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d26b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d26b-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d26b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d26b-115">accessreview すべて</span><span class="sxs-lookup"><span data-stu-id="7d26b-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7d26b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d26b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d26b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d26b-117">Not supported.</span></span> |
|<span data-ttu-id="7d26b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d26b-118">Application</span></span>                            | <span data-ttu-id="7d26b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d26b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d26b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d26b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="7d26b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d26b-121">Request headers</span></span>
| <span data-ttu-id="7d26b-122">名前</span><span class="sxs-lookup"><span data-stu-id="7d26b-122">Name</span></span>         | <span data-ttu-id="7d26b-123">型</span><span class="sxs-lookup"><span data-stu-id="7d26b-123">Type</span></span>        | <span data-ttu-id="7d26b-124">説明</span><span class="sxs-lookup"><span data-stu-id="7d26b-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7d26b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d26b-125">Authorization</span></span> | <span data-ttu-id="7d26b-126">string</span><span class="sxs-lookup"><span data-stu-id="7d26b-126">string</span></span> | <span data-ttu-id="7d26b-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d26b-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d26b-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d26b-129">Request body</span></span>
<span data-ttu-id="7d26b-130">要求本文で、レビュー担当者になるユーザーの ID の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d26b-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="7d26b-131">次の表に、accessreview の更新時に提供できるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d26b-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="7d26b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d26b-132">Property</span></span>     | <span data-ttu-id="7d26b-133">型</span><span class="sxs-lookup"><span data-stu-id="7d26b-133">Type</span></span>        | <span data-ttu-id="7d26b-134">説明</span><span class="sxs-lookup"><span data-stu-id="7d26b-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="7d26b-135">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="7d26b-135">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="7d26b-136">応答</span><span class="sxs-lookup"><span data-stu-id="7d26b-136">Response</span></span>
<span data-ttu-id="7d26b-137">成功した場合、このメソッド`201, Created`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7d26b-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="7d26b-138">例</span><span class="sxs-lookup"><span data-stu-id="7d26b-138">Example</span></span>

<span data-ttu-id="7d26b-139">これは、追加のレビュー担当者との1回限り (定期的でない) アクセスレビューを更新する例です。</span><span class="sxs-lookup"><span data-stu-id="7d26b-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="7d26b-140">要求</span><span class="sxs-lookup"><span data-stu-id="7d26b-140">Request</span></span>
<span data-ttu-id="7d26b-141">要求本文で、ユーザーオブジェクトの id の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d26b-141">In the request body, supply a JSON representation of the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a><span data-ttu-id="7d26b-142">応答</span><span class="sxs-lookup"><span data-stu-id="7d26b-142">Response</span></span>
><span data-ttu-id="7d26b-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7d26b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
