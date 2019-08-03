---
title: educationSubmission リソースの種類
description: 提出物は、割り当てによって所有されます。 提出は、個人 (またはグループ) が割り当てに対して有効になるリソースと、返される成績/フィードバックを表します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 27467548339dc01f7c95fe55bda159c0569c38ba
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173042"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="f55e2-104">educationSubmission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f55e2-104">educationSubmission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f55e2-105">提出物は、割り当てによって所有されます。</span><span class="sxs-lookup"><span data-stu-id="f55e2-105">Submissions are owned by an assignment.</span></span> <span data-ttu-id="f55e2-106">提出は、個人 (またはグループ) が割り当てに対して有効になるリソースと、返される成績/フィードバックを表します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-106">A submission represents the resources that an individual (or group) turn in for an assignment and the grade/feedback that is returned.</span></span>
<span data-ttu-id="f55e2-107">割り当てが発行されると、提出物は自動的に作成されます。</span><span class="sxs-lookup"><span data-stu-id="f55e2-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="f55e2-108">送信では、2つのリソースリストが所有されています。</span><span class="sxs-lookup"><span data-stu-id="f55e2-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="f55e2-109">リソースは、送信されたリソースが、学生が積極的に有効にしたリソースを表している間、ユーザー/グループの作業領域を表します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="f55e2-110">**注:** 状態は読み取り専用で、オブジェクトはアクションによってワークフローを通じて移動されます。</span><span class="sxs-lookup"><span data-stu-id="f55e2-110">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="f55e2-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="f55e2-111">Methods</span></span>

