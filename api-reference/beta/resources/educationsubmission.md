---
title: educationSubmission リソースの種類
description: 提出書類は、割り当てによって所有されます。 提出書類は、リソースを表しますが、個人 (またはグループ) および有効にするに割り当て、グレードとフィードバックが返されます。
author: dipakboyed
ms.openlocfilehash: 5535aef4db988e0f4c4417128b5b53bbed884cc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328022"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="2528a-104">educationSubmission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2528a-104">educationSubmission resource type</span></span>

> <span data-ttu-id="2528a-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2528a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2528a-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2528a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2528a-107">提出書類は、割り当てによって所有されます。</span><span class="sxs-lookup"><span data-stu-id="2528a-107">Submissions are owned by an assignment.</span></span> <span data-ttu-id="2528a-108">提出書類は、リソースを表しますが、個人 (またはグループ) および有効にするに割り当て、グレードとフィードバックが返されます。</span><span class="sxs-lookup"><span data-stu-id="2528a-108">A submission represents the resources that an individual (or group) turn in for an assignment and the grade/feedback that is returned.</span></span>
<span data-ttu-id="2528a-109">割り当てを発行する際の提出書類が自動的に作成します。</span><span class="sxs-lookup"><span data-stu-id="2528a-109">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="2528a-110">提出書類は、2 つのリソースのリストを所有しています。</span><span class="sxs-lookup"><span data-stu-id="2528a-110">The submission owns two lists of resources.</span></span> <span data-ttu-id="2528a-111">リソースでは、送信済みのリソースがアクティブになっている受講者がリソースを表すときに、領域を使用するユーザ/グループを表します。</span><span class="sxs-lookup"><span data-stu-id="2528a-111">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="2528a-112">**注:** 状態は読み取り専用およびオブジェクトがアクションを使用してワークフローを移動します。</span><span class="sxs-lookup"><span data-stu-id="2528a-112">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="2528a-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="2528a-113">Methods</span></span>

