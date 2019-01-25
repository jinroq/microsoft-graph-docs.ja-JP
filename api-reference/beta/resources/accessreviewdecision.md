---
title: accessReviewDecision リソースの種類
description: Azure AD にアクセス確認機能を`accessReviewDecision`、Azure AD アクセス確認意思決定の特定のエンティティへのアクセスを表します。  アクセス レビューの場合、または定期的なアクセス確認のインスタンスの中であり、1 つ`accessReviewDecision`確認済みのユーザー 1 人あたり。  などの 2 つのゲストと 1 つ、ゲスト、メンバー、および、アクセス レビュー来園者のグループがある場合は、そのグループのアクセス確認意思決定の 2 つのオブジェクトがありますし。  校閲者が自分の意思決定を変更または別の校閲者が、それらをオーバーライドする場合、`accessReviewDecision`を更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9642c8a51e4e9efe1a1748243b0e24aeff07cfa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517401"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="91b21-106">accessReviewDecision リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91b21-106">accessReviewDecision resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b21-107">Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `accessReviewDecision` 、Azure AD アクセス確認意思決定の特定のエンティティへのアクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="91b21-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="91b21-108">アクセス レビューの場合、または定期的なアクセス確認のインスタンスの中であり、1 つ`accessReviewDecision`確認済みのユーザー 1 人あたり。</span><span class="sxs-lookup"><span data-stu-id="91b21-108">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="91b21-109">などの 2 つのゲストと 1 つ、ゲスト、メンバー、および、アクセス レビュー来園者のグループがある場合は、そのグループのアクセス確認意思決定の 2 つのオブジェクトがありますし。</span><span class="sxs-lookup"><span data-stu-id="91b21-109">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="91b21-110">校閲者が自分の意思決定を変更または別の校閲者が、それらをオーバーライドする場合、`accessReviewDecision`を更新します。</span><span class="sxs-lookup"><span data-stu-id="91b21-110">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="91b21-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="91b21-111">Methods</span></span>

<span data-ttu-id="91b21-112">なし</span><span class="sxs-lookup"><span data-stu-id="91b21-112">None.</span></span>  <span data-ttu-id="91b21-113">この型のオブジェクトが自動的に作成機能とアクセス確認の初期化、削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="91b21-113">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="91b21-114">それらは、[意思決定](../api/accessreview-listdecisions.md)と[mydecisions](../api/accessreview-listmydecisions.md)の関係を使用して、アクセスの確認から取得できます。</span><span class="sxs-lookup"><span data-stu-id="91b21-114">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="91b21-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91b21-115">Properties</span></span>

<span data-ttu-id="91b21-116">次の表は、この型のオブジェクトの基本プロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="91b21-116">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="91b21-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91b21-117">Property</span></span>                        | <span data-ttu-id="91b21-118">型</span><span class="sxs-lookup"><span data-stu-id="91b21-118">Type</span></span>                         | <span data-ttu-id="91b21-119">説明</span><span class="sxs-lookup"><span data-stu-id="91b21-119">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="91b21-120">アクセス レビュー内での意思決定の id です。</span><span class="sxs-lookup"><span data-stu-id="91b21-120">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="91b21-121">アクセス レビューの機能によって生成された id です。</span><span class="sxs-lookup"><span data-stu-id="91b21-121">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |<span data-ttu-id="91b21-122">%__UserIdentity__%</span><span class="sxs-lookup"><span data-stu-id="91b21-122">[userIdentity](useridentity.md)</span></span>| <span data-ttu-id="91b21-123">校閲者の id です。</span><span class="sxs-lookup"><span data-stu-id="91b21-123">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="91b21-124">日付と時刻の最新のレビューにアクセス権が指定されました。</span><span class="sxs-lookup"><span data-stu-id="91b21-124">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="91b21-125">レビューの結果です。</span><span class="sxs-lookup"><span data-stu-id="91b21-125">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="91b21-126">校閲者のビジネス ・ ジャスティフィケーションを提供された場合。</span><span class="sxs-lookup"><span data-stu-id="91b21-126">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |<span data-ttu-id="91b21-127">%__UserIdentity__%</span><span class="sxs-lookup"><span data-stu-id="91b21-127">[userIdentity](useridentity.md)</span></span>| <span data-ttu-id="91b21-128">レビューの完了時、結果を手動で適用されていた場合、意思決定を適用したユーザーのユーザー id です。</span><span class="sxs-lookup"><span data-stu-id="91b21-128">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="91b21-129">日付と時刻確認の意思決定が適用されています。</span><span class="sxs-lookup"><span data-stu-id="91b21-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="91b21-130">いずれかの意思決定を適用した結果`NotApplied`、 `Success`、 `Failed`、`NotFound`または`NotSupported`。</span><span class="sxs-lookup"><span data-stu-id="91b21-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="91b21-131">機能で生成された推奨事項のいずれかの校閲者に示すように`Approve`、`Deny`または`NotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="91b21-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="91b21-132">さらに、追加のプロパティが決定されているアクセス権を持つオブジェクトのオブジェクトの種類によって表示されます。</span><span class="sxs-lookup"><span data-stu-id="91b21-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="91b21-133">たとえば、アクセス確認の意思決定が特定のユーザーのグループ メンバーシップ、またはアプリケーションへのアクセスの場合は、これらのプロパティを使用した可能性があるかのアクセスを削除するユーザーが識別されます。</span><span class="sxs-lookup"><span data-stu-id="91b21-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="91b21-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91b21-134">Property</span></span>                        | <span data-ttu-id="91b21-135">型</span><span class="sxs-lookup"><span data-stu-id="91b21-135">Type</span></span>                         | <span data-ttu-id="91b21-136">説明</span><span class="sxs-lookup"><span data-stu-id="91b21-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="91b21-137">アクセス権が確認されたユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="91b21-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="91b21-138">アクセス権が確認されたユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="91b21-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="91b21-139">アクセス権が確認されたユーザーのユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="91b21-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="91b21-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91b21-140">Relationships</span></span>

<span data-ttu-id="91b21-141">なし。</span><span class="sxs-lookup"><span data-stu-id="91b21-141">None.</span></span>  <span data-ttu-id="91b21-142">この型のオブジェクトは、 [accessReview](accessreview.md)オブジェクトの[mydecisions](../api/accessreview-listmydecisions.md)の[意思決定](../api/accessreview-listdecisions.md)との関係を使用してアクセス確認から取得できます。</span><span class="sxs-lookup"><span data-stu-id="91b21-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="91b21-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="91b21-143">See also</span></span>

| <span data-ttu-id="91b21-144">メソッド</span><span class="sxs-lookup"><span data-stu-id="91b21-144">Method</span></span>           | <span data-ttu-id="91b21-145">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="91b21-145">Return Type</span></span>    |<span data-ttu-id="91b21-146">説明</span><span class="sxs-lookup"><span data-stu-id="91b21-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91b21-147">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="91b21-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="91b21-148">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="91b21-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="91b21-149">AccessReview の決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="91b21-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="91b21-150">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="91b21-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="91b21-151">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="91b21-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="91b21-152">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="91b21-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91b21-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91b21-153">JSON representation</span></span>

<span data-ttu-id="91b21-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91b21-154">Here is a JSON representation of the resource.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviewdecision.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
