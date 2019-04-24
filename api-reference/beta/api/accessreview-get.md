---
title: accessreview を取得する
description: 'Azure AD access レビュー機能で、accessreview オブジェクトを取得します。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26551f27fdf328865509cd02011f3ee2344f5e82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458769"
---
# <a name="get-accessreview"></a><span data-ttu-id="89e32-103">accessreview を取得する</span><span class="sxs-lookup"><span data-stu-id="89e32-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89e32-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="89e32-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="89e32-105">アクセスレビューのレビュー担当者を取得するには、 [list accessreview レビューアー](accessreview-listreviewers.md) API を使用します。</span><span class="sxs-lookup"><span data-stu-id="89e32-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="89e32-106">アクセスレビューの決定を取得するには、「[リストアクセスレビュー決定](accessreview-listdecisions.md)api」、または「 [my accessreview review 決定](accessreview-listmydecisions.md)api の一覧」を使用します。</span><span class="sxs-lookup"><span data-stu-id="89e32-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="89e32-107">これが定期的なアクセスレビューである場合は、 `instances`リレーションシップを使用して、アクセスレビューの過去、現在、および今後のインスタンスの[accessreview](../resources/accessreview.md)コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="89e32-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="89e32-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89e32-108">Permissions</span></span>
<span data-ttu-id="89e32-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89e32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e32-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89e32-111">Permission type</span></span>                        | <span data-ttu-id="89e32-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89e32-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="89e32-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89e32-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="89e32-114">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="89e32-114"></span></span>  <span data-ttu-id="89e32-115">また、サインインしているユーザーは、アクセスレビューを読み取ることを許可するか、またはアクセスレビューのレビュー担当者として割り当てられるディレクトリロールにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="89e32-115">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="89e32-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89e32-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89e32-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89e32-117">Not supported.</span></span> |
|<span data-ttu-id="89e32-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89e32-118">Application</span></span>                            | <span data-ttu-id="89e32-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89e32-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89e32-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89e32-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="89e32-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89e32-121">Request headers</span></span>
| <span data-ttu-id="89e32-122">名前</span><span class="sxs-lookup"><span data-stu-id="89e32-122">Name</span></span>         | <span data-ttu-id="89e32-123">型</span><span class="sxs-lookup"><span data-stu-id="89e32-123">Type</span></span>        | <span data-ttu-id="89e32-124">説明</span><span class="sxs-lookup"><span data-stu-id="89e32-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="89e32-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="89e32-125">Authorization</span></span> | <span data-ttu-id="89e32-126">string</span><span class="sxs-lookup"><span data-stu-id="89e32-126">string</span></span> | <span data-ttu-id="89e32-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="89e32-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89e32-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="89e32-129">Request body</span></span>
<span data-ttu-id="89e32-130">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="89e32-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="89e32-131">応答</span><span class="sxs-lookup"><span data-stu-id="89e32-131">Response</span></span>
<span data-ttu-id="89e32-132">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89e32-132">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89e32-133">例</span><span class="sxs-lookup"><span data-stu-id="89e32-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89e32-134">要求</span><span class="sxs-lookup"><span data-stu-id="89e32-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="89e32-135">応答</span><span class="sxs-lookup"><span data-stu-id="89e32-135">Response</span></span>
><span data-ttu-id="89e32-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="89e32-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="89e32-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="89e32-138">See also</span></span>

| <span data-ttu-id="89e32-139">メソッド</span><span class="sxs-lookup"><span data-stu-id="89e32-139">Method</span></span>           | <span data-ttu-id="89e32-140">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="89e32-140">Return Type</span></span>    |<span data-ttu-id="89e32-141">説明</span><span class="sxs-lookup"><span data-stu-id="89e32-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89e32-142">accessreview を作成する</span><span class="sxs-lookup"><span data-stu-id="89e32-142">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="89e32-143">accessreview</span><span class="sxs-lookup"><span data-stu-id="89e32-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="89e32-144">新しい accessreview を作成します。</span><span class="sxs-lookup"><span data-stu-id="89e32-144">Create a new accessReview.</span></span> |
|[<span data-ttu-id="89e32-145">programcontrols のリスト</span><span class="sxs-lookup"><span data-stu-id="89e32-145">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="89e32-146">[programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89e32-146">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="89e32-147">テナント内の programcontrols を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="89e32-147">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="89e32-148">accessreview レビュー担当者のリスト</span><span class="sxs-lookup"><span data-stu-id="89e32-148">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="89e32-149">[useridentity](../resources/useridentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89e32-149">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="89e32-150">accessreview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="89e32-150">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="89e32-151">accessreview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="89e32-151">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="89e32-152">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89e32-152">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="89e32-153">accessreview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="89e32-153">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="89e32-154">自分の accessreview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="89e32-154">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="89e32-155">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89e32-155">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="89e32-156">レビュー担当者として、accessreview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="89e32-156">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
