---
title: accessReviewDecision リソースの種類
description: Azure AD access レビュー機能では、は`accessReviewDecision`特定のエンティティのアクセスに対する azure ad アクセスレビューの決定を表します。  アクセスレビュー、または定期的なアクセスレビューのインスタンスでは、レビュー対象の`accessReviewDecision`ユーザーごとに1つあります。  たとえば、グループに2人のゲストとゲスト以外のゲストがメンバーとして設定されている場合、そのグループに対してゲストのアクセスレビューが行われると、2つのアクセスレビューの決定オブジェクトがあります。  レビュー担当者が決定を変更した場合、または別の`accessReviewDecision`レビュー担当者がそれを上書きした場合は、が更新されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 034ecbdaa108d0c63378d1c00136f0415019b262
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657743"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="deb6b-106">accessReviewDecision リソースの種類</span><span class="sxs-lookup"><span data-stu-id="deb6b-106">accessReviewDecision resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deb6b-107">Azure AD [access レビュー](accessreviews-root.md)機能では、は`accessReviewDecision`特定のエンティティのアクセスに対する azure ad アクセスレビューの決定を表します。</span><span class="sxs-lookup"><span data-stu-id="deb6b-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="deb6b-108">アクセスレビュー、または定期的なアクセスレビューのインスタンスでは、レビュー対象の`accessReviewDecision`ユーザーごとに1つあります。</span><span class="sxs-lookup"><span data-stu-id="deb6b-108">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="deb6b-109">たとえば、グループに2人のゲストとゲスト以外のゲストがメンバーとして設定されている場合、そのグループに対してゲストのアクセスレビューが行われると、2つのアクセスレビューの決定オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="deb6b-109">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="deb6b-110">レビュー担当者が決定を変更した場合、または別の`accessReviewDecision`レビュー担当者がそれを上書きした場合は、が更新されます。</span><span class="sxs-lookup"><span data-stu-id="deb6b-110">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="deb6b-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="deb6b-111">Methods</span></span>

<span data-ttu-id="deb6b-112">なし。</span><span class="sxs-lookup"><span data-stu-id="deb6b-112">None.</span></span>  <span data-ttu-id="deb6b-113">この種類のオブジェクトは、アクセスレビューの初期化時にフィーチャーによって自動的に作成され、削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="deb6b-113">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="deb6b-114">これらは、[決定](../api/accessreview-listdecisions.md)と[mydecisions](../api/accessreview-listmydecisions.md)の関係を使用して、アクセスレビューから取得できます。</span><span class="sxs-lookup"><span data-stu-id="deb6b-114">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="deb6b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="deb6b-115">Properties</span></span>

<span data-ttu-id="deb6b-116">この表は、この種類のオブジェクトの基本プロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="deb6b-116">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="deb6b-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="deb6b-117">Property</span></span>                        | <span data-ttu-id="deb6b-118">型</span><span class="sxs-lookup"><span data-stu-id="deb6b-118">Type</span></span>                         | <span data-ttu-id="deb6b-119">説明</span><span class="sxs-lookup"><span data-stu-id="deb6b-119">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="deb6b-120">アクセスレビュー内での決定の id。</span><span class="sxs-lookup"><span data-stu-id="deb6b-120">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="deb6b-121">アクセスレビューのフィーチャー生成された id。</span><span class="sxs-lookup"><span data-stu-id="deb6b-121">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="deb6b-122">userIdentity</span><span class="sxs-lookup"><span data-stu-id="deb6b-122">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="deb6b-123">レビュー担当者の id。</span><span class="sxs-lookup"><span data-stu-id="deb6b-123">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="deb6b-124">このアクセス権に関する最新のレビューが提供された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="deb6b-124">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="deb6b-125">レビューの結果。</span><span class="sxs-lookup"><span data-stu-id="deb6b-125">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="deb6b-126">レビュー担当者の業務上の理由 (指定されている場合)。</span><span class="sxs-lookup"><span data-stu-id="deb6b-126">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="deb6b-127">userIdentity</span><span class="sxs-lookup"><span data-stu-id="deb6b-127">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="deb6b-128">レビューの完了時に、結果が手動で適用された場合、決定を適用したユーザーのユーザー id。</span><span class="sxs-lookup"><span data-stu-id="deb6b-128">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="deb6b-129">レビューの決定が適用された日時。</span><span class="sxs-lookup"><span data-stu-id="deb6b-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="deb6b-130">決定を適用した結果、、、 `NotApplied` `NotFound`また`Success`は`Failed` `NotSupported`のいずれか。</span><span class="sxs-lookup"><span data-stu-id="deb6b-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="deb6b-131">レビュー担当者、 `Approve` `Deny`またはまたは`NotAvailable`のいずれかに表示される、機能で生成された推奨事項。</span><span class="sxs-lookup"><span data-stu-id="deb6b-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="deb6b-132">さらに、決定されたアクセスを所有しているオブジェクトのオブジェクトの種類に応じて、追加のプロパティが存在する場合があります。</span><span class="sxs-lookup"><span data-stu-id="deb6b-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="deb6b-133">たとえば、アクセスレビューの決定が特定のユーザーのグループメンバーシップまたはアプリケーションアクセスである場合、アクセスを削除する可能性があるユーザーが次のプロパティを使用して識別されます。</span><span class="sxs-lookup"><span data-stu-id="deb6b-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="deb6b-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="deb6b-134">Property</span></span>                        | <span data-ttu-id="deb6b-135">型</span><span class="sxs-lookup"><span data-stu-id="deb6b-135">Type</span></span>                         | <span data-ttu-id="deb6b-136">説明</span><span class="sxs-lookup"><span data-stu-id="deb6b-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="deb6b-137">アクセスがレビューされたユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="deb6b-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="deb6b-138">アクセスがレビューされたユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="deb6b-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="deb6b-139">アクセスがレビューされたユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="deb6b-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="deb6b-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="deb6b-140">Relationships</span></span>

<span data-ttu-id="deb6b-141">なし。</span><span class="sxs-lookup"><span data-stu-id="deb6b-141">None.</span></span>  <span data-ttu-id="deb6b-142">この型のオブジェクトは、 [accessreview](accessreview.md)オブジェクトの[決定事項](../api/accessreview-listdecisions.md)と[mydecisions](../api/accessreview-listmydecisions.md)関係を使用して、アクセスレビューから取得できます。</span><span class="sxs-lookup"><span data-stu-id="deb6b-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="deb6b-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="deb6b-143">See also</span></span>

| <span data-ttu-id="deb6b-144">メソッド</span><span class="sxs-lookup"><span data-stu-id="deb6b-144">Method</span></span>           | <span data-ttu-id="deb6b-145">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="deb6b-145">Return Type</span></span>    |<span data-ttu-id="deb6b-146">説明</span><span class="sxs-lookup"><span data-stu-id="deb6b-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="deb6b-147">AccessReview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="deb6b-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="deb6b-148">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="deb6b-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="deb6b-149">AccessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="deb6b-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="deb6b-150">自分の accessReview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="deb6b-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="deb6b-151">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="deb6b-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="deb6b-152">レビュー担当者として、accessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="deb6b-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="deb6b-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="deb6b-153">JSON representation</span></span>

<span data-ttu-id="deb6b-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="deb6b-154">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