| <span data-ttu-id="2528a-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="2528a-114">Method</span></span>           | <span data-ttu-id="2528a-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2528a-115">Return Type</span></span>    |<span data-ttu-id="2528a-116">説明</span><span class="sxs-lookup"><span data-stu-id="2528a-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2528a-117">EducationSubmission を取得します。</span><span class="sxs-lookup"><span data-stu-id="2528a-117">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="2528a-118">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="2528a-118">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="2528a-119">**EducationSubmission**オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2528a-119">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="2528a-120">ボックスの一覧のリソース</span><span class="sxs-lookup"><span data-stu-id="2528a-120">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="2528a-121">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2528a-121">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="2528a-122">**EducationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2528a-122">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="2528a-123">リスト submittedResources</span><span class="sxs-lookup"><span data-stu-id="2528a-123">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="2528a-124">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2528a-124">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="2528a-125">**EducationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2528a-125">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="2528a-126">Update</span><span class="sxs-lookup"><span data-stu-id="2528a-126">Update</span></span>](../api/educationsubmission-update.md) | [<span data-ttu-id="2528a-127">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="2528a-127">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="2528a-128">**EducationSubmission**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2528a-128">Update an **educationSubmission** object.</span></span> |
|[<span data-ttu-id="2528a-129">Return</span><span class="sxs-lookup"><span data-stu-id="2528a-129">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="2528a-130">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="2528a-130">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="2528a-131">教師は、生徒に成績とフィードバックを表示できることを示す戻り値を使用します。</span><span class="sxs-lookup"><span data-stu-id="2528a-131">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="2528a-132">Submit</span><span class="sxs-lookup"><span data-stu-id="2528a-132">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="2528a-133">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="2528a-133">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="2528a-134">受講者にするには、割り当ての使用を送信します。</span><span class="sxs-lookup"><span data-stu-id="2528a-134">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="2528a-135">これは、グレーディングの**submittedResources**フォルダーにリソースをコピーし、ステータスを更新します。</span><span class="sxs-lookup"><span data-stu-id="2528a-135">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="2528a-136">Unsubmit</span><span class="sxs-lookup"><span data-stu-id="2528a-136">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="2528a-137">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="2528a-137">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="2528a-138">受講者は、作業から提出された提出書類の状態に移動するのには、unsubmit を使用します。</span><span class="sxs-lookup"><span data-stu-id="2528a-138">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="2528a-139">これは、グレーディングの**workingResources**フォルダーにリソースをコピーし、ステータスを更新します。</span><span class="sxs-lookup"><span data-stu-id="2528a-139">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="2528a-140">Properties</span><span class="sxs-lookup"><span data-stu-id="2528a-140">Properties</span></span>
| <span data-ttu-id="2528a-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2528a-141">Property</span></span>     | <span data-ttu-id="2528a-142">種類</span><span class="sxs-lookup"><span data-stu-id="2528a-142">Type</span></span>   |<span data-ttu-id="2528a-143">説明</span><span class="sxs-lookup"><span data-stu-id="2528a-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2528a-144">feedback</span><span class="sxs-lookup"><span data-stu-id="2528a-144">feedback</span></span>|[<span data-ttu-id="2528a-145">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="2528a-145">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="2528a-146">受講者に、先生のノートを保存する [フィードバック] プロパティを保持します。</span><span class="sxs-lookup"><span data-stu-id="2528a-146">Holds the feedback property which stores the teacher's notes back to students.</span></span>|
|<span data-ttu-id="2528a-147">grade</span><span class="sxs-lookup"><span data-stu-id="2528a-147">grade</span></span>|[<span data-ttu-id="2528a-148">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="2528a-148">educationAssignmentGrade</span></span>](educationassignmentgrade.md)|<span data-ttu-id="2528a-149">教師は、この送信に割り当てられますグレード情報を保持するには。</span><span class="sxs-lookup"><span data-stu-id="2528a-149">Holds the grade information a teacher assigns to this submission.</span></span>|
|<span data-ttu-id="2528a-150">id</span><span class="sxs-lookup"><span data-stu-id="2528a-150">id</span></span>|<span data-ttu-id="2528a-151">String</span><span class="sxs-lookup"><span data-stu-id="2528a-151">String</span></span>| <span data-ttu-id="2528a-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2528a-152">Read-only.</span></span>|
|<span data-ttu-id="2528a-153">受信者</span><span class="sxs-lookup"><span data-stu-id="2528a-153">recipient</span></span>|[<span data-ttu-id="2528a-154">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="2528a-154">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="2528a-155">この提出書類に割り当てられました。</span><span class="sxs-lookup"><span data-stu-id="2528a-155">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="2528a-156">releasedBy</span><span class="sxs-lookup"><span data-stu-id="2528a-156">releasedBy</span></span>|[<span data-ttu-id="2528a-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="2528a-157">identitySet</span></span>](identityset.md)|<span data-ttu-id="2528a-158">リリースには、この送信のステータスを移動したユーザーです。</span><span class="sxs-lookup"><span data-stu-id="2528a-158">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="2528a-159">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="2528a-159">releasedDateTime</span></span>|<span data-ttu-id="2528a-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2528a-160">DateTimeOffset</span></span>|<span data-ttu-id="2528a-161">提出書類がリリースされた時点での瞬間。</span><span class="sxs-lookup"><span data-stu-id="2528a-161">Moment in time when the submission was released.</span></span> <span data-ttu-id="2528a-162">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2528a-162">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2528a-163">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2528a-163">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2528a-164">返す</span><span class="sxs-lookup"><span data-stu-id="2528a-164">returnedBy</span></span>|[<span data-ttu-id="2528a-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="2528a-165">identitySet</span></span>](identityset.md)|<span data-ttu-id="2528a-166">返されるには、この送信のステータスを移動したユーザーです。</span><span class="sxs-lookup"><span data-stu-id="2528a-166">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="2528a-167">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="2528a-167">returnedDateTime</span></span>|<span data-ttu-id="2528a-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2528a-168">DateTimeOffset</span></span>|<span data-ttu-id="2528a-169">提出書類が返された瞬間です。</span><span class="sxs-lookup"><span data-stu-id="2528a-169">Moment in time when the submission was returned.</span></span> <span data-ttu-id="2528a-170">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2528a-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2528a-171">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2528a-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2528a-172">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="2528a-172">resourcesFolderUrl</span></span>|<span data-ttu-id="2528a-173">String</span><span class="sxs-lookup"><span data-stu-id="2528a-173">String</span></span>|<span data-ttu-id="2528a-174">この送信のためのリソースのすべてのファイル、フォルダーを格納する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2528a-174">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="2528a-175">status</span><span class="sxs-lookup"><span data-stu-id="2528a-175">status</span></span>|<span data-ttu-id="2528a-176">string</span><span class="sxs-lookup"><span data-stu-id="2528a-176">string</span></span>| <span data-ttu-id="2528a-177">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2528a-177">Read-Only.</span></span> <span data-ttu-id="2528a-178">使用可能な値: `working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="2528a-178">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="2528a-179">submittedBy</span><span class="sxs-lookup"><span data-stu-id="2528a-179">submittedBy</span></span>|[<span data-ttu-id="2528a-180">identitySet</span><span class="sxs-lookup"><span data-stu-id="2528a-180">identitySet</span></span>](identityset.md)|<span data-ttu-id="2528a-181">送信済みの状態に、リソースを移動したユーザーです。</span><span class="sxs-lookup"><span data-stu-id="2528a-181">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="2528a-182">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="2528a-182">submittedDateTime</span></span>|<span data-ttu-id="2528a-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2528a-183">DateTimeOffset</span></span>|<span data-ttu-id="2528a-184">提出書類を提出済みの状態に移動したときの時点です。</span><span class="sxs-lookup"><span data-stu-id="2528a-184">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="2528a-185">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2528a-185">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2528a-186">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2528a-186">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2528a-187">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="2528a-187">unsubmittedBy</span></span>|[<span data-ttu-id="2528a-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="2528a-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="2528a-189">リソースを移動したユーザーからは、作業の状態に送信します。</span><span class="sxs-lookup"><span data-stu-id="2528a-189">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="2528a-190">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="2528a-190">unsubmittedDateTime</span></span>|<span data-ttu-id="2528a-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2528a-191">DateTimeOffset</span></span>|<span data-ttu-id="2528a-192">移動するとき、提出書類がから送信、正常な状態に瞬間です。</span><span class="sxs-lookup"><span data-stu-id="2528a-192">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="2528a-193">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2528a-193">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2528a-194">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2528a-194">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="2528a-195">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2528a-195">Relationships</span></span>
| <span data-ttu-id="2528a-196">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2528a-196">Relationship</span></span> | <span data-ttu-id="2528a-197">型</span><span class="sxs-lookup"><span data-stu-id="2528a-197">Type</span></span>   |<span data-ttu-id="2528a-198">説明</span><span class="sxs-lookup"><span data-stu-id="2528a-198">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2528a-199">resources</span><span class="sxs-lookup"><span data-stu-id="2528a-199">resources</span></span>|<span data-ttu-id="2528a-200">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2528a-200">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="2528a-201">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2528a-201">Nullable.</span></span>|
|<span data-ttu-id="2528a-202">submittedResources</span><span class="sxs-lookup"><span data-stu-id="2528a-202">submittedResources</span></span>|<span data-ttu-id="2528a-203">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2528a-203">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="2528a-p111">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2528a-p111">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2528a-206">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2528a-206">JSON representation</span></span>

<span data-ttu-id="2528a-207">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2528a-207">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "grade": {"@odata.type": "microsoft.graph.educationAssignmentGrade"},
  "id": "String (identifier)",
  "recipient": {"@odata.type": "microsoft.graph.educationSubmissionRecipient"},
  "returnedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "returnedDateTime": "String (timestamp)",
  "resourcesFolderUrl": "String",
  "status": "string",
  "submittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "submittedDateTime": "String (timestamp)",
  "unsubmittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "unsubmittedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->