---
title: accessReview リソースの種類
description: 'Azure AD access レビュー機能では、は`accessReview`アクセスレビューを表します。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b1801a7f7cbd52375e4fbbfb42847b29539a2dde
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657736"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="a4e46-103">accessReview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4e46-103">accessReview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4e46-104">Azure AD [access レビュー](accessreviews-root.md)機能では、は`accessReview`アクセスレビューを表します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="a4e46-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4e46-105">Methods</span></span>

| <span data-ttu-id="a4e46-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4e46-106">Method</span></span>           | <span data-ttu-id="a4e46-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a4e46-107">Return Type</span></span>    |<span data-ttu-id="a4e46-108">説明</span><span class="sxs-lookup"><span data-stu-id="a4e46-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4e46-109">AccessReview を取得する</span><span class="sxs-lookup"><span data-stu-id="a4e46-109">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="a4e46-110">accessReview</span><span class="sxs-lookup"><span data-stu-id="a4e46-110">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="a4e46-111">特定の id を持つアクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-111">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="a4e46-112">AccessReview を作成する</span><span class="sxs-lookup"><span data-stu-id="a4e46-112">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="a4e46-113">accessReview</span><span class="sxs-lookup"><span data-stu-id="a4e46-113">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="a4e46-114">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-114">Create a new accessReview.</span></span> |
|[<span data-ttu-id="a4e46-115">AccessReview の削除</span><span class="sxs-lookup"><span data-stu-id="a4e46-115">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="a4e46-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a4e46-116">None.</span></span>   | <span data-ttu-id="a4e46-117">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-117">Delete an accessReview.</span></span> |
|[<span data-ttu-id="a4e46-118">AccessReview を更新する</span><span class="sxs-lookup"><span data-stu-id="a4e46-118">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="a4e46-119">accessReview</span><span class="sxs-lookup"><span data-stu-id="a4e46-119">accessReview</span></span>](accessreview.md) | <span data-ttu-id="a4e46-120">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-120">Update an accessReview.</span></span> |
|[<span data-ttu-id="a4e46-121">AccessReview レビュー担当者のリスト</span><span class="sxs-lookup"><span data-stu-id="a4e46-121">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="a4e46-122">[Useridentity](useridentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4e46-122">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="a4e46-123">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-123">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="a4e46-124">AccessReview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="a4e46-124">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="a4e46-125">なし。</span><span class="sxs-lookup"><span data-stu-id="a4e46-125">None.</span></span>   |   <span data-ttu-id="a4e46-126">閲覧者を accessReview に追加します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-126">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="a4e46-127">AccessReview レビュー担当者を削除する</span><span class="sxs-lookup"><span data-stu-id="a4e46-127">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="a4e46-128">なし。</span><span class="sxs-lookup"><span data-stu-id="a4e46-128">None.</span></span>  |   <span data-ttu-id="a4e46-129">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-129">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="a4e46-130">AccessReview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a4e46-130">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="a4e46-131">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4e46-131">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="a4e46-132">AccessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-132">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="a4e46-133">自分の accessReview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a4e46-133">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="a4e46-134">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4e46-134">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="a4e46-135">レビュー担当者として、accessReview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-135">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="a4e46-136">Access レビュー通知の送信</span><span class="sxs-lookup"><span data-stu-id="a4e46-136">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="a4e46-137">なし。</span><span class="sxs-lookup"><span data-stu-id="a4e46-137">None.</span></span>   |   <span data-ttu-id="a4e46-138">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-138">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="a4e46-139">AccessReview を停止する</span><span class="sxs-lookup"><span data-stu-id="a4e46-139">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="a4e46-140">なし。</span><span class="sxs-lookup"><span data-stu-id="a4e46-140">None.</span></span>   |   <span data-ttu-id="a4e46-141">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-141">Stop an accessReview.</span></span> |
|[<span data-ttu-id="a4e46-142">AccessReview の決定をリセットする</span><span class="sxs-lookup"><span data-stu-id="a4e46-142">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="a4e46-143">なし。</span><span class="sxs-lookup"><span data-stu-id="a4e46-143">None.</span></span>   |   <span data-ttu-id="a4e46-144">進行中の accessReview で意思決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="a4e46-144">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="a4e46-145">AccessReview の決定を適用する</span><span class="sxs-lookup"><span data-stu-id="a4e46-145">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="a4e46-146">なし。</span><span class="sxs-lookup"><span data-stu-id="a4e46-146">None.</span></span>   |   <span data-ttu-id="a4e46-147">完了した accessReview から決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-147">Apply the decisions from a completed accessReview.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4e46-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4e46-148">Properties</span></span>
| <span data-ttu-id="a4e46-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4e46-149">Property</span></span>     | <span data-ttu-id="a4e46-150">型</span><span class="sxs-lookup"><span data-stu-id="a4e46-150">Type</span></span>   |<span data-ttu-id="a4e46-151">説明</span><span class="sxs-lookup"><span data-stu-id="a4e46-151">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="a4e46-152">アクセスレビューのフィーチャーによって割り当てられた一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a4e46-152">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="a4e46-153">アクセスレビュー名。</span><span class="sxs-lookup"><span data-stu-id="a4e46-153">The access review name.</span></span> <span data-ttu-id="a4e46-154">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="a4e46-154">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="a4e46-155">レビューが開始される予定の日時。</span><span class="sxs-lookup"><span data-stu-id="a4e46-155">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="a4e46-156">これは、将来の日付になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-156">This could be a date in the future.</span></span>  <span data-ttu-id="a4e46-157">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="a4e46-157">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="a4e46-158">レビューが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="a4e46-158">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="a4e46-159">これは、開始日よりも1日以上後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="a4e46-159">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="a4e46-160">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="a4e46-160">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="a4e46-161">この読み取り専用フィールドは、accessReview の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-161">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="a4e46-162">一般的な状態に`Initializing`は`NotStarted`、 `Starting``InProgress` `Completing` `Completed` `AutoReviewing`、、、、、、 `AutoReviewed`、などがあります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-162">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="a4e46-163">レビュー担当者に表示する、アクセスレビュー作成者によって提供される説明。</span><span class="sxs-lookup"><span data-stu-id="a4e46-163">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="a4e46-164">ビジネスフローテンプレートの識別子。</span><span class="sxs-lookup"><span data-stu-id="a4e46-164">The business flow template identifier.</span></span> <span data-ttu-id="a4e46-165">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="a4e46-165">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="a4e46-166">レビュー担当者の関係の種類 (ターゲットオブジェクト、また`self`は`delegated` `entityOwners`のいずれか)。</span><span class="sxs-lookup"><span data-stu-id="a4e46-166">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="a4e46-167">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="a4e46-167">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="a4e46-168">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a4e46-168">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="a4e46-169">このレビューを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="a4e46-169">The user who created this review.</span></span> |
| `reviewedEntity`          |[<span data-ttu-id="a4e46-170">identity</span><span class="sxs-lookup"><span data-stu-id="a4e46-170">identity</span></span>](identity.md)                                      | <span data-ttu-id="a4e46-171">アクセスレビューでアクセス権の割り当てを確認しているオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="a4e46-171">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="a4e46-172">これは、グループ内のユーザーのメンバーシップを確認したり、アプリケーションへのユーザーの割り当てを確認したりするためのグループであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="a4e46-172">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="a4e46-173">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="a4e46-173">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="a4e46-174">AccessReview の設定については、以下の「型の定義」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4e46-174">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="a4e46-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4e46-175">Relationships</span></span>




| <span data-ttu-id="a4e46-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4e46-176">Relationship</span></span> | <span data-ttu-id="a4e46-177">型</span><span class="sxs-lookup"><span data-stu-id="a4e46-177">Type</span></span>   |<span data-ttu-id="a4e46-178">説明</span><span class="sxs-lookup"><span data-stu-id="a4e46-178">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="a4e46-179">[Useridentity](useridentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4e46-179">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="a4e46-180">アクセスレビュー reviewerType の種類`delegate`がの場合に、アクセスレビューのレビュー担当者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a4e46-180">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="a4e46-181">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4e46-181">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="a4e46-182">このアクセスレビューに関する決定事項のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a4e46-182">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="a4e46-183">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4e46-183">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="a4e46-184">呼び出し元がレビュー担当者の場合、呼び出し元に対する決定のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a4e46-184">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="a4e46-185">[Accessreview](accessreview.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4e46-185">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="a4e46-186">このオブジェクトが定期的なアクセスレビューである場合、access のコレクションは、過去、現在、および今後のインスタンスをレビューします。</span><span class="sxs-lookup"><span data-stu-id="a4e46-186">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="a4e46-187">オブジェクトにこれらのリレーションシップが存在するかどうかは、オブジェクトが1回限りのアクセスレビューであるか、定期的なアクセスレビューの一連であるか、または定期的なアクセスレビューのインスタンスであるかに応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-187">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="a4e46-188">シナリオ</span><span class="sxs-lookup"><span data-stu-id="a4e46-188">Scenario</span></span> | <span data-ttu-id="a4e46-189">レビュー担当者がいますか?</span><span class="sxs-lookup"><span data-stu-id="a4e46-189">Has reviewers?</span></span> | <span data-ttu-id="a4e46-190">決定事項と myDecisions はありますか?</span><span class="sxs-lookup"><span data-stu-id="a4e46-190">Has decisions and myDecisions?</span></span> | <span data-ttu-id="a4e46-191">インスタンスがあるかどうか</span><span class="sxs-lookup"><span data-stu-id="a4e46-191">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="a4e46-192">ワンタイムアクセスのレビュー</span><span class="sxs-lookup"><span data-stu-id="a4e46-192">One-time access review</span></span>|<span data-ttu-id="a4e46-193">はい</span><span class="sxs-lookup"><span data-stu-id="a4e46-193">Yes</span></span> | <span data-ttu-id="a4e46-194">はい (開始した後)</span><span class="sxs-lookup"><span data-stu-id="a4e46-194">Yes, once started</span></span> | <span data-ttu-id="a4e46-195">いいえ</span><span class="sxs-lookup"><span data-stu-id="a4e46-195">No</span></span> |
| <span data-ttu-id="a4e46-196">定期的なアクセスのレビュー</span><span class="sxs-lookup"><span data-stu-id="a4e46-196">Recurring access review</span></span> | <span data-ttu-id="a4e46-197">はい</span><span class="sxs-lookup"><span data-stu-id="a4e46-197">Yes</span></span> | <span data-ttu-id="a4e46-198">いいえ</span><span class="sxs-lookup"><span data-stu-id="a4e46-198">No</span></span> | <span data-ttu-id="a4e46-199">はい</span><span class="sxs-lookup"><span data-stu-id="a4e46-199">Yes</span></span> |
| <span data-ttu-id="a4e46-200">定期的なアクセスレビューのインスタンス</span><span class="sxs-lookup"><span data-stu-id="a4e46-200">Instance of a recurring access review</span></span> | <span data-ttu-id="a4e46-201">はい</span><span class="sxs-lookup"><span data-stu-id="a4e46-201">Yes</span></span> | <span data-ttu-id="a4e46-202">はい (開始した後)</span><span class="sxs-lookup"><span data-stu-id="a4e46-202">Yes, once started</span></span> | <span data-ttu-id="a4e46-203">いいえ</span><span class="sxs-lookup"><span data-stu-id="a4e46-203">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4e46-204">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4e46-204">JSON representation</span></span>

<span data-ttu-id="a4e46-205">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4e46-205">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReview"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "description": "string",
 "businessFlowTemplateId": "string (identifier)",
 "reviewerType": "string",
 "createdBy": "microsoft.graph.userIdentity",
 "reviewedEntity": "microsoft.graph.identity",
 "settings": "microsoft.graph.accessReviewSettings",
 "reviewers": "Collection(microsoft.graph.userIdentity)"
}

```

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="a4e46-206">AccessReviewSettings の種類</span><span class="sxs-lookup"><span data-stu-id="a4e46-206">The accessReviewSettings type</span></span>

<span data-ttu-id="a4e46-207">は`accessReviewSettings` 、アクセスレビューを作成するときの追加の設定を提供し、アクセスレビューを開始するときの機能の動作を制御します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-207">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="a4e46-208">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-208">This type has the following properties:</span></span> 

| <span data-ttu-id="a4e46-209">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4e46-209">Property</span></span>                     | <span data-ttu-id="a4e46-210">型</span><span class="sxs-lookup"><span data-stu-id="a4e46-210">Type</span></span>                      | <span data-ttu-id="a4e46-211">説明</span><span class="sxs-lookup"><span data-stu-id="a4e46-211">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="a4e46-212">レビュー担当者にメールを送信するかどうか、およびレビュー作成者を有効にするかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="a4e46-212">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="a4e46-213">レビュー担当者に電子メールを送信することが有効かどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="a4e46-213">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="a4e46-214">レビュー担当者がアクセスをレビューする際に理由を指定する必要があるかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="a4e46-214">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="a4e46-215">ユーザーアクティビティがレビューアーに表示される日数。</span><span class="sxs-lookup"><span data-stu-id="a4e46-215">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="a4e46-216">レビュー担当者が自動適用で使用するように指定されていない場合に、機能が決定を設定するかどうかを指定するフラグが有効になります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-216">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="a4e46-217">次に示すように、機能によってレビューの決定を設定する方法の詳細設定 (自動適用で使用)。</span><span class="sxs-lookup"><span data-stu-id="a4e46-217">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="a4e46-218">定期的なパターンの詳細設定。以下に説明します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-218">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="a4e46-219">自動適用機能を使用して、ターゲットオブジェクトのアクセスリソースを自動的に変更するかどうかを示すフラグが有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-219">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="a4e46-220">有効になっていない場合、ユーザーはレビューが完了した後、アクセスレビューを適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-220">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="a4e46-221">レビュー担当者におすすめ候補を表示するかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="a4e46-221">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="a4e46-222">AutoReviewSettings の種類</span><span class="sxs-lookup"><span data-stu-id="a4e46-222">The autoReviewSettings type</span></span>

<span data-ttu-id="a4e46-223">は`autoReviewSettings` 、アクセスレビューの設定内に埋め込まれ、アクセスレビューが完了したときの機能の動作を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-223">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="a4e46-224">この型には、 `notReviewedResult`1 つのプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-224">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="a4e46-225">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4e46-225">Property</span></span>                     | <span data-ttu-id="a4e46-226">型</span><span class="sxs-lookup"><span data-stu-id="a4e46-226">Type</span></span>     | <span data-ttu-id="a4e46-227">説明</span><span class="sxs-lookup"><span data-stu-id="a4e46-227">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="a4e46-228">`Approve`、`Deny`、`Recommendation` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="a4e46-228">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="a4e46-229">AccessReviewRecurrenceSettings の種類</span><span class="sxs-lookup"><span data-stu-id="a4e46-229">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="a4e46-230">は`accessReviewRecurrenceSettings` 、アクセスレビューの設定内に埋め込まれており、定期的にアクセスレビューが繰り返されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-230">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="a4e46-231">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-231">This type has the following properties:</span></span>

| <span data-ttu-id="a4e46-232">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4e46-232">Property</span></span>                     | <span data-ttu-id="a4e46-233">型</span><span class="sxs-lookup"><span data-stu-id="a4e46-233">Type</span></span>                                                                                                          | <span data-ttu-id="a4e46-234">説明</span><span class="sxs-lookup"><span data-stu-id="a4e46-234">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="a4e46-235">繰り返し間隔。、、、、または`onetime` `annual`の`weekly` `monthly` `quarterly`いずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4e46-235">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="a4e46-236">定期的なアイテムの終了方法。</span><span class="sxs-lookup"><span data-stu-id="a4e46-236">How the recurrence ends.</span></span> <span data-ttu-id="a4e46-237">その場合は`Never`、定期的なアイテムの明示的な終了はありません。</span><span class="sxs-lookup"><span data-stu-id="a4e46-237">If it is `Never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="a4e46-238">その場合、 `endBy`定期的なパターンは特定の日付に終了します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-238">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="a4e46-239">含まれて`occurrences`いる場合は、レビューの`recurrentCount`インスタンスが完了した後に series が終了します。</span><span class="sxs-lookup"><span data-stu-id="a4e46-239">If it is `occurrences`, then the series ends after `recurrentCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="a4e46-240">定期的なアイテムの期間 (日単位)。</span><span class="sxs-lookup"><span data-stu-id="a4e46-240">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="a4e46-241">繰り返しの数 (の`recurrenceEndType`値が`occurrences`である場合)、そうでない場合は0。</span><span class="sxs-lookup"><span data-stu-id="a4e46-241">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |


<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
