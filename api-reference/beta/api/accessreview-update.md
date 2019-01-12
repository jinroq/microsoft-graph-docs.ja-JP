---
title: AccessReview を更新します。
description: Azure AD アクセスのレビュー機能では、1 つまたは複数のプロパティを変更するのには既存の accessReview オブジェクトを更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e09219c1979f974b62f17c52163fc93b5d2d3c2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941358"
---
# <a name="update-accessreview"></a><span data-ttu-id="8cb33-103">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="8cb33-103">Update accessReview</span></span>

> <span data-ttu-id="8cb33-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cb33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cb33-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cb33-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、1 つまたは複数のプロパティを変更するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="8cb33-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="8cb33-107">レビュー担当者やレビューの決定を変更するのには、この API は想定されていません。</span><span class="sxs-lookup"><span data-stu-id="8cb33-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="8cb33-108">レビュー担当者を変更するには、 [addReviewer](accessreview-addreviewer.md)または[removeReviewer](accessreview-removereviewer.md) Api を使用します。</span><span class="sxs-lookup"><span data-stu-id="8cb33-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="8cb33-109">すでに開始された 1 回限りのレビュー、または定期的なレビューの既に起動インスタンスを停止、[停止](accessreview-stop.md)API を使用して、初期の段階では、ターゲット ・ グループまたはアプリケーション アクセス権の決定に適用する、[適用](accessreview-apply.md)API を使用して、します。</span><span class="sxs-lookup"><span data-stu-id="8cb33-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API, and to apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="8cb33-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8cb33-110">Permissions</span></span>
<span data-ttu-id="8cb33-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cb33-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb33-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cb33-113">Permission type</span></span>                        | <span data-ttu-id="8cb33-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cb33-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cb33-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cb33-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cb33-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb33-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="8cb33-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cb33-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cb33-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb33-118">Not supported.</span></span> |
|<span data-ttu-id="8cb33-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cb33-119">Application</span></span>                            | <span data-ttu-id="8cb33-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb33-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cb33-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cb33-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="8cb33-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cb33-122">Request headers</span></span>
| <span data-ttu-id="8cb33-123">名前</span><span class="sxs-lookup"><span data-stu-id="8cb33-123">Name</span></span>         | <span data-ttu-id="8cb33-124">種類</span><span class="sxs-lookup"><span data-stu-id="8cb33-124">Type</span></span>        | <span data-ttu-id="8cb33-125">説明</span><span class="sxs-lookup"><span data-stu-id="8cb33-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8cb33-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb33-126">Authorization</span></span> | <span data-ttu-id="8cb33-127">string</span><span class="sxs-lookup"><span data-stu-id="8cb33-127">string</span></span> | <span data-ttu-id="8cb33-128">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="8cb33-128">Bearer \{token\}.</span></span> <span data-ttu-id="8cb33-129">必須。</span><span class="sxs-lookup"><span data-stu-id="8cb33-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cb33-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cb33-130">Request body</span></span>
<span data-ttu-id="8cb33-131">要求の本体の[accessReview](../resources/accessreview.md)オブジェクトのパラメーターの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cb33-131">In the request body, supply a JSON representation of a parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="8cb33-132">次の表は、accessReview を更新するときに指定できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="8cb33-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="8cb33-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cb33-133">Property</span></span>     | <span data-ttu-id="8cb33-134">種類</span><span class="sxs-lookup"><span data-stu-id="8cb33-134">Type</span></span>        | <span data-ttu-id="8cb33-135">説明</span><span class="sxs-lookup"><span data-stu-id="8cb33-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="8cb33-136">アクセス確認の名前です。</span><span class="sxs-lookup"><span data-stu-id="8cb33-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="8cb33-137">日付と時刻と、レビューを開始する予定です。</span><span class="sxs-lookup"><span data-stu-id="8cb33-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="8cb33-138">将来の日付でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8cb33-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="8cb33-139">レビューの終了がスケジュールされているときの日時。</span><span class="sxs-lookup"><span data-stu-id="8cb33-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="8cb33-140">これは、少なくとも 1 つの日を開始日より後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8cb33-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="8cb33-141">校閲者を表示する説明します。</span><span class="sxs-lookup"><span data-stu-id="8cb33-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="8cb33-142">応答</span><span class="sxs-lookup"><span data-stu-id="8cb33-142">Response</span></span>
<span data-ttu-id="8cb33-143">かどうかは成功すると、このメソッドが返されます、`204, Accepted`応答コードおよび応答の本文内の[accessReview](../resources/accessreview.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8cb33-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb33-144">例</span><span class="sxs-lookup"><span data-stu-id="8cb33-144">Example</span></span>

<span data-ttu-id="8cb33-145">これは、1 回限り (繰り返し発生しない) のアクセス確認の更新の例です。</span><span class="sxs-lookup"><span data-stu-id="8cb33-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="8cb33-146">要求</span><span class="sxs-lookup"><span data-stu-id="8cb33-146">Request</span></span>
<span data-ttu-id="8cb33-147">要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの新しいプロパティの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cb33-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8cb33-148">応答</span><span class="sxs-lookup"><span data-stu-id="8cb33-148">Response</span></span>
><span data-ttu-id="8cb33-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cb33-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
