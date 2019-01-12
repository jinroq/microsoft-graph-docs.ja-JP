---
title: accessReviewDecision リソースの種類
description: Azure AD にアクセス確認機能を`accessReviewDecision`、Azure AD アクセス確認意思決定の特定のエンティティへのアクセスを表します。  アクセス レビューの場合、または定期的なアクセス確認のインスタンスの中であり、1 つ`accessReviewDecision`確認済みのユーザー 1 人あたり。  などの 2 つのゲストと 1 つ、ゲスト、メンバー、および、アクセス レビュー来園者のグループがある場合は、そのグループのアクセス確認意思決定の 2 つのオブジェクトがありますし。  校閲者が自分の意思決定を変更または別の校閲者が、それらをオーバーライドする場合、`accessReviewDecision`を更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b10a53726e12c37a598f8df735a3f70174c807
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977557"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="09f81-106">accessReviewDecision リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09f81-106">accessReviewDecision resource type</span></span>

> <span data-ttu-id="09f81-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09f81-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09f81-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09f81-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09f81-109">Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `accessReviewDecision` 、Azure AD アクセス確認意思決定の特定のエンティティへのアクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="09f81-109">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="09f81-110">アクセス レビューの場合、または定期的なアクセス確認のインスタンスの中であり、1 つ`accessReviewDecision`確認済みのユーザー 1 人あたり。</span><span class="sxs-lookup"><span data-stu-id="09f81-110">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="09f81-111">などの 2 つのゲストと 1 つ、ゲスト、メンバー、および、アクセス レビュー来園者のグループがある場合は、そのグループのアクセス確認意思決定の 2 つのオブジェクトがありますし。</span><span class="sxs-lookup"><span data-stu-id="09f81-111">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="09f81-112">校閲者が自分の意思決定を変更または別の校閲者が、それらをオーバーライドする場合、`accessReviewDecision`を更新します。</span><span class="sxs-lookup"><span data-stu-id="09f81-112">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="09f81-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="09f81-113">Methods</span></span>

<span data-ttu-id="09f81-114">なし</span><span class="sxs-lookup"><span data-stu-id="09f81-114">None.</span></span>  <span data-ttu-id="09f81-115">この型のオブジェクトが自動的に作成機能とアクセス確認の初期化、削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="09f81-115">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="09f81-116">それらは、[意思決定](../api/accessreview-listdecisions.md)と[mydecisions](../api/accessreview-listmydecisions.md)の関係を使用して、アクセスの確認から取得できます。</span><span class="sxs-lookup"><span data-stu-id="09f81-116">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="09f81-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09f81-117">Properties</span></span>

<span data-ttu-id="09f81-118">次の表は、この型のオブジェクトの基本プロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="09f81-118">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="09f81-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09f81-119">Property</span></span>                        | <span data-ttu-id="09f81-120">型</span><span class="sxs-lookup"><span data-stu-id="09f81-120">Type</span></span>                         | <span data-ttu-id="09f81-121">説明</span><span class="sxs-lookup"><span data-stu-id="09f81-121">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="09f81-122">アクセス レビュー内での意思決定の id です。</span><span class="sxs-lookup"><span data-stu-id="09f81-122">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="09f81-123">アクセス レビューの機能によって生成された id です。</span><span class="sxs-lookup"><span data-stu-id="09f81-123">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="09f81-124">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="09f81-124">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="09f81-125">校閲者の id です。</span><span class="sxs-lookup"><span data-stu-id="09f81-125">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="09f81-126">日付と時刻の最新のレビューにアクセス権が指定されました。</span><span class="sxs-lookup"><span data-stu-id="09f81-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="09f81-127">レビューの結果です。</span><span class="sxs-lookup"><span data-stu-id="09f81-127">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="09f81-128">校閲者のビジネス ・ ジャスティフィケーションを提供された場合。</span><span class="sxs-lookup"><span data-stu-id="09f81-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="09f81-129">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="09f81-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="09f81-130">レビューの完了時、結果を手動で適用されていた場合、意思決定を適用したユーザーのユーザー id です。</span><span class="sxs-lookup"><span data-stu-id="09f81-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="09f81-131">日付と時刻確認の意思決定が適用されています。</span><span class="sxs-lookup"><span data-stu-id="09f81-131">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="09f81-132">いずれかの意思決定を適用した結果`NotApplied`、 `Success`、 `Failed`、`NotFound`または`NotSupported`。</span><span class="sxs-lookup"><span data-stu-id="09f81-132">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="09f81-133">機能で生成された推奨事項のいずれかの校閲者に示すように`Approve`、`Deny`または`NotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="09f81-133">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="09f81-134">さらに、追加のプロパティが決定されているアクセス権を持つオブジェクトのオブジェクトの種類によって表示されます。</span><span class="sxs-lookup"><span data-stu-id="09f81-134">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="09f81-135">たとえば、アクセス確認の意思決定が特定のユーザーのグループ メンバーシップ、またはアプリケーションへのアクセスの場合は、これらのプロパティを使用した可能性があるかのアクセスを削除するユーザーが識別されます。</span><span class="sxs-lookup"><span data-stu-id="09f81-135">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="09f81-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09f81-136">Property</span></span>                        | <span data-ttu-id="09f81-137">型</span><span class="sxs-lookup"><span data-stu-id="09f81-137">Type</span></span>                         | <span data-ttu-id="09f81-138">説明</span><span class="sxs-lookup"><span data-stu-id="09f81-138">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="09f81-139">アクセス権が確認されたユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="09f81-139">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="09f81-140">アクセス権が確認されたユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="09f81-140">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="09f81-141">アクセス権が確認されたユーザーのユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="09f81-141">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="09f81-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09f81-142">Relationships</span></span>

<span data-ttu-id="09f81-143">なし。</span><span class="sxs-lookup"><span data-stu-id="09f81-143">None.</span></span>  <span data-ttu-id="09f81-144">この型のオブジェクトは、 [accessReview](accessreview.md)オブジェクトの[mydecisions](../api/accessreview-listmydecisions.md)の[意思決定](../api/accessreview-listdecisions.md)との関係を使用してアクセス確認から取得できます。</span><span class="sxs-lookup"><span data-stu-id="09f81-144">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="09f81-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="09f81-145">See also</span></span>

| <span data-ttu-id="09f81-146">メソッド</span><span class="sxs-lookup"><span data-stu-id="09f81-146">Method</span></span>           | <span data-ttu-id="09f81-147">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="09f81-147">Return Type</span></span>    |<span data-ttu-id="09f81-148">説明</span><span class="sxs-lookup"><span data-stu-id="09f81-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09f81-149">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="09f81-149">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="09f81-150">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09f81-150">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="09f81-151">AccessReview の決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="09f81-151">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="09f81-152">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="09f81-152">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="09f81-153">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09f81-153">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="09f81-154">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="09f81-154">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09f81-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09f81-155">JSON representation</span></span>

<span data-ttu-id="09f81-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09f81-156">Here is a JSON representation of the resource.</span></span>

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
