---
title: AccessReview を更新します。
description: Azure AD アクセスのレビュー機能では、1 つまたは複数のプロパティを変更するのには既存の accessReview オブジェクトを更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e4e74daa092c6f18c845c7f0c468af90385b899b
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016752"
---
# <a name="update-accessreview"></a><span data-ttu-id="cd519-103">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="cd519-103">Update accessReview</span></span>

> <span data-ttu-id="cd519-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd519-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd519-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd519-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd519-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、1 つまたは複数のプロパティを変更するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="cd519-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="cd519-107">レビュー担当者やレビューの決定を変更するのには、この API は想定されていません。</span><span class="sxs-lookup"><span data-stu-id="cd519-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="cd519-108">レビュー担当者を変更するには、 [addReviewer](accessreview-addreviewer.md)または[removeReviewer](accessreview-removereviewer.md) Api を使用します。</span><span class="sxs-lookup"><span data-stu-id="cd519-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="cd519-109">すでに開始された 1 回限りのレビュー、または定期的なレビューの既に起動インスタンスを停止するには、初期の段階では、[停止する](accessreview-stop.md)API を使用します。</span><span class="sxs-lookup"><span data-stu-id="cd519-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="cd519-110">ターゲット ・ グループ、またはアプリケーションのアクセス権の決定を適用するには、[適用](accessreview-apply.md)API を使用します。</span><span class="sxs-lookup"><span data-stu-id="cd519-110">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="cd519-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cd519-111">Permissions</span></span>
<span data-ttu-id="cd519-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd519-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd519-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd519-114">Permission type</span></span>                        | <span data-ttu-id="cd519-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd519-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd519-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd519-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd519-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd519-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="cd519-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd519-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd519-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd519-119">Not supported.</span></span> |
|<span data-ttu-id="cd519-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd519-120">Application</span></span>                            | <span data-ttu-id="cd519-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd519-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd519-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd519-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="cd519-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd519-123">Request headers</span></span>
| <span data-ttu-id="cd519-124">名前</span><span class="sxs-lookup"><span data-stu-id="cd519-124">Name</span></span>         | <span data-ttu-id="cd519-125">型</span><span class="sxs-lookup"><span data-stu-id="cd519-125">Type</span></span>        | <span data-ttu-id="cd519-126">説明</span><span class="sxs-lookup"><span data-stu-id="cd519-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cd519-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd519-127">Authorization</span></span> | <span data-ttu-id="cd519-128">string</span><span class="sxs-lookup"><span data-stu-id="cd519-128">string</span></span> | <span data-ttu-id="cd519-129">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="cd519-129">Bearer \{token\}.</span></span> <span data-ttu-id="cd519-130">必須。</span><span class="sxs-lookup"><span data-stu-id="cd519-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd519-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd519-131">Request body</span></span>
<span data-ttu-id="cd519-132">要求の本文に、JSON 形式の[accessReview](../resources/accessreview.md)オブジェクトのパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="cd519-132">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="cd519-133">次の表は、accessReview を更新するときに指定できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="cd519-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="cd519-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd519-134">Property</span></span>     | <span data-ttu-id="cd519-135">型</span><span class="sxs-lookup"><span data-stu-id="cd519-135">Type</span></span>        | <span data-ttu-id="cd519-136">説明</span><span class="sxs-lookup"><span data-stu-id="cd519-136">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="cd519-137">アクセス確認の名前です。</span><span class="sxs-lookup"><span data-stu-id="cd519-137">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="cd519-138">日付と時刻と、レビューを開始する予定です。</span><span class="sxs-lookup"><span data-stu-id="cd519-138">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="cd519-139">将来の日付でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="cd519-139">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="cd519-140">レビューの終了がスケジュールされているときの日時。</span><span class="sxs-lookup"><span data-stu-id="cd519-140">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="cd519-141">これは、少なくとも 1 つの日を開始日より後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="cd519-141">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="cd519-142">校閲者を表示する説明します。</span><span class="sxs-lookup"><span data-stu-id="cd519-142">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="cd519-143">応答</span><span class="sxs-lookup"><span data-stu-id="cd519-143">Response</span></span>
<span data-ttu-id="cd519-144">かどうかは成功すると、このメソッドが返されます、`204, Accepted`応答コードおよび応答の本文内の[accessReview](../resources/accessreview.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cd519-144">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd519-145">例</span><span class="sxs-lookup"><span data-stu-id="cd519-145">Example</span></span>

<span data-ttu-id="cd519-146">これは、1 回限り (繰り返し発生しない) のアクセス確認の更新の例です。</span><span class="sxs-lookup"><span data-stu-id="cd519-146">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="cd519-147">要求</span><span class="sxs-lookup"><span data-stu-id="cd519-147">Request</span></span>
<span data-ttu-id="cd519-148">要求の本文には、 [accessReview](../resources/accessreview.md)オブジェクトの新しいプロパティの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="cd519-148">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="cd519-149">応答</span><span class="sxs-lookup"><span data-stu-id="cd519-149">Response</span></span>
><span data-ttu-id="cd519-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cd519-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
