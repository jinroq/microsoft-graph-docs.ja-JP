---
title: accessReviewDecision リソースの種類
description: Azure AD にアクセス確認機能を`accessReviewDecision`、Azure AD アクセス確認意思決定の特定のエンティティへのアクセスを表します。  アクセス レビューの場合、または定期的なアクセス確認のインスタンスの中であり、1 つ`accessReviewDecision`確認済みのユーザー 1 人あたり。  などの 2 つのゲストと 1 つ、ゲスト、メンバー、および、アクセス レビュー来園者のグループがある場合は、そのグループのアクセス確認意思決定の 2 つのオブジェクトがありますし。  校閲者が自分の意思決定を変更または別の校閲者が、それらをオーバーライドする場合、`accessReviewDecision`を更新します。
localization_priority: Normal
ms.openlocfilehash: 208337f3427fad65499b400dee769d379c38dcb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870050"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="d877e-106">accessReviewDecision リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d877e-106">accessReviewDecision resource type</span></span>

> <span data-ttu-id="d877e-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d877e-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d877e-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d877e-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d877e-109">Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `accessReviewDecision` 、Azure AD アクセス確認意思決定の特定のエンティティへのアクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="d877e-109">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="d877e-110">アクセス レビューの場合、または定期的なアクセス確認のインスタンスの中であり、1 つ`accessReviewDecision`確認済みのユーザー 1 人あたり。</span><span class="sxs-lookup"><span data-stu-id="d877e-110">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="d877e-111">などの 2 つのゲストと 1 つ、ゲスト、メンバー、および、アクセス レビュー来園者のグループがある場合は、そのグループのアクセス確認意思決定の 2 つのオブジェクトがありますし。</span><span class="sxs-lookup"><span data-stu-id="d877e-111">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="d877e-112">校閲者が自分の意思決定を変更または別の校閲者が、それらをオーバーライドする場合、`accessReviewDecision`を更新します。</span><span class="sxs-lookup"><span data-stu-id="d877e-112">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="d877e-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="d877e-113">Methods</span></span>

<span data-ttu-id="d877e-114">なし</span><span class="sxs-lookup"><span data-stu-id="d877e-114">None.</span></span>  <span data-ttu-id="d877e-115">この型のオブジェクトが自動的に作成機能とアクセス確認の初期化、削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="d877e-115">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="d877e-116">それらは、[意思決定](../api/accessreview-listdecisions.md)と[mydecisions](../api/accessreview-listmydecisions.md)の関係を使用して、アクセスの確認から取得できます。</span><span class="sxs-lookup"><span data-stu-id="d877e-116">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="d877e-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d877e-117">Properties</span></span>

<span data-ttu-id="d877e-118">次の表は、この型のオブジェクトの基本プロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="d877e-118">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="d877e-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d877e-119">Property</span></span>                        | <span data-ttu-id="d877e-120">種類</span><span class="sxs-lookup"><span data-stu-id="d877e-120">Type</span></span>                         | <span data-ttu-id="d877e-121">説明</span><span class="sxs-lookup"><span data-stu-id="d877e-121">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="d877e-122">アクセス レビュー内での意思決定の id です。</span><span class="sxs-lookup"><span data-stu-id="d877e-122">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="d877e-123">アクセス レビューの機能によって生成された id です。</span><span class="sxs-lookup"><span data-stu-id="d877e-123">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="d877e-124">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="d877e-124">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="d877e-125">校閲者の id です。</span><span class="sxs-lookup"><span data-stu-id="d877e-125">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="d877e-126">日付と時刻の最新のレビューにアクセス権が指定されました。</span><span class="sxs-lookup"><span data-stu-id="d877e-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="d877e-127">レビューの結果です。</span><span class="sxs-lookup"><span data-stu-id="d877e-127">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="d877e-128">校閲者のビジネス ・ ジャスティフィケーションを提供された場合。</span><span class="sxs-lookup"><span data-stu-id="d877e-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="d877e-129">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="d877e-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="d877e-130">レビューの完了時、結果を手動で適用されていた場合、意思決定を適用したユーザーのユーザー id です。</span><span class="sxs-lookup"><span data-stu-id="d877e-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="d877e-131">日付と時刻確認の意思決定が適用されています。</span><span class="sxs-lookup"><span data-stu-id="d877e-131">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="d877e-132">いずれかの意思決定を適用した結果`NotApplied`、 `Success`、 `Failed`、`NotFound`または`NotSupported`。</span><span class="sxs-lookup"><span data-stu-id="d877e-132">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="d877e-133">機能で生成された推奨事項のいずれかの校閲者に示すように`Approve`、`Deny`または`NotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="d877e-133">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="d877e-134">さらに、追加のプロパティが決定されているアクセス権を持つオブジェクトのオブジェクトの種類によって表示されます。</span><span class="sxs-lookup"><span data-stu-id="d877e-134">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="d877e-135">たとえば、アクセス確認の意思決定が特定のユーザーのグループ メンバーシップ、またはアプリケーションへのアクセスの場合は、これらのプロパティを使用した可能性があるかのアクセスを削除するユーザーが識別されます。</span><span class="sxs-lookup"><span data-stu-id="d877e-135">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="d877e-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d877e-136">Property</span></span>                        | <span data-ttu-id="d877e-137">種類</span><span class="sxs-lookup"><span data-stu-id="d877e-137">Type</span></span>                         | <span data-ttu-id="d877e-138">説明</span><span class="sxs-lookup"><span data-stu-id="d877e-138">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="d877e-139">アクセス権が確認されたユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="d877e-139">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="d877e-140">アクセス権が確認されたユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="d877e-140">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="d877e-141">アクセス権が確認されたユーザーのユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="d877e-141">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="d877e-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d877e-142">Relationships</span></span>

<span data-ttu-id="d877e-143">なし。</span><span class="sxs-lookup"><span data-stu-id="d877e-143">None.</span></span>  <span data-ttu-id="d877e-144">この型のオブジェクトは、 [accessReview](accessreview.md)オブジェクトの[mydecisions](../api/accessreview-listmydecisions.md)の[意思決定](../api/accessreview-listdecisions.md)との関係を使用してアクセス確認から取得できます。</span><span class="sxs-lookup"><span data-stu-id="d877e-144">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="d877e-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="d877e-145">See also</span></span>

| <span data-ttu-id="d877e-146">メソッド</span><span class="sxs-lookup"><span data-stu-id="d877e-146">Method</span></span>           | <span data-ttu-id="d877e-147">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d877e-147">Return Type</span></span>    |<span data-ttu-id="d877e-148">説明</span><span class="sxs-lookup"><span data-stu-id="d877e-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d877e-149">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="d877e-149">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="d877e-150">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d877e-150">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="d877e-151">AccessReview の決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="d877e-151">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="d877e-152">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="d877e-152">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="d877e-153">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d877e-153">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="d877e-154">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="d877e-154">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d877e-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d877e-155">JSON representation</span></span>

<span data-ttu-id="d877e-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d877e-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
