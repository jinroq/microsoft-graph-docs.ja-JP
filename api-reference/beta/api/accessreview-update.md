---
title: AccessReview を更新します。
description: Azure AD アクセスのレビュー機能では、1 つまたは複数のプロパティを変更するのには既存の accessReview オブジェクトを更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1256ccdabea8eb5c0c0ffb3365e0c87276999236
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524367"
---
# <a name="update-accessreview"></a><span data-ttu-id="0a030-103">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="0a030-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a030-104">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、1 つまたは複数のプロパティを変更するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a030-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="0a030-105">レビュー担当者やレビューの決定を変更するのには、この API は想定されていません。</span><span class="sxs-lookup"><span data-stu-id="0a030-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="0a030-106">レビュー担当者を変更するには、 [addReviewer](accessreview-addreviewer.md)または[removeReviewer](accessreview-removereviewer.md) Api を使用します。</span><span class="sxs-lookup"><span data-stu-id="0a030-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="0a030-107">すでに開始された 1 回限りのレビュー、または定期的なレビューの既に起動インスタンスを停止するには、初期の段階では、[停止する](accessreview-stop.md)API を使用します。</span><span class="sxs-lookup"><span data-stu-id="0a030-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="0a030-108">ターゲット ・ グループ、またはアプリケーションのアクセス権の決定を適用するには、[適用](accessreview-apply.md)API を使用します。</span><span class="sxs-lookup"><span data-stu-id="0a030-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0a030-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a030-109">Permissions</span></span>
<span data-ttu-id="0a030-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a030-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a030-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a030-112">Permission type</span></span>                        | <span data-ttu-id="0a030-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a030-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a030-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a030-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a030-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a030-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0a030-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a030-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a030-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a030-117">Not supported.</span></span> |
|<span data-ttu-id="0a030-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a030-118">Application</span></span>                            | <span data-ttu-id="0a030-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a030-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a030-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a030-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="0a030-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a030-121">Request headers</span></span>
| <span data-ttu-id="0a030-122">名前</span><span class="sxs-lookup"><span data-stu-id="0a030-122">Name</span></span>         | <span data-ttu-id="0a030-123">型</span><span class="sxs-lookup"><span data-stu-id="0a030-123">Type</span></span>        | <span data-ttu-id="0a030-124">説明</span><span class="sxs-lookup"><span data-stu-id="0a030-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0a030-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a030-125">Authorization</span></span> | <span data-ttu-id="0a030-126">string</span><span class="sxs-lookup"><span data-stu-id="0a030-126">string</span></span> | <span data-ttu-id="0a030-127">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="0a030-127">Bearer \{token\}.</span></span> <span data-ttu-id="0a030-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="0a030-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a030-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a030-129">Request body</span></span>
<span data-ttu-id="0a030-130">要求の本文に、JSON 形式の[accessReview](../resources/accessreview.md)オブジェクトのパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a030-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="0a030-131">次の表は、accessReview を更新するときに指定できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="0a030-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="0a030-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a030-132">Property</span></span>     | <span data-ttu-id="0a030-133">型</span><span class="sxs-lookup"><span data-stu-id="0a030-133">Type</span></span>        | <span data-ttu-id="0a030-134">説明</span><span class="sxs-lookup"><span data-stu-id="0a030-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="0a030-135">アクセス確認の名前です。</span><span class="sxs-lookup"><span data-stu-id="0a030-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="0a030-136">日付と時刻と、レビューを開始する予定です。</span><span class="sxs-lookup"><span data-stu-id="0a030-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="0a030-137">将来の日付でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="0a030-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="0a030-138">レビューの終了がスケジュールされているときの日時。</span><span class="sxs-lookup"><span data-stu-id="0a030-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="0a030-139">これは、少なくとも 1 つの日を開始日より後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="0a030-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="0a030-140">校閲者を表示する説明します。</span><span class="sxs-lookup"><span data-stu-id="0a030-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="0a030-141">応答</span><span class="sxs-lookup"><span data-stu-id="0a030-141">Response</span></span>
<span data-ttu-id="0a030-142">かどうかは成功すると、このメソッドが返されます、`204, Accepted`応答コードおよび応答の本文内の[accessReview](../resources/accessreview.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0a030-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a030-143">例</span><span class="sxs-lookup"><span data-stu-id="0a030-143">Example</span></span>

<span data-ttu-id="0a030-144">これは、1 回限り (繰り返し発生しない) のアクセス確認の更新の例です。</span><span class="sxs-lookup"><span data-stu-id="0a030-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="0a030-145">要求</span><span class="sxs-lookup"><span data-stu-id="0a030-145">Request</span></span>
<span data-ttu-id="0a030-146">要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの新しいプロパティの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a030-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="0a030-147">応答</span><span class="sxs-lookup"><span data-stu-id="0a030-147">Response</span></span>
><span data-ttu-id="0a030-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0a030-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
