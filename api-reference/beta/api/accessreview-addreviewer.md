---
title: AccessReview の校閲者を追加します。
description: 'Azure AD アクセスのレビュー機能では、レビュー担当者として他のユーザーを追加するのには既存の accessReview オブジェクトを更新します。  この操作のみ許可されてはまだ完了していない、アクセスの確認のためや、アクセスの確認にのみ、校閲者が明示的に指定されています。 この操作は、アクセス確認をユーザーが独自のアクセスを確認するには許可されませんし、校閲者として、グループの所有者が割り当てられている、アクセス確認のためではありません。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a526451330321c7fbbfd1d5287dd5ad892eee84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516365"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="8b8ce-105">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b8ce-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、レビュー担当者として他のユーザーを追加するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="8b8ce-107">この操作のみ許可されてはまだ完了していない、アクセスの確認のためや、アクセスの確認にのみ、校閲者が明示的に指定されています。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="8b8ce-108">この操作は、アクセス確認をユーザーが独自のアクセスを確認するには許可されませんし、校閲者として、グループの所有者が割り当てられている、アクセス確認のためではありません。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="8b8ce-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8b8ce-109">Permissions</span></span>
<span data-ttu-id="8b8ce-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b8ce-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b8ce-112">Permission type</span></span>                        | <span data-ttu-id="8b8ce-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b8ce-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b8ce-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b8ce-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b8ce-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b8ce-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="8b8ce-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b8ce-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b8ce-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-117">Not supported.</span></span> |
|<span data-ttu-id="8b8ce-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b8ce-118">Application</span></span>                            | <span data-ttu-id="8b8ce-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b8ce-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b8ce-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="8b8ce-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b8ce-121">Request headers</span></span>
| <span data-ttu-id="8b8ce-122">名前</span><span class="sxs-lookup"><span data-stu-id="8b8ce-122">Name</span></span>         | <span data-ttu-id="8b8ce-123">型</span><span class="sxs-lookup"><span data-stu-id="8b8ce-123">Type</span></span>        | <span data-ttu-id="8b8ce-124">説明</span><span class="sxs-lookup"><span data-stu-id="8b8ce-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8b8ce-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b8ce-125">Authorization</span></span> | <span data-ttu-id="8b8ce-126">string</span><span class="sxs-lookup"><span data-stu-id="8b8ce-126">string</span></span> | <span data-ttu-id="8b8ce-127">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="8b8ce-127">Bearer \{token\}.</span></span> <span data-ttu-id="8b8ce-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b8ce-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b8ce-129">Request body</span></span>
<span data-ttu-id="8b8ce-130">要求の本文には、校閲者となるユーザーの ID の JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="8b8ce-131">次の表は、accessReview を更新するときに指定できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="8b8ce-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b8ce-132">Property</span></span>     | <span data-ttu-id="8b8ce-133">型</span><span class="sxs-lookup"><span data-stu-id="8b8ce-133">Type</span></span>        | <span data-ttu-id="8b8ce-134">説明</span><span class="sxs-lookup"><span data-stu-id="8b8ce-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="8b8ce-135">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-135">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="8b8ce-136">応答</span><span class="sxs-lookup"><span data-stu-id="8b8ce-136">Response</span></span>
<span data-ttu-id="8b8ce-137">かどうかは成功すると、このメソッドが返されます、`201, Created`応答コード。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="8b8ce-138">例</span><span class="sxs-lookup"><span data-stu-id="8b8ce-138">Example</span></span>

<span data-ttu-id="8b8ce-139">これは、1 回限り (繰り返し発生しない) のアクセス確認をその他の校閲者の更新の例です。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="8b8ce-140">要求</span><span class="sxs-lookup"><span data-stu-id="8b8ce-140">Request</span></span>
<span data-ttu-id="8b8ce-141">要求の本文に、JSON 形式のユーザー オブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-141">In the request body, supply a JSON representation of the id of the user object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8b8ce-142">応答</span><span class="sxs-lookup"><span data-stu-id="8b8ce-142">Response</span></span>
><span data-ttu-id="8b8ce-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8b8ce-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
