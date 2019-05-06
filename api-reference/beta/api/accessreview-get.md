---
title: AccessReview を取得する
description: 'Azure AD access レビュー機能で、accessReview オブジェクトを取得します。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a6df4461144f6823378ae16b93ff68dbee4c2413
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586282"
---
# <a name="get-accessreview"></a><span data-ttu-id="030c8-103">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="030c8-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="030c8-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="030c8-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="030c8-105">アクセスレビューのレビュー担当者を取得するには、 [List accessreview レビューアー](accessreview-listreviewers.md) API を使用します。</span><span class="sxs-lookup"><span data-stu-id="030c8-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="030c8-106">アクセスレビューの決定を取得するには、「[リストアクセスレビュー決定](accessreview-listdecisions.md)api」、または「 [My accessreview review 決定](accessreview-listmydecisions.md)api の一覧」を使用します。</span><span class="sxs-lookup"><span data-stu-id="030c8-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="030c8-107">これが定期的なアクセスレビューである場合は、 `instances`リレーションシップを使用して、アクセスレビューの過去、現在、および今後のインスタンスの[accessreview](../resources/accessreview.md)コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="030c8-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="030c8-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="030c8-108">Permissions</span></span>
<span data-ttu-id="030c8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="030c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="030c8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="030c8-111">Permission type</span></span>                        | <span data-ttu-id="030c8-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="030c8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="030c8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="030c8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="030c8-114">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="030c8-114">AccessReview.Read.All</span></span>  |
|<span data-ttu-id="030c8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="030c8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="030c8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="030c8-116">Not supported.</span></span> |
|<span data-ttu-id="030c8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="030c8-117">Application</span></span>                            | <span data-ttu-id="030c8-118">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="030c8-118">AccessReview.Read.All</span></span>  |

<span data-ttu-id="030c8-119">この API を呼び出すためには、サインインしているユーザーが、アクセスレビューを読み取ることを許可するディレクトリロールにあるか、アクセスレビューのレビュー担当者としてユーザーを割り当てることも必要です。</span><span class="sxs-lookup"><span data-stu-id="030c8-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="030c8-120">詳細については、「[アクセスレビュー](../resources/accessreviews-root.md)の役割とアクセス許可の要件」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="030c8-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="030c8-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="030c8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="030c8-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="030c8-122">Request headers</span></span>
| <span data-ttu-id="030c8-123">名前</span><span class="sxs-lookup"><span data-stu-id="030c8-123">Name</span></span>         | <span data-ttu-id="030c8-124">型</span><span class="sxs-lookup"><span data-stu-id="030c8-124">Type</span></span>        | <span data-ttu-id="030c8-125">説明</span><span class="sxs-lookup"><span data-stu-id="030c8-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="030c8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="030c8-126">Authorization</span></span> | <span data-ttu-id="030c8-127">string</span><span class="sxs-lookup"><span data-stu-id="030c8-127">string</span></span> | <span data-ttu-id="030c8-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="030c8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="030c8-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="030c8-130">Request body</span></span>
<span data-ttu-id="030c8-131">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="030c8-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="030c8-132">応答</span><span class="sxs-lookup"><span data-stu-id="030c8-132">Response</span></span>
<span data-ttu-id="030c8-133">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[accessreview](../resources/accessreview.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="030c8-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="030c8-134">例</span><span class="sxs-lookup"><span data-stu-id="030c8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="030c8-135">要求</span><span class="sxs-lookup"><span data-stu-id="030c8-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```

##### <a name="response"></a><span data-ttu-id="030c8-136">応答</span><span class="sxs-lookup"><span data-stu-id="030c8-136">Response</span></span>
><span data-ttu-id="030c8-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="030c8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="030c8-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="030c8-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="030c8-140">Visual</span><span class="sxs-lookup"><span data-stu-id="030c8-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="030c8-141">Java</span><span class="sxs-lookup"><span data-stu-id="030c8-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="030c8-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="030c8-142">See also</span></span>

| <span data-ttu-id="030c8-143">メソッド</span><span class="sxs-lookup"><span data-stu-id="030c8-143">Method</span></span>           | <span data-ttu-id="030c8-144">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="030c8-144">Return Type</span></span>    |<span data-ttu-id="030c8-145">説明</span><span class="sxs-lookup"><span data-stu-id="030c8-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="030c8-146">AccessReview を作成する</span><span class="sxs-lookup"><span data-stu-id="030c8-146">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="030c8-147">accessReview</span><span class="sxs-lookup"><span data-stu-id="030c8-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="030c8-148">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="030c8-148">Create a new accessReview.</span></span> |
|[<span data-ttu-id="030c8-149">ProgramControls のリスト</span><span class="sxs-lookup"><span data-stu-id="030c8-149">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="030c8-150">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="030c8-150">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="030c8-151">テナント内の programControls を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="030c8-151">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="030c8-152">AccessReview レビュー担当者のリスト</span><span class="sxs-lookup"><span data-stu-id="030c8-152">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="030c8-153">[Useridentity](../resources/useridentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="030c8-153">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="030c8-154">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="030c8-154">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="030c8-155">AccessReview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="030c8-155">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="030c8-156">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="030c8-156">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="030c8-157">AccessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="030c8-157">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="030c8-158">自分の accessReview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="030c8-158">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="030c8-159">[accessReviewDecision](../resources/accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="030c8-159">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="030c8-160">レビュー担当者として、accessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="030c8-160">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
