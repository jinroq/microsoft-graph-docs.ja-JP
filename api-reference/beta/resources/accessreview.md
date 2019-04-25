---
title: accessreview リソースの種類
description: 'Azure AD access レビュー機能では、は`accessReview`アクセスレビューを表します。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2cb5d32a8dcc6b12330aca6e831a8ab2083759df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544112"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="304ef-103">accessreview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="304ef-103">accessReview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="304ef-104">Azure AD [access レビュー](accessreviews-root.md)機能では、は`accessReview`アクセスレビューを表します。</span><span class="sxs-lookup"><span data-stu-id="304ef-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="304ef-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="304ef-105">Methods</span></span>

| <span data-ttu-id="304ef-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="304ef-106">Method</span></span>           | <span data-ttu-id="304ef-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="304ef-107">Return Type</span></span>    |<span data-ttu-id="304ef-108">説明</span><span class="sxs-lookup"><span data-stu-id="304ef-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="304ef-109">accessreview を取得する</span><span class="sxs-lookup"><span data-stu-id="304ef-109">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="304ef-110">accessreview</span><span class="sxs-lookup"><span data-stu-id="304ef-110">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="304ef-111">特定の id を持つアクセスレビューを取得します。</span><span class="sxs-lookup"><span data-stu-id="304ef-111">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="304ef-112">accessreview を作成する</span><span class="sxs-lookup"><span data-stu-id="304ef-112">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="304ef-113">accessreview</span><span class="sxs-lookup"><span data-stu-id="304ef-113">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="304ef-114">新しい accessreview を作成します。</span><span class="sxs-lookup"><span data-stu-id="304ef-114">Create a new accessReview.</span></span> |
|[<span data-ttu-id="304ef-115">accessreview の削除</span><span class="sxs-lookup"><span data-stu-id="304ef-115">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="304ef-116">なし。</span><span class="sxs-lookup"><span data-stu-id="304ef-116">None.</span></span>   | <span data-ttu-id="304ef-117">accessreview を削除します。</span><span class="sxs-lookup"><span data-stu-id="304ef-117">Delete an accessReview.</span></span> |
|[<span data-ttu-id="304ef-118">accessreview を更新する</span><span class="sxs-lookup"><span data-stu-id="304ef-118">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="304ef-119">accessreview</span><span class="sxs-lookup"><span data-stu-id="304ef-119">accessReview</span></span>](accessreview.md) | <span data-ttu-id="304ef-120">accessreview を更新します。</span><span class="sxs-lookup"><span data-stu-id="304ef-120">Update an accessReview.</span></span> |
|[<span data-ttu-id="304ef-121">accessreview レビュー担当者のリスト</span><span class="sxs-lookup"><span data-stu-id="304ef-121">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="304ef-122">[useridentity](useridentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="304ef-122">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="304ef-123">accessreview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="304ef-123">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="304ef-124">accessreview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="304ef-124">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="304ef-125">なし。</span><span class="sxs-lookup"><span data-stu-id="304ef-125">None.</span></span>   |   <span data-ttu-id="304ef-126">閲覧者を accessreview に追加します。</span><span class="sxs-lookup"><span data-stu-id="304ef-126">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="304ef-127">accessreview レビュー担当者を削除する</span><span class="sxs-lookup"><span data-stu-id="304ef-127">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="304ef-128">なし。</span><span class="sxs-lookup"><span data-stu-id="304ef-128">None.</span></span>  |   <span data-ttu-id="304ef-129">accessreview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="304ef-129">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="304ef-130">accessreview に関する決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="304ef-130">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="304ef-131">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="304ef-131">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="304ef-132">accessreview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="304ef-132">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="304ef-133">自分の accessreview の決定事項を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="304ef-133">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="304ef-134">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="304ef-134">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="304ef-135">レビュー担当者として、accessreview の決定事項を取得します。</span><span class="sxs-lookup"><span data-stu-id="304ef-135">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="304ef-136">access レビュー通知の送信</span><span class="sxs-lookup"><span data-stu-id="304ef-136">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="304ef-137">なし。</span><span class="sxs-lookup"><span data-stu-id="304ef-137">None.</span></span>   |   <span data-ttu-id="304ef-138">accessreview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="304ef-138">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="304ef-139">accessreview を停止する</span><span class="sxs-lookup"><span data-stu-id="304ef-139">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="304ef-140">なし。</span><span class="sxs-lookup"><span data-stu-id="304ef-140">None.</span></span>   |   <span data-ttu-id="304ef-141">accessreview を停止します。</span><span class="sxs-lookup"><span data-stu-id="304ef-141">Stop an accessReview.</span></span> |
|[<span data-ttu-id="304ef-142">accessreview の決定をリセットする</span><span class="sxs-lookup"><span data-stu-id="304ef-142">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="304ef-143">なし。</span><span class="sxs-lookup"><span data-stu-id="304ef-143">None.</span></span>   |   <span data-ttu-id="304ef-144">進行中の accessreview で意思決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="304ef-144">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="304ef-145">accessreview の決定を適用する</span><span class="sxs-lookup"><span data-stu-id="304ef-145">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="304ef-146">なし。</span><span class="sxs-lookup"><span data-stu-id="304ef-146">None.</span></span>   |   <span data-ttu-id="304ef-147">完了した accessreview から決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="304ef-147">Apply the decisions from a completed accessReview.</span></span>|

## <a name="permissions"></a><span data-ttu-id="304ef-148">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="304ef-148">Permissions</span></span>

|<span data-ttu-id="304ef-149">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="304ef-149">Permission type</span></span>                        | <span data-ttu-id="304ef-150">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="304ef-150">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="304ef-151">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="304ef-151">Delegated (work or school account)</span></span>     | <span data-ttu-id="304ef-152">accessreview を参照してください。</span><span class="sxs-lookup"><span data-stu-id="304ef-152">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="304ef-153">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="304ef-153">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="304ef-154">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="304ef-154">Not supported.</span></span> |
|<span data-ttu-id="304ef-155">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="304ef-155">Application</span></span>                            | <span data-ttu-id="304ef-156">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="304ef-156">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="304ef-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="304ef-157">Properties</span></span>
| <span data-ttu-id="304ef-158">プロパティ</span><span class="sxs-lookup"><span data-stu-id="304ef-158">Property</span></span>     | <span data-ttu-id="304ef-159">型</span><span class="sxs-lookup"><span data-stu-id="304ef-159">Type</span></span>   |<span data-ttu-id="304ef-160">説明</span><span class="sxs-lookup"><span data-stu-id="304ef-160">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="304ef-161">アクセスレビューのフィーチャーによって割り当てられた一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="304ef-161">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="304ef-162">アクセスレビュー名。</span><span class="sxs-lookup"><span data-stu-id="304ef-162">The access review name.</span></span> <span data-ttu-id="304ef-163">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="304ef-163">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="304ef-164">レビューが開始される予定の日時。</span><span class="sxs-lookup"><span data-stu-id="304ef-164">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="304ef-165">これは、将来の日付になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="304ef-165">This could be a date in the future.</span></span>  <span data-ttu-id="304ef-166">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="304ef-166">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="304ef-167">レビューが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="304ef-167">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="304ef-168">これは、開始日よりも1日以上後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="304ef-168">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="304ef-169">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="304ef-169">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="304ef-170">この読み取り専用フィールドは、accessreview の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="304ef-170">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="304ef-171">一般的な状態に`Initializing`は`NotStarted`、 `Starting``InProgress` `Completing` `Completed` `AutoReviewing`、、、、、、 `AutoReviewed`、などがあります。</span><span class="sxs-lookup"><span data-stu-id="304ef-171">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="304ef-172">レビュー担当者に表示する、アクセスレビュー作成者によって提供される説明。</span><span class="sxs-lookup"><span data-stu-id="304ef-172">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="304ef-173">ビジネスフローテンプレートの識別子。</span><span class="sxs-lookup"><span data-stu-id="304ef-173">The business flow template identifier.</span></span> <span data-ttu-id="304ef-174">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="304ef-174">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="304ef-175">レビュー担当者の関係の種類 (ターゲットオブジェクト、また`self`は`delegated` `entityOwners`のいずれか)。</span><span class="sxs-lookup"><span data-stu-id="304ef-175">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="304ef-176">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="304ef-176">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="304ef-177">userIdentity</span><span class="sxs-lookup"><span data-stu-id="304ef-177">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="304ef-178">このレビューを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="304ef-178">The user who created this review.</span></span> |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="304ef-179">アクセスレビューでアクセス権の割り当てを確認しているオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="304ef-179">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="304ef-180">これは、グループ内のユーザーのメンバーシップを確認したり、アプリケーションへのユーザーの割り当てを確認したりするためのグループであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="304ef-180">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="304ef-181">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="304ef-181">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="304ef-182">accessreview の設定については、以下の「型の定義」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="304ef-182">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="304ef-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="304ef-183">Relationships</span></span>




| <span data-ttu-id="304ef-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="304ef-184">Relationship</span></span> | <span data-ttu-id="304ef-185">型</span><span class="sxs-lookup"><span data-stu-id="304ef-185">Type</span></span>   |<span data-ttu-id="304ef-186">説明</span><span class="sxs-lookup"><span data-stu-id="304ef-186">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="304ef-187">[useridentity](useridentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="304ef-187">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="304ef-188">アクセスレビュー reviewerType の種類`delegate`がの場合に、アクセスレビューのレビュー担当者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="304ef-188">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="304ef-189">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="304ef-189">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="304ef-190">このアクセスレビューに関する決定事項のコレクション。</span><span class="sxs-lookup"><span data-stu-id="304ef-190">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="304ef-191">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="304ef-191">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="304ef-192">呼び出し元がレビュー担当者の場合、呼び出し元に対する決定のコレクション。</span><span class="sxs-lookup"><span data-stu-id="304ef-192">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="304ef-193">[accessreview](accessreview.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="304ef-193">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="304ef-194">このオブジェクトが定期的なアクセスレビューである場合、access のコレクションは、過去、現在、および今後のインスタンスをレビューします。</span><span class="sxs-lookup"><span data-stu-id="304ef-194">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="304ef-195">オブジェクトにこれらのリレーションシップが存在するかどうかは、オブジェクトが1回限りのアクセスレビューであるか、定期的なアクセスレビューの一連であるか、または定期的なアクセスレビューのインスタンスであるかに応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="304ef-195">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="304ef-196">シナリオ</span><span class="sxs-lookup"><span data-stu-id="304ef-196">Scenario</span></span> | <span data-ttu-id="304ef-197">レビュー担当者がいますか?</span><span class="sxs-lookup"><span data-stu-id="304ef-197">Has reviewers?</span></span> | <span data-ttu-id="304ef-198">決定事項と mydecisions はありますか?</span><span class="sxs-lookup"><span data-stu-id="304ef-198">Has decisions and myDecisions?</span></span> | <span data-ttu-id="304ef-199">インスタンスがあるかどうか</span><span class="sxs-lookup"><span data-stu-id="304ef-199">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="304ef-200">ワンタイムアクセスのレビュー</span><span class="sxs-lookup"><span data-stu-id="304ef-200">One-time access review</span></span>|<span data-ttu-id="304ef-201">はい</span><span class="sxs-lookup"><span data-stu-id="304ef-201">Yes</span></span> | <span data-ttu-id="304ef-202">はい (開始した後)</span><span class="sxs-lookup"><span data-stu-id="304ef-202">Yes, once started</span></span> | <span data-ttu-id="304ef-203">いいえ</span><span class="sxs-lookup"><span data-stu-id="304ef-203">No</span></span> |
| <span data-ttu-id="304ef-204">定期的なアクセスのレビュー</span><span class="sxs-lookup"><span data-stu-id="304ef-204">Recurring access review</span></span> | <span data-ttu-id="304ef-205">はい</span><span class="sxs-lookup"><span data-stu-id="304ef-205">Yes</span></span> | <span data-ttu-id="304ef-206">いいえ</span><span class="sxs-lookup"><span data-stu-id="304ef-206">No</span></span> | <span data-ttu-id="304ef-207">はい</span><span class="sxs-lookup"><span data-stu-id="304ef-207">Yes</span></span> |
| <span data-ttu-id="304ef-208">定期的なアクセスレビューのインスタンス</span><span class="sxs-lookup"><span data-stu-id="304ef-208">Instance of a recurring access review</span></span> | <span data-ttu-id="304ef-209">はい</span><span class="sxs-lookup"><span data-stu-id="304ef-209">Yes</span></span> | <span data-ttu-id="304ef-210">はい (開始した後)</span><span class="sxs-lookup"><span data-stu-id="304ef-210">Yes, once started</span></span> | <span data-ttu-id="304ef-211">いいえ</span><span class="sxs-lookup"><span data-stu-id="304ef-211">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="304ef-212">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="304ef-212">JSON representation</span></span>

<span data-ttu-id="304ef-213">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="304ef-213">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="304ef-214">accessReviewSettings の種類</span><span class="sxs-lookup"><span data-stu-id="304ef-214">The accessReviewSettings type</span></span>

<span data-ttu-id="304ef-215">は`accessReviewSettings` 、アクセスレビューを作成するときの追加の設定を提供し、アクセスレビューを開始するときの機能の動作を制御します。</span><span class="sxs-lookup"><span data-stu-id="304ef-215">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="304ef-216">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="304ef-216">This type has the following properties:</span></span> 

| <span data-ttu-id="304ef-217">プロパティ</span><span class="sxs-lookup"><span data-stu-id="304ef-217">Property</span></span>                     | <span data-ttu-id="304ef-218">型</span><span class="sxs-lookup"><span data-stu-id="304ef-218">Type</span></span>                      | <span data-ttu-id="304ef-219">説明</span><span class="sxs-lookup"><span data-stu-id="304ef-219">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="304ef-220">レビュー担当者にメールを送信するかどうか、およびレビュー作成者を有効にするかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="304ef-220">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="304ef-221">レビュー担当者に電子メールを送信することが有効かどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="304ef-221">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="304ef-222">レビュー担当者がアクセスをレビューする際に理由を指定する必要があるかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="304ef-222">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="304ef-223">ユーザーアクティビティがレビューアーに表示される日数。</span><span class="sxs-lookup"><span data-stu-id="304ef-223">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="304ef-224">レビュー担当者が自動適用で使用するように指定されていない場合に、機能が決定を設定するかどうかを指定するフラグが有効になります。</span><span class="sxs-lookup"><span data-stu-id="304ef-224">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="304ef-225">次に示すように、機能によってレビューの決定を設定する方法の詳細設定 (自動適用で使用)。</span><span class="sxs-lookup"><span data-stu-id="304ef-225">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="304ef-226">定期的なパターンの詳細設定。以下に説明します。</span><span class="sxs-lookup"><span data-stu-id="304ef-226">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="304ef-227">自動適用機能を使用して、ターゲットオブジェクトのアクセスリソースを自動的に変更するかどうかを示すフラグが有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="304ef-227">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="304ef-228">有効になっていない場合、ユーザーはレビューが完了した後、アクセスレビューを適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="304ef-228">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="304ef-229">レビュー担当者におすすめ候補を表示するかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="304ef-229">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |



## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="304ef-230">autoreviewsettings の種類</span><span class="sxs-lookup"><span data-stu-id="304ef-230">The autoReviewSettings type</span></span>

<span data-ttu-id="304ef-231">は`autoReviewSettings` 、アクセスレビューの設定内に埋め込まれ、アクセスレビューが完了したときの機能の動作を指定します。</span><span class="sxs-lookup"><span data-stu-id="304ef-231">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="304ef-232">この型には、 `notReviewedResult`1 つのプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="304ef-232">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="304ef-233">プロパティ</span><span class="sxs-lookup"><span data-stu-id="304ef-233">Property</span></span>                     | <span data-ttu-id="304ef-234">型</span><span class="sxs-lookup"><span data-stu-id="304ef-234">Type</span></span>     | <span data-ttu-id="304ef-235">説明</span><span class="sxs-lookup"><span data-stu-id="304ef-235">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="304ef-236">`Approve`、`Deny`、`Recommendation` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="304ef-236">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="304ef-237">accessReviewRecurrenceSettings の種類</span><span class="sxs-lookup"><span data-stu-id="304ef-237">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="304ef-238">は`accessReviewRecurrenceSettings` 、アクセスレビューの設定内に埋め込まれており、定期的にアクセスレビューが繰り返されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="304ef-238">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="304ef-239">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="304ef-239">This type has the following properties:</span></span>

| <span data-ttu-id="304ef-240">プロパティ</span><span class="sxs-lookup"><span data-stu-id="304ef-240">Property</span></span>                     | <span data-ttu-id="304ef-241">型</span><span class="sxs-lookup"><span data-stu-id="304ef-241">Type</span></span>                                                                                                          | <span data-ttu-id="304ef-242">説明</span><span class="sxs-lookup"><span data-stu-id="304ef-242">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="304ef-243">繰り返し間隔。、、、、または`onetime` `annual`の`weekly` `monthly` `quarterly`いずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="304ef-243">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="304ef-244">定期的なアイテムの終了方法。</span><span class="sxs-lookup"><span data-stu-id="304ef-244">How the recurrence ends.</span></span> <span data-ttu-id="304ef-245">その場合は`Never`、定期的なアイテムの明示的な終了はありません。</span><span class="sxs-lookup"><span data-stu-id="304ef-245">If it is `Never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="304ef-246">その場合、 `endBy`定期的なパターンは特定の日付に終了します。</span><span class="sxs-lookup"><span data-stu-id="304ef-246">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="304ef-247">含まれて`occurrences`いる場合は、レビューの`recurrentCount`インスタンスが完了した後に series が終了します。</span><span class="sxs-lookup"><span data-stu-id="304ef-247">If it is `occurrences`, then the series ends after `recurrentCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="304ef-248">定期的なアイテムの期間 (日単位)。</span><span class="sxs-lookup"><span data-stu-id="304ef-248">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="304ef-249">繰り返しの数 (の`recurrenceEndType`値が`occurrences`である場合)、そうでない場合は0。</span><span class="sxs-lookup"><span data-stu-id="304ef-249">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |



<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
