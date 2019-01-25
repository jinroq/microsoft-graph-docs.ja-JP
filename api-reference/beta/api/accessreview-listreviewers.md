---
title: AccessReview の校閲者の一覧
description: Azure AD にアクセスが機能を確認、校閲者の accessReview オブジェクトを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d2227ed6343900780df57aeece2fe511f07da04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529279"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="af60d-103">AccessReview の校閲者の一覧</span><span class="sxs-lookup"><span data-stu-id="af60d-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af60d-104">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、校閲者の[accessReview](../resources/accessreview.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="af60d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="af60d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af60d-105">Permissions</span></span>
<span data-ttu-id="af60d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af60d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af60d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af60d-108">Permission type</span></span>                        | <span data-ttu-id="af60d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="af60d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="af60d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af60d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="af60d-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="af60d-111"></span></span>  <span data-ttu-id="af60d-112">サインインしているユーザーは、ディレクトリの役割をアクセスのレビューを読むことを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="af60d-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="af60d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af60d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af60d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af60d-114">Not supported.</span></span> |
|<span data-ttu-id="af60d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af60d-115">Application</span></span>                            | <span data-ttu-id="af60d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af60d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af60d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af60d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="af60d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af60d-118">Request headers</span></span>
| <span data-ttu-id="af60d-119">名前</span><span class="sxs-lookup"><span data-stu-id="af60d-119">Name</span></span>         | <span data-ttu-id="af60d-120">型</span><span class="sxs-lookup"><span data-stu-id="af60d-120">Type</span></span>        | <span data-ttu-id="af60d-121">説明</span><span class="sxs-lookup"><span data-stu-id="af60d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="af60d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af60d-122">Authorization</span></span> | <span data-ttu-id="af60d-123">string</span><span class="sxs-lookup"><span data-stu-id="af60d-123">string</span></span> | <span data-ttu-id="af60d-124">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="af60d-124">Bearer \{token\}.</span></span> <span data-ttu-id="af60d-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="af60d-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af60d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="af60d-126">Request body</span></span>
<span data-ttu-id="af60d-127">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="af60d-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="af60d-128">応答</span><span class="sxs-lookup"><span data-stu-id="af60d-128">Response</span></span>
<span data-ttu-id="af60d-129">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[割り当てられていません](../resources/useridentity.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="af60d-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af60d-130">例</span><span class="sxs-lookup"><span data-stu-id="af60d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af60d-131">要求</span><span class="sxs-lookup"><span data-stu-id="af60d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="af60d-132">応答</span><span class="sxs-lookup"><span data-stu-id="af60d-132">Response</span></span>
><span data-ttu-id="af60d-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="af60d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="af60d-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="af60d-135">See also</span></span>

| <span data-ttu-id="af60d-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="af60d-136">Method</span></span>           | <span data-ttu-id="af60d-137">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="af60d-137">Return Type</span></span>    |<span data-ttu-id="af60d-138">説明</span><span class="sxs-lookup"><span data-stu-id="af60d-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af60d-139">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="af60d-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="af60d-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="af60d-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="af60d-141">アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="af60d-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="af60d-142">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="af60d-142">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="af60d-143">なし。</span><span class="sxs-lookup"><span data-stu-id="af60d-143">None.</span></span>   |   <span data-ttu-id="af60d-144">AccessReview には、レビュー担当者を追加します。</span><span class="sxs-lookup"><span data-stu-id="af60d-144">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="af60d-145">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="af60d-145">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="af60d-146">なし。</span><span class="sxs-lookup"><span data-stu-id="af60d-146">None.</span></span> |   <span data-ttu-id="af60d-147">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="af60d-147">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
