---
title: accessreview を更新する
description: Azure AD access レビュー機能で、既存の accessreview オブジェクトを更新して、そのプロパティの1つ以上を変更します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1256ccdabea8eb5c0c0ffb3365e0c87276999236
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459445"
---
# <a name="update-accessreview"></a><span data-ttu-id="0635b-103">accessreview を更新する</span><span class="sxs-lookup"><span data-stu-id="0635b-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0635b-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[accessreview](../resources/accessreview.md)オブジェクトを更新して、そのプロパティの1つ以上を変更します。</span><span class="sxs-lookup"><span data-stu-id="0635b-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="0635b-105">この API は、レビュー担当者またはレビューの決定を変更するためのものではありません。</span><span class="sxs-lookup"><span data-stu-id="0635b-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="0635b-106">レビュー担当者を変更するには、 [addreviewer](accessreview-addreviewer.md)または[removereviewer](accessreview-removereviewer.md) api を使用します。</span><span class="sxs-lookup"><span data-stu-id="0635b-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="0635b-107">既に開始した1回限りのレビュー、または定期的なレビューの事前に開始されているインスタンスを停止するには、 [stop](accessreview-stop.md) API を使用します。</span><span class="sxs-lookup"><span data-stu-id="0635b-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="0635b-108">目的のグループまたはアプリのアクセス権に決定を適用するには、[API の[適用](accessreview-apply.md)] を使用します。</span><span class="sxs-lookup"><span data-stu-id="0635b-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0635b-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0635b-109">Permissions</span></span>
<span data-ttu-id="0635b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0635b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0635b-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0635b-112">Permission type</span></span>                        | <span data-ttu-id="0635b-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0635b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0635b-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0635b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0635b-115">accessreview すべて</span><span class="sxs-lookup"><span data-stu-id="0635b-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0635b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0635b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0635b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0635b-117">Not supported.</span></span> |
|<span data-ttu-id="0635b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0635b-118">Application</span></span>                            | <span data-ttu-id="0635b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0635b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0635b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0635b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="0635b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0635b-121">Request headers</span></span>
| <span data-ttu-id="0635b-122">名前</span><span class="sxs-lookup"><span data-stu-id="0635b-122">Name</span></span>         | <span data-ttu-id="0635b-123">型</span><span class="sxs-lookup"><span data-stu-id="0635b-123">Type</span></span>        | <span data-ttu-id="0635b-124">説明</span><span class="sxs-lookup"><span data-stu-id="0635b-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0635b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0635b-125">Authorization</span></span> | <span data-ttu-id="0635b-126">string</span><span class="sxs-lookup"><span data-stu-id="0635b-126">string</span></span> | <span data-ttu-id="0635b-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="0635b-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0635b-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0635b-129">Request body</span></span>
<span data-ttu-id="0635b-130">要求本文で、 [accessreview](../resources/accessreview.md)オブジェクトのパラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0635b-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="0635b-131">次の表に、accessreview の更新時に提供できるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0635b-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="0635b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0635b-132">Property</span></span>     | <span data-ttu-id="0635b-133">型</span><span class="sxs-lookup"><span data-stu-id="0635b-133">Type</span></span>        | <span data-ttu-id="0635b-134">説明</span><span class="sxs-lookup"><span data-stu-id="0635b-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="0635b-135">アクセスレビュー名。</span><span class="sxs-lookup"><span data-stu-id="0635b-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="0635b-136">レビューが開始される予定の日時。</span><span class="sxs-lookup"><span data-stu-id="0635b-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="0635b-137">これは、将来の日付である必要があります。</span><span class="sxs-lookup"><span data-stu-id="0635b-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="0635b-138">レビューが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="0635b-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="0635b-139">これは、開始日よりも1日以上後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="0635b-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="0635b-140">レビュー担当者に表示する説明。</span><span class="sxs-lookup"><span data-stu-id="0635b-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="0635b-141">応答</span><span class="sxs-lookup"><span data-stu-id="0635b-141">Response</span></span>
<span data-ttu-id="0635b-142">成功した場合、このメソッド`204, Accepted`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0635b-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0635b-143">例</span><span class="sxs-lookup"><span data-stu-id="0635b-143">Example</span></span>

<span data-ttu-id="0635b-144">これは、1回限り (定期的でない) アクセスレビューを更新する例です。</span><span class="sxs-lookup"><span data-stu-id="0635b-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="0635b-145">要求</span><span class="sxs-lookup"><span data-stu-id="0635b-145">Request</span></span>
<span data-ttu-id="0635b-146">要求本文で、 [accessreview](../resources/accessreview.md)オブジェクトの新しいプロパティの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0635b-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```

##### <a name="response"></a><span data-ttu-id="0635b-147">応答</span><span class="sxs-lookup"><span data-stu-id="0635b-147">Response</span></span>
><span data-ttu-id="0635b-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0635b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
