---
title: accessReview リソースの種類
description: 'Azure AD にアクセス確認機能を`accessReview`、アクセス確認を表します。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9099b1ec55a8ed017f77757d527abbd7e45bdf6
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016738"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="abafc-103">accessReview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="abafc-103">accessReview resource type</span></span>

> <span data-ttu-id="abafc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="abafc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abafc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abafc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abafc-106">Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `accessReview` 、アクセス確認を表します。</span><span class="sxs-lookup"><span data-stu-id="abafc-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="abafc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="abafc-107">Methods</span></span>

| <span data-ttu-id="abafc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="abafc-108">Method</span></span>           | <span data-ttu-id="abafc-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="abafc-109">Return Type</span></span>    |<span data-ttu-id="abafc-110">説明</span><span class="sxs-lookup"><span data-stu-id="abafc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="abafc-111">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="abafc-111">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="abafc-112">accessReview</span><span class="sxs-lookup"><span data-stu-id="abafc-112">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="abafc-113">特定の id を持つ、アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="abafc-113">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="abafc-114">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="abafc-114">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="abafc-115">accessReview</span><span class="sxs-lookup"><span data-stu-id="abafc-115">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="abafc-116">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="abafc-116">Create a new accessReview.</span></span> |
|[<span data-ttu-id="abafc-117">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="abafc-117">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="abafc-118">なし。</span><span class="sxs-lookup"><span data-stu-id="abafc-118">None.</span></span>   | <span data-ttu-id="abafc-119">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="abafc-119">Delete an accessReview.</span></span> |
|[<span data-ttu-id="abafc-120">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="abafc-120">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="abafc-121">accessReview</span><span class="sxs-lookup"><span data-stu-id="abafc-121">accessReview</span></span>](accessreview.md) | <span data-ttu-id="abafc-122">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="abafc-122">Update an accessReview.</span></span> |
|[<span data-ttu-id="abafc-123">AccessReview の校閲者の一覧</span><span class="sxs-lookup"><span data-stu-id="abafc-123">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="abafc-124">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="abafc-124">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="abafc-125">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="abafc-125">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="abafc-126">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="abafc-126">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="abafc-127">なし。</span><span class="sxs-lookup"><span data-stu-id="abafc-127">None.</span></span>   |   <span data-ttu-id="abafc-128">AccessReview には、レビュー担当者を追加します。</span><span class="sxs-lookup"><span data-stu-id="abafc-128">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="abafc-129">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="abafc-129">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="abafc-130">なし。</span><span class="sxs-lookup"><span data-stu-id="abafc-130">None.</span></span>  |   <span data-ttu-id="abafc-131">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="abafc-131">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="abafc-132">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="abafc-132">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="abafc-133">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="abafc-133">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="abafc-134">AccessReview の決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="abafc-134">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="abafc-135">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="abafc-135">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="abafc-136">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="abafc-136">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="abafc-137">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="abafc-137">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="abafc-138">AccessReview アラームを送信します。</span><span class="sxs-lookup"><span data-stu-id="abafc-138">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="abafc-139">なし。</span><span class="sxs-lookup"><span data-stu-id="abafc-139">None.</span></span>   |   <span data-ttu-id="abafc-140">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="abafc-140">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="abafc-141">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="abafc-141">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="abafc-142">なし。</span><span class="sxs-lookup"><span data-stu-id="abafc-142">None.</span></span>   |   <span data-ttu-id="abafc-143">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="abafc-143">Stop an accessReview.</span></span> |
|[<span data-ttu-id="abafc-144">リセット accessReview 決定</span><span class="sxs-lookup"><span data-stu-id="abafc-144">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="abafc-145">なし。</span><span class="sxs-lookup"><span data-stu-id="abafc-145">None.</span></span>   |   <span data-ttu-id="abafc-146">進行中の accessReview の決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="abafc-146">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="abafc-147">AccessReview の決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="abafc-147">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="abafc-148">なし。</span><span class="sxs-lookup"><span data-stu-id="abafc-148">None.</span></span>   |   <span data-ttu-id="abafc-149">完了した accessReview からの決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="abafc-149">Apply the decisions from a completed accessReview.</span></span>|

## <a name="permissions"></a><span data-ttu-id="abafc-150">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="abafc-150">Permissions</span></span>

|<span data-ttu-id="abafc-151">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abafc-151">Permission type</span></span>                        | <span data-ttu-id="abafc-152">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="abafc-152">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="abafc-153">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="abafc-153">Delegated (work or school account)</span></span>     | <span data-ttu-id="abafc-154">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abafc-154">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="abafc-155">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="abafc-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abafc-156">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abafc-156">Not supported.</span></span> |
|<span data-ttu-id="abafc-157">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abafc-157">Application</span></span>                            | <span data-ttu-id="abafc-158">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abafc-158">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="abafc-159">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abafc-159">Properties</span></span>
| <span data-ttu-id="abafc-160">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abafc-160">Property</span></span>     | <span data-ttu-id="abafc-161">型</span><span class="sxs-lookup"><span data-stu-id="abafc-161">Type</span></span>   |<span data-ttu-id="abafc-162">説明</span><span class="sxs-lookup"><span data-stu-id="abafc-162">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="abafc-163">機能に割り当てられた一意の識別子アクセス レビューします。</span><span class="sxs-lookup"><span data-stu-id="abafc-163">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="abafc-164">アクセス確認の名前です。</span><span class="sxs-lookup"><span data-stu-id="abafc-164">The access review name.</span></span> <span data-ttu-id="abafc-165">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="abafc-165">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="abafc-166">日付と時刻と、レビューを開始する予定です。</span><span class="sxs-lookup"><span data-stu-id="abafc-166">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="abafc-167">将来の日付可能性があります。</span><span class="sxs-lookup"><span data-stu-id="abafc-167">This could be a date in the future.</span></span>  <span data-ttu-id="abafc-168">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="abafc-168">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="abafc-169">レビューの終了がスケジュールされているときの日時。</span><span class="sxs-lookup"><span data-stu-id="abafc-169">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="abafc-170">これは、少なくとも 1 つの日を開始日より後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="abafc-170">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="abafc-171">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="abafc-171">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="abafc-172">この読み取り専用フィールドは、accessReview のステータスを指定します。</span><span class="sxs-lookup"><span data-stu-id="abafc-172">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="abafc-173">標準的な状態には、 `Initializing`、 `NotStarted`、 `Starting`、`InProgress`、 `Completing`、 `Completed`、`AutoReviewing`と`AutoReviewed`。</span><span class="sxs-lookup"><span data-stu-id="abafc-173">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="abafc-174">アクセス レビュー作成者は、校閲者を表示して説明します。</span><span class="sxs-lookup"><span data-stu-id="abafc-174">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="abafc-175">業務フローのテンプレートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="abafc-175">The business flow template identifier.</span></span> <span data-ttu-id="abafc-176">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="abafc-176">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="abafc-177">関連付けの種類、対象のオブジェクトのいずれかの校閲者の`self`、`delegated`または`entityOwners`。</span><span class="sxs-lookup"><span data-stu-id="abafc-177">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="abafc-178">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="abafc-178">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="abafc-179">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="abafc-179">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="abafc-180">このレビューを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="abafc-180">The user who created this review.</span></span> |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="abafc-181">アクセス権を確認するオブジェクトがアクセス権限の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="abafc-181">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="abafc-182">グループでは、ユーザーのグループ メンバーシップの確認のため、またはアプリケーションへのユーザーの割り当ての詳細についてはアプリケーションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="abafc-182">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="abafc-183">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="abafc-183">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="abafc-184">AccessReview の設定は、以下の種類の定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abafc-184">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="abafc-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="abafc-185">Relationships</span></span>




| <span data-ttu-id="abafc-186">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="abafc-186">Relationship</span></span> | <span data-ttu-id="abafc-187">型</span><span class="sxs-lookup"><span data-stu-id="abafc-187">Type</span></span>   |<span data-ttu-id="abafc-188">説明</span><span class="sxs-lookup"><span data-stu-id="abafc-188">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="abafc-189">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="abafc-189">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="abafc-190">アクセス レビュー reviewerType 型の場合、アクセス確認などの校閲者のコレクション`delegate`。</span><span class="sxs-lookup"><span data-stu-id="abafc-190">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="abafc-191">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="abafc-191">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="abafc-192">このアクセス確認のための意思決定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="abafc-192">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="abafc-193">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="abafc-193">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="abafc-194">呼び出し元、呼び出し元が、校閲者である場合の意思決定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="abafc-194">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="abafc-195">[accessReview](accessreview.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="abafc-195">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="abafc-196">アクセス レビューのコレクション インスタンスの過去、現在、将来、このオブジェクトが定期的なアクセスの確認である場合。</span><span class="sxs-lookup"><span data-stu-id="abafc-196">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="abafc-197">オブジェクトにこれらの関係が存在するかどうかは、オブジェクトは、1 回限りのアクセスの確認、一連の定期的なアクセスの確認、または定期的なアクセス確認のインスタンスかどうかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="abafc-197">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="abafc-198">シナリオ</span><span class="sxs-lookup"><span data-stu-id="abafc-198">Scenario</span></span> | <span data-ttu-id="abafc-199">校閲者はありますか。</span><span class="sxs-lookup"><span data-stu-id="abafc-199">Has reviewers?</span></span> | <span data-ttu-id="abafc-200">意思決定と myDecisions を持つでしょうか。</span><span class="sxs-lookup"><span data-stu-id="abafc-200">Has decisions and myDecisions?</span></span> | <span data-ttu-id="abafc-201">インスタンスが存在するか。</span><span class="sxs-lookup"><span data-stu-id="abafc-201">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="abafc-202">1 回限りのアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="abafc-202">One-time access review</span></span>|<span data-ttu-id="abafc-203">はい</span><span class="sxs-lookup"><span data-stu-id="abafc-203">Yes</span></span> | <span data-ttu-id="abafc-204">開始後、[はい]</span><span class="sxs-lookup"><span data-stu-id="abafc-204">Yes, once started</span></span> | <span data-ttu-id="abafc-205">いいえ</span><span class="sxs-lookup"><span data-stu-id="abafc-205">No</span></span> |
| <span data-ttu-id="abafc-206">定期的なアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="abafc-206">Recurring access review</span></span> | <span data-ttu-id="abafc-207">はい</span><span class="sxs-lookup"><span data-stu-id="abafc-207">Yes</span></span> | <span data-ttu-id="abafc-208">いいえ</span><span class="sxs-lookup"><span data-stu-id="abafc-208">No</span></span> | <span data-ttu-id="abafc-209">はい</span><span class="sxs-lookup"><span data-stu-id="abafc-209">Yes</span></span> |
| <span data-ttu-id="abafc-210">インスタンスの定期的なアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="abafc-210">Instance of a recurring access review</span></span> | <span data-ttu-id="abafc-211">はい</span><span class="sxs-lookup"><span data-stu-id="abafc-211">Yes</span></span> | <span data-ttu-id="abafc-212">開始後、[はい]</span><span class="sxs-lookup"><span data-stu-id="abafc-212">Yes, once started</span></span> | <span data-ttu-id="abafc-213">いいえ</span><span class="sxs-lookup"><span data-stu-id="abafc-213">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="abafc-214">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="abafc-214">JSON representation</span></span>

<span data-ttu-id="abafc-215">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="abafc-215">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="abafc-216">AccessReviewSettings 型</span><span class="sxs-lookup"><span data-stu-id="abafc-216">The accessReviewSettings type</span></span>

<span data-ttu-id="abafc-217">`accessReviewSettings` 、アクセス確認を開始するときに、機能の動作を制御するのには、アクセス確認を作成するときに追加の設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="abafc-217">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="abafc-218">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="abafc-218">This type has the following properties:</span></span> 

| <span data-ttu-id="abafc-219">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abafc-219">Property</span></span>                     | <span data-ttu-id="abafc-220">型</span><span class="sxs-lookup"><span data-stu-id="abafc-220">Type</span></span>                      | <span data-ttu-id="abafc-221">説明</span><span class="sxs-lookup"><span data-stu-id="abafc-221">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="abafc-222">校閲者とレビュー作成者にメールの送信が有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="abafc-222">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="abafc-223">校閲者に送信の通知メールが有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="abafc-223">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="abafc-224">校閲者がアクセスを確認するときに妥当性を提供するために必要かどうかを示すためにフラグを設定します。</span><span class="sxs-lookup"><span data-stu-id="abafc-224">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="abafc-225">校閲者を表示するユーザー ・ アクティビティの日数です。</span><span class="sxs-lookup"><span data-stu-id="abafc-225">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="abafc-226">レビュー担当者が指定されていません 1 つで auto-apply を使用する場合にこの機能が、意思決定を設定するかどうかを示すフラグが有効になります。</span><span class="sxs-lookup"><span data-stu-id="abafc-226">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="abafc-227">方法の詳細設定機能は、以下で説明されている auto-apply で使用するため、レビュー決定を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="abafc-227">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="abafc-228">定期的なアイテムを以下に示す詳細な設定です。</span><span class="sxs-lookup"><span data-stu-id="abafc-228">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="abafc-229">示すかどうかの自動適用機能により、ターゲット オブジェクトのアクセス リソースを自動的に変更が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="abafc-229">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="abafc-230">有効でない場合ユーザーする必要があります、レビューが完了すると、適用のアクセス確認。</span><span class="sxs-lookup"><span data-stu-id="abafc-230">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="abafc-231">校閲者への推奨事項を表示が有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="abafc-231">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |



## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="abafc-232">AutoReviewSettings 型</span><span class="sxs-lookup"><span data-stu-id="abafc-232">The autoReviewSettings type</span></span>

<span data-ttu-id="abafc-233">`autoReviewSettings`が組み込まれて、アクセス設定の確認、および、アクセス確認が完了したときに、機能の動作を指定します。</span><span class="sxs-lookup"><span data-stu-id="abafc-233">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="abafc-234">型が 1 つのプロパティを持つ`notReviewedResult`。</span><span class="sxs-lookup"><span data-stu-id="abafc-234">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="abafc-235">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abafc-235">Property</span></span>                     | <span data-ttu-id="abafc-236">型</span><span class="sxs-lookup"><span data-stu-id="abafc-236">Type</span></span>     | <span data-ttu-id="abafc-237">説明</span><span class="sxs-lookup"><span data-stu-id="abafc-237">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="abafc-238">`Approve`、`Deny`、`Recommendation` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="abafc-238">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="abafc-239">AccessReviewRecurrenceSettings 型</span><span class="sxs-lookup"><span data-stu-id="abafc-239">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="abafc-240">`accessReviewRecurrenceSettings` 、アクセス設定の確認、内で埋め込まれ、アクセス確認が定期的に繰り返されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="abafc-240">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="abafc-241">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="abafc-241">This type has the following properties:</span></span>

| <span data-ttu-id="abafc-242">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abafc-242">Property</span></span>                     | <span data-ttu-id="abafc-243">型</span><span class="sxs-lookup"><span data-stu-id="abafc-243">Type</span></span>                                                                                                          | <span data-ttu-id="abafc-244">説明</span><span class="sxs-lookup"><span data-stu-id="abafc-244">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="abafc-245">1 つである必要があります、定期的な間隔の`onetime`、 `weekly`、 `monthly`、 `quarterly`、または`annual`。</span><span class="sxs-lookup"><span data-stu-id="abafc-245">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="abafc-246">どのように、定期的なアイテムを終了します。</span><span class="sxs-lookup"><span data-stu-id="abafc-246">How the recurrence ends.</span></span> <span data-ttu-id="abafc-247">場合`Never`、定期的な一連の明示的な終了はありません。</span><span class="sxs-lookup"><span data-stu-id="abafc-247">If it is `Never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="abafc-248">場合`endBy`、定期的なアイテムが、特定の日付に終了します。</span><span class="sxs-lookup"><span data-stu-id="abafc-248">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="abafc-249">場合`occurrences`後、シリーズを終了し、`recurrentCount`レビューのインスタンスを完了します。</span><span class="sxs-lookup"><span data-stu-id="abafc-249">If it is `occurrences`, then the series ends after `recurrentCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="abafc-250">定期的な予定の日の期間です。</span><span class="sxs-lookup"><span data-stu-id="abafc-250">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="abafc-251">反復数場合の値`recurrenceEndType`、 `occurrences`、またはそれ以外は 0 です。</span><span class="sxs-lookup"><span data-stu-id="abafc-251">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |



<!-- {
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
