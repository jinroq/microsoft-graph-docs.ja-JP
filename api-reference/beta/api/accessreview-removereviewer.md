---
title: AccessReview のレビュー担当者を削除します。
description: 'Azure AD アクセスのレビュー機能では、レビュー担当者として、ユーザーを削除するのには既存の accessReview オブジェクトを更新します。  この操作のみ許可されてはまだ完了していない、アクセスの確認のためや、アクセスの確認にのみ、校閲者が明示的に指定されています。 この操作は、アクセス確認をユーザーが独自のアクセスを確認するには許可されませんし、校閲者として、グループの所有者が割り当てられている、アクセス確認のためではありません。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3b6ea0fecb6b9179f40fa185aa770a743776eaa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523128"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="02a60-105">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="02a60-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a60-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、レビュー担当者として、ユーザーを削除するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="02a60-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="02a60-107">この操作のみ許可されてはまだ完了していない、アクセスの確認のためや、アクセスの確認にのみ、校閲者が明示的に指定されています。</span><span class="sxs-lookup"><span data-stu-id="02a60-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="02a60-108">この操作は、アクセス確認をユーザーが独自のアクセスを確認するには許可されませんし、校閲者として、グループの所有者が割り当てられている、アクセス確認のためではありません。</span><span class="sxs-lookup"><span data-stu-id="02a60-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="02a60-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02a60-109">Permissions</span></span>
<span data-ttu-id="02a60-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02a60-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a60-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02a60-112">Permission type</span></span>                        | <span data-ttu-id="02a60-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02a60-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="02a60-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02a60-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="02a60-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a60-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="02a60-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02a60-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02a60-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02a60-117">Not supported.</span></span> |
|<span data-ttu-id="02a60-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02a60-118">Application</span></span>                            | <span data-ttu-id="02a60-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02a60-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02a60-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02a60-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="02a60-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02a60-121">Request headers</span></span>
| <span data-ttu-id="02a60-122">名前</span><span class="sxs-lookup"><span data-stu-id="02a60-122">Name</span></span>         | <span data-ttu-id="02a60-123">型</span><span class="sxs-lookup"><span data-stu-id="02a60-123">Type</span></span>        | <span data-ttu-id="02a60-124">説明</span><span class="sxs-lookup"><span data-stu-id="02a60-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="02a60-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a60-125">Authorization</span></span> | <span data-ttu-id="02a60-126">string</span><span class="sxs-lookup"><span data-stu-id="02a60-126">string</span></span> | <span data-ttu-id="02a60-127">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="02a60-127">Bearer \{token\}.</span></span> <span data-ttu-id="02a60-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="02a60-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02a60-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="02a60-129">Request body</span></span>
<span data-ttu-id="02a60-130">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="02a60-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="02a60-131">応答</span><span class="sxs-lookup"><span data-stu-id="02a60-131">Response</span></span>
<span data-ttu-id="02a60-132">成功した場合、このメソッドは、200 シリーズの応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="02a60-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="02a60-133">例</span><span class="sxs-lookup"><span data-stu-id="02a60-133">Example</span></span>

<span data-ttu-id="02a60-134">これは、不要なのレビュー担当者を削除するのには 1 回限り (繰り返し発生しない) アクセス レビューの更新の例です。</span><span class="sxs-lookup"><span data-stu-id="02a60-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="02a60-135">要求</span><span class="sxs-lookup"><span data-stu-id="02a60-135">Request</span></span>
<span data-ttu-id="02a60-136">要求の URL では、accessReview オブジェクトの id と、ユーザー オブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="02a60-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="02a60-137">応答</span><span class="sxs-lookup"><span data-stu-id="02a60-137">Response</span></span>
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