| <span data-ttu-id="f55e2-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="f55e2-112">Method</span></span>           | <span data-ttu-id="f55e2-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f55e2-113">Return Type</span></span>    |<span data-ttu-id="f55e2-114">説明</span><span class="sxs-lookup"><span data-stu-id="f55e2-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f55e2-115">EducationSubmission を取得する</span><span class="sxs-lookup"><span data-stu-id="f55e2-115">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="f55e2-116">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="f55e2-116">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="f55e2-117">**EducationSubmission**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f55e2-117">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="f55e2-118">リソースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f55e2-118">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="f55e2-119">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f55e2-119">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="f55e2-120">**EducationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-120">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="f55e2-121">SubmittedResources を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f55e2-121">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="f55e2-122">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f55e2-122">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="f55e2-123">**EducationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-123">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="f55e2-124">結果の一覧表示</span><span class="sxs-lookup"><span data-stu-id="f55e2-124">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="f55e2-125">[educationOutcome](educationoutcome.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f55e2-125">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="f55e2-126">**EducationOutcome**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-126">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="f55e2-127">Update</span><span class="sxs-lookup"><span data-stu-id="f55e2-127">Update</span></span>](../api/educationsubmission-update.md) | [<span data-ttu-id="f55e2-128">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="f55e2-128">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="f55e2-129">**EducationSubmission**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-129">Update an **educationSubmission** object.</span></span> |
|[<span data-ttu-id="f55e2-130">Return</span><span class="sxs-lookup"><span data-stu-id="f55e2-130">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="f55e2-131">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="f55e2-131">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="f55e2-132">教師は、return を使用して、成績/フィードバックを学生に表示できることを示します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-132">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="f55e2-133">Submit</span><span class="sxs-lookup"><span data-stu-id="f55e2-133">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="f55e2-134">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="f55e2-134">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="f55e2-135">学生は、submit を使用して割り当てを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f55e2-135">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="f55e2-136">これにより、リソースが [対象] の [ **Submittedresources** ] フォルダーにコピーされ、状態が更新されます。</span><span class="sxs-lookup"><span data-stu-id="f55e2-136">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="f55e2-137">送信取り消し</span><span class="sxs-lookup"><span data-stu-id="f55e2-137">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="f55e2-138">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="f55e2-138">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="f55e2-139">学生は、未送信を使用して、提出物の状態を送信前から作業に移行します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-139">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="f55e2-140">これにより、リソースが**workingResources**フォルダーにコピーされて、状況を更新して更新します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-140">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="f55e2-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f55e2-141">Properties</span></span>
| <span data-ttu-id="f55e2-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f55e2-142">Property</span></span>     | <span data-ttu-id="f55e2-143">型</span><span class="sxs-lookup"><span data-stu-id="f55e2-143">Type</span></span>   |<span data-ttu-id="f55e2-144">説明</span><span class="sxs-lookup"><span data-stu-id="f55e2-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f55e2-145">feedback</span><span class="sxs-lookup"><span data-stu-id="f55e2-145">feedback</span></span>|[<span data-ttu-id="f55e2-146">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="f55e2-146">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="f55e2-147">教師のメモを生徒に返すフィードバックプロパティを保持します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-147">Holds the feedback property which stores the teacher's notes back to students.</span></span>|
|<span data-ttu-id="f55e2-148">grade</span><span class="sxs-lookup"><span data-stu-id="f55e2-148">grade</span></span>|[<span data-ttu-id="f55e2-149">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="f55e2-149">educationAssignmentGrade</span></span>](educationassignmentgrade.md)|<span data-ttu-id="f55e2-150">教師がこの送信に割り当てる成績情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-150">Holds the grade information a teacher assigns to this submission.</span></span>|
|<span data-ttu-id="f55e2-151">id</span><span class="sxs-lookup"><span data-stu-id="f55e2-151">id</span></span>|<span data-ttu-id="f55e2-152">String</span><span class="sxs-lookup"><span data-stu-id="f55e2-152">String</span></span>| <span data-ttu-id="f55e2-153">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f55e2-153">Read-only.</span></span>|
|<span data-ttu-id="f55e2-154">受信者</span><span class="sxs-lookup"><span data-stu-id="f55e2-154">recipient</span></span>|[<span data-ttu-id="f55e2-155">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="f55e2-155">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="f55e2-156">この提出物が割り当てられるユーザー。</span><span class="sxs-lookup"><span data-stu-id="f55e2-156">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="f55e2-157">releasedBy</span><span class="sxs-lookup"><span data-stu-id="f55e2-157">releasedBy</span></span>|[<span data-ttu-id="f55e2-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="f55e2-158">identitySet</span></span>](identityset.md)|<span data-ttu-id="f55e2-159">この提出の状態をリリース済みに移動したユーザー。</span><span class="sxs-lookup"><span data-stu-id="f55e2-159">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="f55e2-160">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="f55e2-160">releasedDateTime</span></span>|<span data-ttu-id="f55e2-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f55e2-161">DateTimeOffset</span></span>|<span data-ttu-id="f55e2-162">提出物がいつリリースされたかを示します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-162">Moment in time when the submission was released.</span></span> <span data-ttu-id="f55e2-163">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f55e2-163">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f55e2-164">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f55e2-164">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f55e2-165">returnedBy</span><span class="sxs-lookup"><span data-stu-id="f55e2-165">returnedBy</span></span>|[<span data-ttu-id="f55e2-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="f55e2-166">identitySet</span></span>](identityset.md)|<span data-ttu-id="f55e2-167">この提出の状態を取得したユーザー。</span><span class="sxs-lookup"><span data-stu-id="f55e2-167">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="f55e2-168">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="f55e2-168">returnedDateTime</span></span>|<span data-ttu-id="f55e2-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f55e2-169">DateTimeOffset</span></span>|<span data-ttu-id="f55e2-170">送信が返された瞬間の時間。</span><span class="sxs-lookup"><span data-stu-id="f55e2-170">Moment in time when the submission was returned.</span></span> <span data-ttu-id="f55e2-171">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f55e2-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f55e2-172">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f55e2-172">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f55e2-173">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="f55e2-173">resourcesFolderUrl</span></span>|<span data-ttu-id="f55e2-174">String</span><span class="sxs-lookup"><span data-stu-id="f55e2-174">String</span></span>|<span data-ttu-id="f55e2-175">この送信のすべてのファイルリソースを格納する必要があるフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="f55e2-175">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="f55e2-176">status</span><span class="sxs-lookup"><span data-stu-id="f55e2-176">status</span></span>|<span data-ttu-id="f55e2-177">string</span><span class="sxs-lookup"><span data-stu-id="f55e2-177">string</span></span>| <span data-ttu-id="f55e2-178">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f55e2-178">Read-Only.</span></span> <span data-ttu-id="f55e2-179">使用可能な値: `working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="f55e2-179">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="f55e2-180">submittedBy</span><span class="sxs-lookup"><span data-stu-id="f55e2-180">submittedBy</span></span>|[<span data-ttu-id="f55e2-181">identitySet</span><span class="sxs-lookup"><span data-stu-id="f55e2-181">identitySet</span></span>](identityset.md)|<span data-ttu-id="f55e2-182">リソースを送信済み状態に移行したユーザー。</span><span class="sxs-lookup"><span data-stu-id="f55e2-182">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="f55e2-183">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="f55e2-183">submittedDateTime</span></span>|<span data-ttu-id="f55e2-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f55e2-184">DateTimeOffset</span></span>|<span data-ttu-id="f55e2-185">提出された状態に提出された時点の状態。</span><span class="sxs-lookup"><span data-stu-id="f55e2-185">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="f55e2-186">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f55e2-186">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f55e2-187">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f55e2-187">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f55e2-188">未提出者</span><span class="sxs-lookup"><span data-stu-id="f55e2-188">unsubmittedBy</span></span>|[<span data-ttu-id="f55e2-189">identitySet</span><span class="sxs-lookup"><span data-stu-id="f55e2-189">identitySet</span></span>](identityset.md)|<span data-ttu-id="f55e2-190">提出されたリソースを作業中の状態に移行したユーザー。</span><span class="sxs-lookup"><span data-stu-id="f55e2-190">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="f55e2-191">非 Submitteddatetime</span><span class="sxs-lookup"><span data-stu-id="f55e2-191">unsubmittedDateTime</span></span>|<span data-ttu-id="f55e2-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f55e2-192">DateTimeOffset</span></span>|<span data-ttu-id="f55e2-193">提出物が送信されてから作業中の状態に移行した時点の状態です。</span><span class="sxs-lookup"><span data-stu-id="f55e2-193">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="f55e2-194">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f55e2-194">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f55e2-195">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f55e2-195">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="f55e2-196">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f55e2-196">Relationships</span></span>
| <span data-ttu-id="f55e2-197">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f55e2-197">Relationship</span></span> | <span data-ttu-id="f55e2-198">型</span><span class="sxs-lookup"><span data-stu-id="f55e2-198">Type</span></span>   |<span data-ttu-id="f55e2-199">説明</span><span class="sxs-lookup"><span data-stu-id="f55e2-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f55e2-200">リソース</span><span class="sxs-lookup"><span data-stu-id="f55e2-200">resources</span></span>|<span data-ttu-id="f55e2-201">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f55e2-201">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="f55e2-202">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f55e2-202">Nullable.</span></span>|
|<span data-ttu-id="f55e2-203">submittedResources</span><span class="sxs-lookup"><span data-stu-id="f55e2-203">submittedResources</span></span>|<span data-ttu-id="f55e2-204">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f55e2-204">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="f55e2-205">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f55e2-205">Read-only.</span></span> <span data-ttu-id="f55e2-206">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f55e2-206">Nullable.</span></span>|
|<span data-ttu-id="f55e2-207">結果</span><span class="sxs-lookup"><span data-stu-id="f55e2-207">outcomes</span></span>|<span data-ttu-id="f55e2-208">[educationOutcome](educationOutcome.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f55e2-208">[educationOutcome](educationOutcome.md) collection</span></span>|<span data-ttu-id="f55e2-p111">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="f55e2-p111">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f55e2-211">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f55e2-211">JSON representation</span></span>

<span data-ttu-id="f55e2-212">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f55e2-212">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
    "feedback":{"@odata.type":"microsoft.graph.educationFeedback"},
    "grade":{"@odata.type":"microsoft.graph.educationAssignmentGrade"},
    "id":"String (identifier)",
    "recipient":{"@odata.type":"microsoft.graph.educationSubmissionRecipient"},
    "returnedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "returnedDateTime":"String (timestamp)",
    "resourcesFolderUrl":"String",
    "status":"string",
    "submittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "submittedDateTime":"String (timestamp)",
    "unsubmittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "unsubmittedDateTime":"String (timestamp)",
    "releasedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "releasedDateTime":"String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
