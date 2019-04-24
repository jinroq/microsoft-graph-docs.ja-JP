---
title: accessreview レビュー担当者のリスト
description: Azure AD access レビュー機能で、accessreview オブジェクトのレビュー担当者を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d2227ed6343900780df57aeece2fe511f07da04f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459417"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="dd559-103">accessreview レビュー担当者のリスト</span><span class="sxs-lookup"><span data-stu-id="dd559-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd559-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトのレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="dd559-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd559-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dd559-105">Permissions</span></span>
<span data-ttu-id="dd559-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd559-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dd559-108">Permission type</span></span>                        | <span data-ttu-id="dd559-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dd559-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd559-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dd559-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd559-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="dd559-111"></span></span>  <span data-ttu-id="dd559-112">サインインしているユーザーは、アクセスレビューを読み取ることができるようにするために、ディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd559-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="dd559-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dd559-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd559-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd559-114">Not supported.</span></span> |
|<span data-ttu-id="dd559-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dd559-115">Application</span></span>                            | <span data-ttu-id="dd559-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd559-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd559-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd559-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="dd559-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd559-118">Request headers</span></span>
| <span data-ttu-id="dd559-119">名前</span><span class="sxs-lookup"><span data-stu-id="dd559-119">Name</span></span>         | <span data-ttu-id="dd559-120">型</span><span class="sxs-lookup"><span data-stu-id="dd559-120">Type</span></span>        | <span data-ttu-id="dd559-121">説明</span><span class="sxs-lookup"><span data-stu-id="dd559-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dd559-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd559-122">Authorization</span></span> | <span data-ttu-id="dd559-123">string</span><span class="sxs-lookup"><span data-stu-id="dd559-123">string</span></span> | <span data-ttu-id="dd559-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="dd559-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd559-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dd559-126">Request body</span></span>
<span data-ttu-id="dd559-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="dd559-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="dd559-128">応答</span><span class="sxs-lookup"><span data-stu-id="dd559-128">Response</span></span>
<span data-ttu-id="dd559-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[useridentity](../resources/useridentity.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="dd559-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd559-130">例</span><span class="sxs-lookup"><span data-stu-id="dd559-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd559-131">要求</span><span class="sxs-lookup"><span data-stu-id="dd559-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="dd559-132">応答</span><span class="sxs-lookup"><span data-stu-id="dd559-132">Response</span></span>
><span data-ttu-id="dd559-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dd559-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dd559-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="dd559-135">See also</span></span>

| <span data-ttu-id="dd559-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="dd559-136">Method</span></span>           | <span data-ttu-id="dd559-137">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dd559-137">Return Type</span></span>    |<span data-ttu-id="dd559-138">説明</span><span class="sxs-lookup"><span data-stu-id="dd559-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd559-139">accessreview を取得する</span><span class="sxs-lookup"><span data-stu-id="dd559-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="dd559-140">accessreview</span><span class="sxs-lookup"><span data-stu-id="dd559-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="dd559-141">アクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="dd559-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="dd559-142">accessreview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="dd559-142">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="dd559-143">なし。</span><span class="sxs-lookup"><span data-stu-id="dd559-143">None.</span></span>   |   <span data-ttu-id="dd559-144">閲覧者を accessreview に追加します。</span><span class="sxs-lookup"><span data-stu-id="dd559-144">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="dd559-145">accessreview レビュー担当者を削除する</span><span class="sxs-lookup"><span data-stu-id="dd559-145">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="dd559-146">なし。</span><span class="sxs-lookup"><span data-stu-id="dd559-146">None.</span></span> |   <span data-ttu-id="dd559-147">accessreview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="dd559-147">Remove a reviewer from an accessReview.</span></span> |


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
