---
title: accessReview リソースの種類
description: 'Azure AD にアクセス確認機能を`accessReview`、アクセス確認を表します。  '
localization_priority: Normal
ms.openlocfilehash: 283fed0f9e96ca9d0f9cdf06fdfee824326c038d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826076"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="ac5d2-103">accessReview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac5d2-103">accessReview resource type</span></span>

> <span data-ttu-id="ac5d2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac5d2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac5d2-106">Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `accessReview` 、アクセス確認を表します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="ac5d2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac5d2-107">Methods</span></span>

| <span data-ttu-id="ac5d2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac5d2-108">Method</span></span>           | <span data-ttu-id="ac5d2-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ac5d2-109">Return Type</span></span>    |<span data-ttu-id="ac5d2-110">説明</span><span class="sxs-lookup"><span data-stu-id="ac5d2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac5d2-111">AccessReview を取得します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-111">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="ac5d2-112">accessReview</span><span class="sxs-lookup"><span data-stu-id="ac5d2-112">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="ac5d2-113">特定の id を持つ、アクセス確認を取得します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-113">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="ac5d2-114">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-114">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="ac5d2-115">accessReview</span><span class="sxs-lookup"><span data-stu-id="ac5d2-115">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="ac5d2-116">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-116">Create a new accessReview.</span></span> |
|[<span data-ttu-id="ac5d2-117">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-117">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="ac5d2-118">なし。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-118">None.</span></span>   | <span data-ttu-id="ac5d2-119">AccessReview を削除します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-119">Delete an accessReview.</span></span> |
|[<span data-ttu-id="ac5d2-120">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-120">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="ac5d2-121">accessReview</span><span class="sxs-lookup"><span data-stu-id="ac5d2-121">accessReview</span></span>](accessreview.md) | <span data-ttu-id="ac5d2-122">AccessReview を更新します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-122">Update an accessReview.</span></span> |
|[<span data-ttu-id="ac5d2-123">AccessReview の校閲者の一覧</span><span class="sxs-lookup"><span data-stu-id="ac5d2-123">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="ac5d2-124">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="ac5d2-124">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="ac5d2-125">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-125">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="ac5d2-126">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-126">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="ac5d2-127">なし。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-127">None.</span></span>   |   <span data-ttu-id="ac5d2-128">AccessReview には、レビュー担当者を追加します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-128">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="ac5d2-129">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-129">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="ac5d2-130">なし。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-130">None.</span></span>  |   <span data-ttu-id="ac5d2-131">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-131">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="ac5d2-132">リストの accessReview の決定</span><span class="sxs-lookup"><span data-stu-id="ac5d2-132">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="ac5d2-133">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ac5d2-133">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="ac5d2-134">AccessReview の決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-134">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="ac5d2-135">マイ accessReview の決定事項を表示します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-135">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="ac5d2-136">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ac5d2-136">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="ac5d2-137">参照者、accessReview の自分の意思決定を取得します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-137">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="ac5d2-138">AccessReview アラームを送信します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-138">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="ac5d2-139">なし。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-139">None.</span></span>   |   <span data-ttu-id="ac5d2-140">AccessReview のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-140">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="ac5d2-141">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-141">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="ac5d2-142">なし。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-142">None.</span></span>   |   <span data-ttu-id="ac5d2-143">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-143">Stop an accessReview.</span></span> |
|[<span data-ttu-id="ac5d2-144">リセット accessReview 決定</span><span class="sxs-lookup"><span data-stu-id="ac5d2-144">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="ac5d2-145">なし。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-145">None.</span></span>   |   <span data-ttu-id="ac5d2-146">進行中の accessReview の決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-146">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="ac5d2-147">AccessReview の決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-147">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="ac5d2-148">なし。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-148">None.</span></span>   |   <span data-ttu-id="ac5d2-149">完了した accessReview からの決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-149">Apply the decisions from a completed accessReview.</span></span>|

## <a name="permissions"></a><span data-ttu-id="ac5d2-150">Permissions</span><span class="sxs-lookup"><span data-stu-id="ac5d2-150">Permissions</span></span>

|<span data-ttu-id="ac5d2-151">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac5d2-151">Permission type</span></span>                        | <span data-ttu-id="ac5d2-152">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac5d2-152">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac5d2-153">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac5d2-153">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac5d2-154">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac5d2-154">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="ac5d2-155">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac5d2-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac5d2-156">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-156">Not supported.</span></span> |
|<span data-ttu-id="ac5d2-157">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac5d2-157">Application</span></span>                            | <span data-ttu-id="ac5d2-158">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-158">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="ac5d2-159">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-159">Properties</span></span>
| <span data-ttu-id="ac5d2-160">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-160">Property</span></span>     | <span data-ttu-id="ac5d2-161">種類</span><span class="sxs-lookup"><span data-stu-id="ac5d2-161">Type</span></span>   |<span data-ttu-id="ac5d2-162">説明</span><span class="sxs-lookup"><span data-stu-id="ac5d2-162">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="ac5d2-163">機能に割り当てられた一意の識別子アクセス レビューします。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-163">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="ac5d2-164">アクセス確認の名前です。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-164">The access review name.</span></span> <span data-ttu-id="ac5d2-165">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-165">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="ac5d2-166">日付と時刻と、レビューを開始する予定です。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-166">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="ac5d2-167">将来の日付可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-167">This could be a date in the future.</span></span>  <span data-ttu-id="ac5d2-168">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-168">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="ac5d2-169">レビューの終了がスケジュールされているときの日時。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-169">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="ac5d2-170">これは、少なくとも 1 つの日を開始日より後でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-170">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="ac5d2-171">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-171">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="ac5d2-172">この読み取り専用フィールドは、accessReview の現在の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-172">This read-only field specifies the current status of an accessReview.</span></span> <span data-ttu-id="ac5d2-173">標準的な状態には、 `Initializing`、 `NotStarted`、 `Starting`、`InProgress`、 `Completing`、 `Completed`、`AutoReviewing`と`AutoReviewed`。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-173">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="ac5d2-174">アクセス レビュー作成者は、校閲者を表示して説明します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-174">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="ac5d2-175">業務フローのテンプレートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-175">The business flow template identifier.</span></span> <span data-ttu-id="ac5d2-176">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-176">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="ac5d2-177">関連付けの種類、対象のオブジェクトのいずれかの校閲者の`self`、`delegate`または`entityOwners`。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-177">The relationship type of reviewer to the target object, one of `self`, `delegate` or `entityOwners`.</span></span> <span data-ttu-id="ac5d2-178">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-178">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="ac5d2-179">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="ac5d2-179">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="ac5d2-180">このレビューを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-180">The user who created this review.</span></span> |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="ac5d2-181">アクセス権を確認するオブジェクトは、アクセス権限の割り当て、グループへのユーザーのメンバーシップ、またはアプリケーションへのユーザーの割り当てなどのこと。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-181">The object for which the access reviews is of the access rights assignments, such as the memberships of users to a group or assignments of users to an application.</span></span> <span data-ttu-id="ac5d2-182">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-182">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="ac5d2-183">AccessReview の設定は、以下の種類の定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-183">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="ac5d2-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-184">Relationships</span></span>




| <span data-ttu-id="ac5d2-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-185">Relationship</span></span> | <span data-ttu-id="ac5d2-186">型</span><span class="sxs-lookup"><span data-stu-id="ac5d2-186">Type</span></span>   |<span data-ttu-id="ac5d2-187">説明</span><span class="sxs-lookup"><span data-stu-id="ac5d2-187">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="ac5d2-188">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="ac5d2-188">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="ac5d2-189">アクセス レビュー reviewerType 型の場合、アクセス確認などの校閲者のコレクション`delegate`。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-189">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="ac5d2-190">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ac5d2-190">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="ac5d2-191">このアクセス確認のための意思決定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-191">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="ac5d2-192">[accessReviewDecision](accessreviewdecision.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ac5d2-192">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="ac5d2-193">呼び出し元、呼び出し元が、校閲者である場合の意思決定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-193">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="ac5d2-194">[accessReview](accessreview.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ac5d2-194">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="ac5d2-195">アクセス レビューのコレクション インスタンスの過去、現在、将来、このオブジェクトが定期的なアクセスの確認である場合。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-195">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="ac5d2-196">オブジェクトに関係があるかどうかは、オブジェクトは、1 回限りのアクセスの確認、一連の定期的なアクセスの確認、または定期的なアクセス確認のインスタンスかどうかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-196">Whether there are relationships present on an object, depend upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="ac5d2-197">シナリオ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-197">Scenario</span></span> | <span data-ttu-id="ac5d2-198">校閲者はありますか。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-198">Has reviewers?</span></span> | <span data-ttu-id="ac5d2-199">意思決定と myDecisions を持つでしょうか。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-199">Has decisions and myDecisions?</span></span> | <span data-ttu-id="ac5d2-200">インスタンスが存在するか。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-200">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="ac5d2-201">1 回限りのアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="ac5d2-201">One-time access review</span></span>|<span data-ttu-id="ac5d2-202">はい</span><span class="sxs-lookup"><span data-stu-id="ac5d2-202">Yes</span></span> | <span data-ttu-id="ac5d2-203">開始後、[はい]</span><span class="sxs-lookup"><span data-stu-id="ac5d2-203">Yes, once started</span></span> | <span data-ttu-id="ac5d2-204">いいえ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-204">No</span></span> |
| <span data-ttu-id="ac5d2-205">定期的なアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="ac5d2-205">Recurring access review</span></span> | <span data-ttu-id="ac5d2-206">はい</span><span class="sxs-lookup"><span data-stu-id="ac5d2-206">Yes</span></span> | <span data-ttu-id="ac5d2-207">いいえ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-207">No</span></span> | <span data-ttu-id="ac5d2-208">はい</span><span class="sxs-lookup"><span data-stu-id="ac5d2-208">Yes</span></span> |
| <span data-ttu-id="ac5d2-209">インスタンスの定期的なアクセスの確認</span><span class="sxs-lookup"><span data-stu-id="ac5d2-209">Instance of a recurring access review</span></span> | <span data-ttu-id="ac5d2-210">はい</span><span class="sxs-lookup"><span data-stu-id="ac5d2-210">Yes</span></span> | <span data-ttu-id="ac5d2-211">開始後、[はい]</span><span class="sxs-lookup"><span data-stu-id="ac5d2-211">Yes, once started</span></span> | <span data-ttu-id="ac5d2-212">いいえ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-212">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ac5d2-213">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac5d2-213">JSON representation</span></span>

<span data-ttu-id="ac5d2-214">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-214">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="ac5d2-215">AccessReviewSettings 型</span><span class="sxs-lookup"><span data-stu-id="ac5d2-215">The accessReviewSettings type</span></span>

<span data-ttu-id="ac5d2-216">`accessReviewSettings` 、アクセス確認を開始するときに、機能の動作を制御するのには、アクセス確認を作成するときに追加の設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-216">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="ac5d2-217">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-217">This type has the following properties:</span></span> 

| <span data-ttu-id="ac5d2-218">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-218">Property</span></span>                     | <span data-ttu-id="ac5d2-219">種類</span><span class="sxs-lookup"><span data-stu-id="ac5d2-219">Type</span></span>                      | <span data-ttu-id="ac5d2-220">説明</span><span class="sxs-lookup"><span data-stu-id="ac5d2-220">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="ac5d2-221">校閲者とレビュー作成者にメールの送信が有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-221">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="ac5d2-222">校閲者に送信の通知メールが有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-222">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="ac5d2-223">校閲者がアクセスを確認するときに妥当性を提供するために必要かどうかを示すためにフラグを設定します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-223">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="ac5d2-224">校閲者を表示するユーザー ・ アクティビティの日数です。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-224">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="ac5d2-225">レビュー担当者が指定されていません 1 つで auto-apply を使用する場合にこの機能が、意思決定を設定するかどうかを示すフラグが有効になります。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-225">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="ac5d2-226">方法の詳細設定機能は、以下で説明されている auto-apply で使用するため、レビュー決定を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-226">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="ac5d2-227">定期的なアイテムを以下に示す詳細な設定です。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-227">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="ac5d2-228">示すかどうかの自動適用機能により、ターゲット オブジェクトのアクセス リソースを自動的に変更が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-228">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="ac5d2-229">有効でない場合は、アクセス確認が完了した後、ユーザーは後アクセス レビューの変更を適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-229">If not enabled, a user must subsequently apply the change of the access review after the access review is completed.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="ac5d2-230">校閲者への推奨事項を表示が有効になっているかどうかを示すフラグです。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-230">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |



## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="ac5d2-231">AutoReviewSettings 型</span><span class="sxs-lookup"><span data-stu-id="ac5d2-231">The autoReviewSettings type</span></span>

<span data-ttu-id="ac5d2-232">`autoReviewSettings`が組み込まれて、アクセス設定の確認、および、アクセス確認が完了したときに、機能の動作を指定します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-232">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="ac5d2-233">型が 1 つのプロパティを持つ`notReviewedResult`。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-233">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="ac5d2-234">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-234">Property</span></span>                     | <span data-ttu-id="ac5d2-235">種類</span><span class="sxs-lookup"><span data-stu-id="ac5d2-235">Type</span></span>     | <span data-ttu-id="ac5d2-236">説明</span><span class="sxs-lookup"><span data-stu-id="ac5d2-236">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="ac5d2-237">`Approve`、`Deny`、`Recommendation` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-237">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="ac5d2-238">AccessReviewRecurrenceSettings 型</span><span class="sxs-lookup"><span data-stu-id="ac5d2-238">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="ac5d2-239">`accessReviewRecurrenceSettings` 、アクセス設定の確認、内で埋め込まれ、アクセス確認が定期的に繰り返されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-239">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="ac5d2-240">この型には、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-240">This type has the following properties:</span></span>

| <span data-ttu-id="ac5d2-241">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac5d2-241">Property</span></span>                     | <span data-ttu-id="ac5d2-242">種類</span><span class="sxs-lookup"><span data-stu-id="ac5d2-242">Type</span></span>                                                                                                          | <span data-ttu-id="ac5d2-243">説明</span><span class="sxs-lookup"><span data-stu-id="ac5d2-243">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="ac5d2-244">1 つである必要があります、定期的な間隔の`onetime`、 `weekly`、 `monthly`、`quarterly`または`annual`。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-244">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly` or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="ac5d2-245">どのように、定期的なアイテムは終了します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-245">How the recurrence will end.</span></span> <span data-ttu-id="ac5d2-246">いずれかのことができます`Never`、定期的な予定の系列の明示的な終了が行われない`Endby`、定期的なアイテムを特定の日付に終了して`occurrences`、レビューのインスタンスの特定の数を完了した後に、シリーズを終了します。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-246">It can be one of `Never`,that there is no explicit end of the recurrence series, `Endby`, that the recurrence ends at a certain date, and `occurrences`, that the series ends after certain number of instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="ac5d2-247">定期的な予定の日の期間です。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-247">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="ac5d2-248">反復数場合の値`recurrenceEndType`、 `occurrences`。</span><span class="sxs-lookup"><span data-stu-id="ac5d2-248">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`.</span></span>                                                        |



<!-- {
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
