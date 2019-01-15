---
title: AccessReview を取得します。
description: 'Azure AD のレビュー機能にアクセス、accessReview オブジェクトを取得します。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a13776b9aa215d752797b6ba2de2f477660ed31d
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016661"
---
# <a name="get-accessreview"></a><span data-ttu-id="6a913-103">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a913-103">Get accessReview</span></span>

> <span data-ttu-id="6a913-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a913-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a913-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a913-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a913-106">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [accessReview](../resources/accessreview.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="6a913-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="6a913-107">アクセス レビューのレビュー担当者を取得するには、 [accessReview の校閲者の一覧](accessreview-listreviewers.md)API を使用します。</span><span class="sxs-lookup"><span data-stu-id="6a913-107">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="6a913-108">アクセス レビューの決定を取得するには、 [] ボックスの一覧 accessReview の意思決定](accessreview-listdecisions.md)の API、または[私の accessReview の決定事項を表示](accessreview-listmydecisions.md)API を使用します。</span><span class="sxs-lookup"><span data-stu-id="6a913-108">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="6a913-109">定期的なアクセス確認の場合を使用して、`instances`までは、アクセス確認のインスタンスを現在および将来の[accessReview](../resources/accessreview.md)コレクションを取得するために関係します。</span><span class="sxs-lookup"><span data-stu-id="6a913-109">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a913-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a913-110">Permissions</span></span>
<span data-ttu-id="6a913-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a913-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a913-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a913-113">Permission type</span></span>                        | <span data-ttu-id="6a913-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a913-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a913-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a913-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a913-116">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="6a913-116"></span></span>  <span data-ttu-id="6a913-117">サインインしているユーザーは、ディレクトリの役割をアクセスのレビューを読むことを許可またはアクセスのレビューのレビュー担当者として割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a913-117">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="6a913-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a913-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a913-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a913-119">Not supported.</span></span> |
|<span data-ttu-id="6a913-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a913-120">Application</span></span>                            | <span data-ttu-id="6a913-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a913-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a913-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a913-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="6a913-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a913-123">Request headers</span></span>
| <span data-ttu-id="6a913-124">名前</span><span class="sxs-lookup"><span data-stu-id="6a913-124">Name</span></span>         | <span data-ttu-id="6a913-125">型</span><span class="sxs-lookup"><span data-stu-id="6a913-125">Type</span></span>        | <span data-ttu-id="6a913-126">説明</span><span class="sxs-lookup"><span data-stu-id="6a913-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6a913-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a913-127">Authorization</span></span> | <span data-ttu-id="6a913-128">string</span><span class="sxs-lookup"><span data-stu-id="6a913-128">string</span></span> | <span data-ttu-id="6a913-129">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="6a913-129">Bearer \{token\}.</span></span> <span data-ttu-id="6a913-130">必須。</span><span class="sxs-lookup"><span data-stu-id="6a913-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a913-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a913-131">Request body</span></span>
<span data-ttu-id="6a913-132">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="6a913-132">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="6a913-133">応答</span><span class="sxs-lookup"><span data-stu-id="6a913-133">Response</span></span>
<span data-ttu-id="6a913-134">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文内の[accessReview](../resources/accessreview.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6a913-134">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a913-135">例</span><span class="sxs-lookup"><span data-stu-id="6a913-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a913-136">要求</span><span class="sxs-lookup"><span data-stu-id="6a913-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="6a913-137">応答</span><span class="sxs-lookup"><span data-stu-id="6a913-137">Response</span></span>
><span data-ttu-id="6a913-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6a913-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="6a913-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a913-140">See also</span></span>

| <span data-ttu-id="6a913-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a913-141">Method</span></span>           | <span data-ttu-id="6a913-142">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6a913-142">Return Type</span></span>    |<span data-ttu-id="6a913-143">説明</span><span class="sxs-lookup"><span data-stu-id="6a913-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a913-144">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="6a913-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="6a913-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="6a913-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="6a913-146">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="6a913-146">Create a new accessReview.</span></span> |
|[<span data-ttu-id="6a913-147">リスト programControls</span><span class="sxs-lookup"><span data-stu-id="6a913-147">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="6a913-148">[デバッギング](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6a913-148">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="6a913-149">テナント内の programControls を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6a913-149">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="6a913-150">AccessReview の校閲者の一覧</span><span class="sxs-lookup"><span data-stu-id="6a913-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="6a913-151">コレクションを[割り当てられていません](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="6a913-151">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="6a913-152">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a913-152">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="6a913-153">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="6a913-153">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="6a913-154">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6a913-154">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="6a913-155">AccessReview の決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a913-155">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="6a913-156">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="6a913-156">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="6a913-157">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6a913-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="6a913-158">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a913-158">As a reviewer, get my decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
