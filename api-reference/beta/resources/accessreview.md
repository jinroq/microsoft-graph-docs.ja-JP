---
title: accessReview リソースの種類
description: 'Azure AD にアクセス確認機能を`accessReview`、アクセス確認を表します。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2cb5d32a8dcc6b12330aca6e831a8ab2083759df
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642493"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="413ea-103">accessReview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="413ea-103">accessReview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="413ea-104">Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `accessReview` 、アクセス確認を表します。</span><span class="sxs-lookup"><span data-stu-id="413ea-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="413ea-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="413ea-105">Methods</span></span>

| <span data-ttu-id="413ea-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="413ea-106">Method</span></span>           | <span data-ttu-id="413ea-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="413ea-107">Return Type</span></span>    |<span data-ttu-id="413ea-108">説明</span><span class="sxs-lookup"><span data-stu-id="413ea-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="413ea-109">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="413ea-109">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="413ea-110">accessReview</span><span class="sxs-lookup"><span data-stu-id="413ea-110">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="413ea-111">特定の id を持つ、アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="413ea-111">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="413ea-112">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="413ea-112">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="413ea-113">accessReview</span><span class="sxs-lookup"><span data-stu-id="413ea-113">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="413ea-114">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="413ea-114">Create a new accessReview.</span></span> |
|[<span data-ttu-id="413ea-115">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="413ea-115">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="413ea-116">なし。</span><span class="sxs-lookup"><span data-stu-id="413ea-116">None.</span></span>   | <span data-ttu-id="413ea-117">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="413ea-117">Delete an accessReview.</span></span> |
|[<span data-ttu-id="413ea-118">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="413ea-118">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="413ea-119">accessReview</span><span class="sxs-lookup"><span data-stu-id="413ea-119">accessReview</span></span>](accessreview.md) | <span data-ttu-id="413ea-120">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="413ea-120">Update an accessReview.</span></span> |
|[<span data-ttu-id="413ea-121">AccessReview の校閲者の一覧</span><span class="sxs-lookup"><span data-stu-id="413ea-121">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="413ea-122">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="413ea-122">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="413ea-123">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="413ea-123">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="413ea-124">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="413ea-124">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="413ea-125">なし。</span><span class="sxs-lookup"><span data-stu-id="413ea-125">None.</span></span>   |   <span data-ttu-id="413ea-126">AccessReview には、レビュー担当者を追加します。</span><span class="sxs-lookup"><span data-stu-id="413ea-126">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="413ea-127">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="413ea-127">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="413ea-128">なし。</span><span class="sxs-lookup"><span data-stu-id="413ea-128">None.</span></span>  |   <span data-ttu-id="413ea-129">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="413ea-129">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="413ea-130">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="413ea-130">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="413ea-131">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="413ea-131">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="413ea-132">AccessReview の決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="413ea-132">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="413ea-133">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="413ea-133">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="413ea-134">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="413ea-134">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="413ea-135">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="413ea-135">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="413ea-136">AccessReview アラームを送信します。</span><span class="sxs-lookup"><span data-stu-id="413ea-136">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="413ea-137">なし。</span><span class="sxs-lookup"><span data-stu-id="413ea-137">None.</span></span>   |   <span data-ttu-id="413ea-138">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="413ea-138">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="413ea-139">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="413ea-139">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="413ea-140">なし。</span><span class="sxs-lookup"><span data-stu-id="413ea-140">None.</span></span>   |   <span data-ttu-id="413ea-141">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="413ea-141">Stop an accessReview.</span></span> |
|[<span data-ttu-id="413ea-142">リセット accessReview 決定</span><span class="sxs-lookup"><span data-stu-id="413ea-142">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="413ea-143">なし。</span><span class="sxs-lookup"><span data-stu-id="413ea-143">None.</span></span>   |   <span data-ttu-id="413ea-144">進行中の accessReview の決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="413ea-144">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="413ea-145">AccessReview の決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="413ea-145">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="413ea-146">なし。</span><span class="sxs-lookup"><span data-stu-id="413ea-146">None.</span></span>   |   <span data-ttu-id="413ea-147">完了した accessReview からの決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="413ea-147">Apply the decisions from a completed accessReview.</span></span>|

## <a name="permissions"></a><span data-ttu-id="413ea-148">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="413ea-148">Permissions</span></span>

|<span data-ttu-id="413ea-149">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="413ea-149">Permission type</span></span>                        | <span data-ttu-id="413ea-150">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="413ea-150">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="413ea-151">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="413ea-151">Delegated (work or school account)</span></span>     | <span data-ttu-id="413ea-152">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="413ea-152">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="413ea-153">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="413ea-153">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="413ea-154">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="413ea-154">Not supported.</span></span> |
|<span data-ttu-id="413ea-155">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="413ea-155">Application</span></span>                            | <span data-ttu-id="413ea-156">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="413ea-156">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="413ea-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="413ea-157">Properties</span></span>
| <span data-ttu-id="413ea-158">プロパティ</span><span class="sxs-lookup"><span data-stu-id="413ea-158">Property</span></span>     | <span data-ttu-id="413ea-159">型</span><span class="sxs-lookup"><span data-stu-id="413ea-159">Type</span></span>   |<span data-ttu-id="413ea-160">説明</span><span class="sxs-lookup"><span data-stu-id="413ea-160">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="413ea-161">機能に割り当てられた一意の識別子アクセス レビューします。</span><span class="sxs-lookup"><span data-stu-id="413ea-161">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="413ea-162">アクセス確認の名前です。</span><span class="sxs-lookup"><span data-stu-id="413ea-162">The access review name.</span></span> <span data-ttu-id="413ea-163">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="413ea-163">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="413ea-164">日付と時刻と、レビューを開始する予定です。</span><span class="sxs-lookup"><span data-stu-id="413ea-164">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="413ea-165">将来の日付可能性があります。</span><span class="sxs-lookup"><span data-stu-id="413ea-165">This could be a date in the future.</span></span>  <span data-ttu-id="413ea-166">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="413ea-166">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="413ea-167">レビューの終了がスケジュールされているときの日時。</span><span class="sxs-lookup"><span data-stu-id="413ea-167">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="413ea-168">これは、少なくとも 1 つの日を開始日より後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="413ea-168">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="413ea-169">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="413ea-169">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="413ea-170">この読み取り専用フィールドは、accessReview のステータスを指定します。</span><span class="sxs-lookup"><span data-stu-id="413ea-170">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="413ea-171">標準的な状態には、 `Initializing`、 `NotStarted`、 `Starting`、`InProgress`、 `Completing`、 `Completed`、`AutoReviewing`と`AutoReviewed`。</span><span class="sxs-lookup"><span data-stu-id="413ea-171">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="413ea-172">アクセス レビュー作成者は、校閲者を表示して説明します。</span><span class="sxs-lookup"><span data-stu-id="413ea-172">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="413ea-173">業務フローのテンプレートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="413ea-173">The business flow template identifier.</span></span> <span data-ttu-id="413ea-174">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="413ea-174">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="413ea-175">関連付けの種類、対象のオブジェクトのいずれかの校閲者の`self`、`delegated`または`entityOwners`。</span><span class="sxs-lookup"><span data-stu-id="413ea-175">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="413ea-176">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="413ea-176">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="413ea-177">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="413ea-177">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="413ea-178">このレビューを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="413ea-178">The user who created this review.</span></span> |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="413ea-179">アクセス権を確認するオブジェクトがアクセス権限の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="413ea-179">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="413ea-180">グループでは、ユーザーのグループ メンバーシップの確認のため、またはアプリケーションへのユーザーの割り当ての詳細についてはアプリケーションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="413ea-180">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="413ea-181">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="413ea-181">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="413ea-182">AccessReview の設定は、以下の種類の定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="413ea-182">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="413ea-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="413ea-183">Relationships</span></span>




| <span data-ttu-id="413ea-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="413ea-184">Relationship</span></span> | <span data-ttu-id="413ea-185">型</span><span class="sxs-lookup"><span data-stu-id="413ea-185">Type</span></span>   |<span data-ttu-id="413ea-186">説明</span><span class="sxs-lookup"><span data-stu-id="413ea-186">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="413ea-187">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="413ea-187">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="413ea-188">アクセス レビュー reviewerType 型の場合、アクセス確認などの校閲者のコレクション`delegate`。</span><span class="sxs-lookup"><span data-stu-id="413ea-188">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="413ea-189">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="413ea-189">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="413ea-190">このアクセス確認のための意思決定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="413ea-190">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="413ea-191">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="413ea-191">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="413ea-192">呼び出し元、呼び出し元が、校閲者である場合の意思決定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="413ea-192">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="413ea-193">[accessReview](accessreview.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="413ea-193">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="413ea-194">アクセス レビューのコレクション インスタンスの過去、現在、将来、このオブジェクトが定期的なアクセスの確認である場合。</span><span class="sxs-lookup"><span data-stu-id="413ea-194">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="413ea-195">オブジェクトにこれらの関係が存在するかどうかは、オブジェクトは、1 回限りのアクセスの確認、一連の定期的なアクセスの確認、または定期的なアクセス確認のインスタンスかどうかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="413ea-195">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="413ea-196">シナリオ</span><span class="sxs-lookup"><span data-stu-id="413ea-196">Scenario</span></span> | <span data-ttu-id="413ea-197">校閲者はありますか。</span><span class="sxs-lookup"><span data-stu-id="413ea-197">Has reviewers?</span></span> | <span data-ttu-id="413ea-198">意思決定と myDecisions を持つでしょうか。</span><span class="sxs-lookup"><span data-stu-id="413ea-198">Has decisions and myDecisions?</span></span> | <span data-ttu-id="413ea-199">インスタンスが存在するか。</span><span class="sxs-lookup"><span data-stu-id="413ea-199">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="413ea-200">1 回限りのアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="413ea-200">One-time access review</span></span>|<span data-ttu-id="413ea-201">はい</span><span class="sxs-lookup"><span data-stu-id="413ea-201">Yes</span></span> | <span data-ttu-id="413ea-202">開始後、[はい]</span><span class="sxs-lookup"><span data-stu-id="413ea-202">Yes, once started</span></span> | <span data-ttu-id="413ea-203">いいえ</span><span class="sxs-lookup"><span data-stu-id="413ea-203">No</span></span> |
| <span data-ttu-id="413ea-204">定期的なアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="413ea-204">Recurring access review</span></span> | <span data-ttu-id="413ea-205">はい</span><span class="sxs-lookup"><span data-stu-id="413ea-205">Yes</span></span> | <span data-ttu-id="413ea-206">いいえ</span><span class="sxs-lookup"><span data-stu-id="413ea-206">No</span></span> | <span data-ttu-id="413ea-207">はい</span><span class="sxs-lookup"><span data-stu-id="413ea-207">Yes</span></span> |
| <span data-ttu-id="413ea-208">インスタンスの定期的なアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="413ea-208">Instance of a recurring access review</span></span> | <span data-ttu-id="413ea-209">はい</span><span class="sxs-lookup"><span data-stu-id="413ea-209">Yes</span></span> | <span data-ttu-id="413ea-210">開始後、[はい]</span><span class="sxs-lookup"><span data-stu-id="413ea-210">Yes, once started</span></span> | <span data-ttu-id="413ea-211">いいえ</span><span class="sxs-lookup"><span data-stu-id="413ea-211">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="413ea-212">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="413ea-212">JSON representation</span></span>

<span data-ttu-id="413ea-213">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="413ea-213">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="413ea-214">AccessReviewSettings 型</span><span class="sxs-lookup"><span data-stu-id="413ea-214">The accessReviewSettings type</span></span>

<span data-ttu-id="413ea-215">`accessReviewSettings` 、アクセス確認を開始するときに、機能の動作を制御するのには、アクセス確認を作成するときに追加の設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="413ea-215">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="413ea-216">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="413ea-216">This type has the following properties:</span></span> 

| <span data-ttu-id="413ea-217">プロパティ</span><span class="sxs-lookup"><span data-stu-id="413ea-217">Property</span></span>                     | <span data-ttu-id="413ea-218">型</span><span class="sxs-lookup"><span data-stu-id="413ea-218">Type</span></span>                      | <span data-ttu-id="413ea-219">説明</span><span class="sxs-lookup"><span data-stu-id="413ea-219">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="413ea-220">校閲者とレビュー作成者にメールの送信が有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="413ea-220">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="413ea-221">校閲者に送信の通知メールが有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="413ea-221">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="413ea-222">校閲者がアクセスを確認するときに妥当性を提供するために必要かどうかを示すためにフラグを設定します。</span><span class="sxs-lookup"><span data-stu-id="413ea-222">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="413ea-223">校閲者を表示するユーザー ・ アクティビティの日数です。</span><span class="sxs-lookup"><span data-stu-id="413ea-223">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="413ea-224">レビュー担当者が指定されていません 1 つで auto-apply を使用する場合にこの機能が、意思決定を設定するかどうかを示すフラグが有効になります。</span><span class="sxs-lookup"><span data-stu-id="413ea-224">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="413ea-225">方法の詳細設定機能は、以下で説明されている auto-apply で使用するため、レビュー決定を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="413ea-225">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="413ea-226">定期的なアイテムを以下に示す詳細な設定です。</span><span class="sxs-lookup"><span data-stu-id="413ea-226">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="413ea-227">示すかどうかの自動適用機能により、ターゲット オブジェクトのアクセス リソースを自動的に変更が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="413ea-227">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="413ea-228">有効でない場合ユーザーする必要があります、レビューが完了すると、適用のアクセス確認。</span><span class="sxs-lookup"><span data-stu-id="413ea-228">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="413ea-229">校閲者への推奨事項を表示が有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="413ea-229">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |



## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="413ea-230">AutoReviewSettings 型</span><span class="sxs-lookup"><span data-stu-id="413ea-230">The autoReviewSettings type</span></span>

<span data-ttu-id="413ea-231">`autoReviewSettings`が組み込まれて、アクセス設定の確認、および、アクセス確認が完了したときに、機能の動作を指定します。</span><span class="sxs-lookup"><span data-stu-id="413ea-231">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="413ea-232">型が 1 つのプロパティを持つ`notReviewedResult`。</span><span class="sxs-lookup"><span data-stu-id="413ea-232">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="413ea-233">プロパティ</span><span class="sxs-lookup"><span data-stu-id="413ea-233">Property</span></span>                     | <span data-ttu-id="413ea-234">型</span><span class="sxs-lookup"><span data-stu-id="413ea-234">Type</span></span>     | <span data-ttu-id="413ea-235">説明</span><span class="sxs-lookup"><span data-stu-id="413ea-235">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="413ea-236">`Approve`、`Deny`、`Recommendation` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="413ea-236">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="413ea-237">AccessReviewRecurrenceSettings 型</span><span class="sxs-lookup"><span data-stu-id="413ea-237">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="413ea-238">`accessReviewRecurrenceSettings` 、アクセス設定の確認、内で埋め込まれ、アクセス確認が定期的に繰り返されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="413ea-238">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="413ea-239">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="413ea-239">This type has the following properties:</span></span>

| <span data-ttu-id="413ea-240">プロパティ</span><span class="sxs-lookup"><span data-stu-id="413ea-240">Property</span></span>                     | <span data-ttu-id="413ea-241">型</span><span class="sxs-lookup"><span data-stu-id="413ea-241">Type</span></span>                                                                                                          | <span data-ttu-id="413ea-242">説明</span><span class="sxs-lookup"><span data-stu-id="413ea-242">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="413ea-243">1 つである必要があります、定期的な間隔の`onetime`、 `weekly`、 `monthly`、 `quarterly`、または`annual`。</span><span class="sxs-lookup"><span data-stu-id="413ea-243">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="413ea-244">どのように、定期的なアイテムを終了します。</span><span class="sxs-lookup"><span data-stu-id="413ea-244">How the recurrence ends.</span></span> <span data-ttu-id="413ea-245">場合`Never`、定期的な一連の明示的な終了はありません。</span><span class="sxs-lookup"><span data-stu-id="413ea-245">If it is `Never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="413ea-246">場合`endBy`、定期的なアイテムが、特定の日付に終了します。</span><span class="sxs-lookup"><span data-stu-id="413ea-246">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="413ea-247">場合`occurrences`後、シリーズを終了し、`recurrentCount`レビューのインスタンスを完了します。</span><span class="sxs-lookup"><span data-stu-id="413ea-247">If it is `occurrences`, then the series ends after `recurrentCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="413ea-248">定期的な予定の日の期間です。</span><span class="sxs-lookup"><span data-stu-id="413ea-248">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="413ea-249">反復数場合の値`recurrenceEndType`、 `occurrences`、またはそれ以外は 0 です。</span><span class="sxs-lookup"><span data-stu-id="413ea-249">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |



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
