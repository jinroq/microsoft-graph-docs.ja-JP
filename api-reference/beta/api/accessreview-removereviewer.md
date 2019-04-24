---
title: accessreview レビュー担当者を削除する
description: 'Azure AD access レビュー機能で、既存の accessreview オブジェクトを更新して、ユーザーを校閲者として削除します。  この操作は、まだ完了していないアクセスレビューに対してのみ許可されており、レビュー担当者が明示的に指定されているアクセスレビューに対してのみ使用できます。 この操作は、ユーザーが自分のアクセスを確認するアクセスレビューでは許可されず、グループの所有者がレビュー担当者として割り当てられているアクセスレビューのためのものではありません。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3b6ea0fecb6b9179f40fa185aa770a743776eaa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459432"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="2f454-105">accessreview レビュー担当者を削除する</span><span class="sxs-lookup"><span data-stu-id="2f454-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f454-106">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[accessreview](../resources/accessreview.md)オブジェクトを更新して、ユーザーを校閲者として削除します。</span><span class="sxs-lookup"><span data-stu-id="2f454-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="2f454-107">この操作は、まだ完了していないアクセスレビューに対してのみ許可されており、レビュー担当者が明示的に指定されているアクセスレビューに対してのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="2f454-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="2f454-108">この操作は、ユーザーが自分のアクセスを確認するアクセスレビューでは許可されず、グループの所有者がレビュー担当者として割り当てられているアクセスレビューのためのものではありません。</span><span class="sxs-lookup"><span data-stu-id="2f454-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="2f454-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f454-109">Permissions</span></span>
<span data-ttu-id="2f454-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f454-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f454-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f454-112">Permission type</span></span>                        | <span data-ttu-id="2f454-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f454-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f454-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f454-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f454-115">accessreview すべて</span><span class="sxs-lookup"><span data-stu-id="2f454-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="2f454-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f454-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f454-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f454-117">Not supported.</span></span> |
|<span data-ttu-id="2f454-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f454-118">Application</span></span>                            | <span data-ttu-id="2f454-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f454-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f454-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f454-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="2f454-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f454-121">Request headers</span></span>
| <span data-ttu-id="2f454-122">名前</span><span class="sxs-lookup"><span data-stu-id="2f454-122">Name</span></span>         | <span data-ttu-id="2f454-123">型</span><span class="sxs-lookup"><span data-stu-id="2f454-123">Type</span></span>        | <span data-ttu-id="2f454-124">説明</span><span class="sxs-lookup"><span data-stu-id="2f454-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2f454-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f454-125">Authorization</span></span> | <span data-ttu-id="2f454-126">string</span><span class="sxs-lookup"><span data-stu-id="2f454-126">string</span></span> | <span data-ttu-id="2f454-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f454-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f454-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f454-129">Request body</span></span>
<span data-ttu-id="2f454-130">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="2f454-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="2f454-131">応答</span><span class="sxs-lookup"><span data-stu-id="2f454-131">Response</span></span>
<span data-ttu-id="2f454-132">成功した場合、このメソッドは200シリーズの応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2f454-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="2f454-133">例</span><span class="sxs-lookup"><span data-stu-id="2f454-133">Example</span></span>

<span data-ttu-id="2f454-134">これは、不要なレビューを削除するために、1回限り (定期的でない) アクセスレビューを更新する例です。</span><span class="sxs-lookup"><span data-stu-id="2f454-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="2f454-135">要求</span><span class="sxs-lookup"><span data-stu-id="2f454-135">Request</span></span>
<span data-ttu-id="2f454-136">要求 URL で、accessreview オブジェクトの id と、ユーザーオブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="2f454-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="2f454-137">応答</span><span class="sxs-lookup"><span data-stu-id="2f454-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
