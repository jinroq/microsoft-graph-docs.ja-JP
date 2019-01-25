---
title: educationSubmission リソースの種類
description: 提出書類は、割り当てによって所有されます。 提出書類は、リソースを表しますが、個人 (またはグループ) および有効にするに割り当て、グレードとフィードバックが返されます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: aeeb1355da2ffcb0ebf561af2ecd15ac93221e26
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521426"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="30d9e-104">educationSubmission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30d9e-104">educationSubmission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30d9e-105">提出書類は、割り当てによって所有されます。</span><span class="sxs-lookup"><span data-stu-id="30d9e-105">Submissions are owned by an assignment.</span></span> <span data-ttu-id="30d9e-106">提出書類は、リソースを表しますが、個人 (またはグループ) および有効にするに割り当て、グレードとフィードバックが返されます。</span><span class="sxs-lookup"><span data-stu-id="30d9e-106">A submission represents the resources that an individual (or group) turn in for an assignment and the grade/feedback that is returned.</span></span>
<span data-ttu-id="30d9e-107">割り当てを発行する際の提出書類が自動的に作成します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="30d9e-108">提出書類は、2 つのリソースのリストを所有しています。</span><span class="sxs-lookup"><span data-stu-id="30d9e-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="30d9e-109">リソースでは、送信済みのリソースがアクティブになっている受講者がリソースを表すときに、領域を使用するユーザ/グループを表します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="30d9e-110">**注:** 状態は読み取り専用およびオブジェクトがアクションを使用してワークフローを移動します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-110">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="30d9e-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="30d9e-111">Methods</span></span>

| <span data-ttu-id="30d9e-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="30d9e-112">Method</span></span>           | <span data-ttu-id="30d9e-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="30d9e-113">Return Type</span></span>    |<span data-ttu-id="30d9e-114">説明</span><span class="sxs-lookup"><span data-stu-id="30d9e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30d9e-115">EducationSubmission を取得します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-115">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="30d9e-116">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="30d9e-116">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="30d9e-117">**EducationSubmission**オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30d9e-117">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="30d9e-118">ボックスの一覧のリソース</span><span class="sxs-lookup"><span data-stu-id="30d9e-118">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="30d9e-119">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="30d9e-119">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="30d9e-120">**EducationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-120">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="30d9e-121">リスト submittedResources</span><span class="sxs-lookup"><span data-stu-id="30d9e-121">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="30d9e-122">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="30d9e-122">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="30d9e-123">**EducationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-123">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="30d9e-124">Update</span><span class="sxs-lookup"><span data-stu-id="30d9e-124">Update</span></span>](../api/educationsubmission-update.md) | [<span data-ttu-id="30d9e-125">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="30d9e-125">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="30d9e-126">**EducationSubmission**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-126">Update an **educationSubmission** object.</span></span> |
|[<span data-ttu-id="30d9e-127">Return</span><span class="sxs-lookup"><span data-stu-id="30d9e-127">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="30d9e-128">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="30d9e-128">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="30d9e-129">教師は、生徒に成績とフィードバックを表示できることを示す戻り値を使用します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-129">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="30d9e-130">Submit</span><span class="sxs-lookup"><span data-stu-id="30d9e-130">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="30d9e-131">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="30d9e-131">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="30d9e-132">受講者にするには、割り当ての使用を送信します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-132">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="30d9e-133">これは、グレーディングの**submittedResources**フォルダーにリソースをコピーし、ステータスを更新します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-133">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="30d9e-134">Unsubmit</span><span class="sxs-lookup"><span data-stu-id="30d9e-134">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="30d9e-135">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="30d9e-135">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="30d9e-136">受講者は、作業から提出された提出書類の状態に移動するのには、unsubmit を使用します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-136">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="30d9e-137">これは、グレーディングの**workingResources**フォルダーにリソースをコピーし、ステータスを更新します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-137">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="30d9e-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30d9e-138">Properties</span></span>
| <span data-ttu-id="30d9e-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30d9e-139">Property</span></span>     | <span data-ttu-id="30d9e-140">型</span><span class="sxs-lookup"><span data-stu-id="30d9e-140">Type</span></span>   |<span data-ttu-id="30d9e-141">説明</span><span class="sxs-lookup"><span data-stu-id="30d9e-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30d9e-142">feedback</span><span class="sxs-lookup"><span data-stu-id="30d9e-142">feedback</span></span>|[<span data-ttu-id="30d9e-143">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="30d9e-143">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="30d9e-144">受講者に、先生のノートを保存する [フィードバック] プロパティを保持します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-144">Holds the feedback property which stores the teacher's notes back to students.</span></span>|
|<span data-ttu-id="30d9e-145">grade</span><span class="sxs-lookup"><span data-stu-id="30d9e-145">grade</span></span>|[<span data-ttu-id="30d9e-146">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="30d9e-146">educationAssignmentGrade</span></span>](educationassignmentgrade.md)|<span data-ttu-id="30d9e-147">教師は、この送信に割り当てられますグレード情報を保持するには。</span><span class="sxs-lookup"><span data-stu-id="30d9e-147">Holds the grade information a teacher assigns to this submission.</span></span>|
|<span data-ttu-id="30d9e-148">id</span><span class="sxs-lookup"><span data-stu-id="30d9e-148">id</span></span>|<span data-ttu-id="30d9e-149">String</span><span class="sxs-lookup"><span data-stu-id="30d9e-149">String</span></span>| <span data-ttu-id="30d9e-150">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="30d9e-150">Read-only.</span></span>|
|<span data-ttu-id="30d9e-151">Recipient</span><span class="sxs-lookup"><span data-stu-id="30d9e-151">recipient</span></span>|[<span data-ttu-id="30d9e-152">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="30d9e-152">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="30d9e-153">この提出書類に割り当てられました。</span><span class="sxs-lookup"><span data-stu-id="30d9e-153">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="30d9e-154">releasedBy</span><span class="sxs-lookup"><span data-stu-id="30d9e-154">releasedBy</span></span>|[<span data-ttu-id="30d9e-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="30d9e-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="30d9e-156">リリースには、この送信のステータスを移動したユーザーです。</span><span class="sxs-lookup"><span data-stu-id="30d9e-156">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="30d9e-157">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="30d9e-157">releasedDateTime</span></span>|<span data-ttu-id="30d9e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d9e-158">DateTimeOffset</span></span>|<span data-ttu-id="30d9e-159">提出書類がリリースされた時点での瞬間。</span><span class="sxs-lookup"><span data-stu-id="30d9e-159">Moment in time when the submission was released.</span></span> <span data-ttu-id="30d9e-160">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="30d9e-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30d9e-161">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="30d9e-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="30d9e-162">返す</span><span class="sxs-lookup"><span data-stu-id="30d9e-162">returnedBy</span></span>|[<span data-ttu-id="30d9e-163">identitySet</span><span class="sxs-lookup"><span data-stu-id="30d9e-163">identitySet</span></span>](identityset.md)|<span data-ttu-id="30d9e-164">返されるには、この送信のステータスを移動したユーザーです。</span><span class="sxs-lookup"><span data-stu-id="30d9e-164">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="30d9e-165">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="30d9e-165">returnedDateTime</span></span>|<span data-ttu-id="30d9e-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d9e-166">DateTimeOffset</span></span>|<span data-ttu-id="30d9e-167">提出書類が返された瞬間です。</span><span class="sxs-lookup"><span data-stu-id="30d9e-167">Moment in time when the submission was returned.</span></span> <span data-ttu-id="30d9e-168">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="30d9e-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30d9e-169">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="30d9e-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="30d9e-170">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="30d9e-170">resourcesFolderUrl</span></span>|<span data-ttu-id="30d9e-171">String</span><span class="sxs-lookup"><span data-stu-id="30d9e-171">String</span></span>|<span data-ttu-id="30d9e-172">この送信のためのリソースのすべてのファイル、フォルダーを格納する必要があります。</span><span class="sxs-lookup"><span data-stu-id="30d9e-172">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="30d9e-173">status</span><span class="sxs-lookup"><span data-stu-id="30d9e-173">status</span></span>|<span data-ttu-id="30d9e-174">string</span><span class="sxs-lookup"><span data-stu-id="30d9e-174">string</span></span>| <span data-ttu-id="30d9e-175">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="30d9e-175">Read-Only.</span></span> <span data-ttu-id="30d9e-176">使用可能な値: `working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="30d9e-176">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="30d9e-177">submittedBy</span><span class="sxs-lookup"><span data-stu-id="30d9e-177">submittedBy</span></span>|[<span data-ttu-id="30d9e-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="30d9e-178">identitySet</span></span>](identityset.md)|<span data-ttu-id="30d9e-179">送信済みの状態に、リソースを移動したユーザーです。</span><span class="sxs-lookup"><span data-stu-id="30d9e-179">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="30d9e-180">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="30d9e-180">submittedDateTime</span></span>|<span data-ttu-id="30d9e-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d9e-181">DateTimeOffset</span></span>|<span data-ttu-id="30d9e-182">提出書類を提出済みの状態に移動したときの時点です。</span><span class="sxs-lookup"><span data-stu-id="30d9e-182">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="30d9e-183">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="30d9e-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30d9e-184">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="30d9e-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="30d9e-185">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="30d9e-185">unsubmittedBy</span></span>|[<span data-ttu-id="30d9e-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="30d9e-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="30d9e-187">リソースを移動したユーザーからは、作業の状態に送信します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-187">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="30d9e-188">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="30d9e-188">unsubmittedDateTime</span></span>|<span data-ttu-id="30d9e-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d9e-189">DateTimeOffset</span></span>|<span data-ttu-id="30d9e-190">移動するとき、提出書類がから送信、正常な状態に瞬間です。</span><span class="sxs-lookup"><span data-stu-id="30d9e-190">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="30d9e-191">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="30d9e-191">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30d9e-192">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="30d9e-192">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="30d9e-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="30d9e-193">Relationships</span></span>
| <span data-ttu-id="30d9e-194">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="30d9e-194">Relationship</span></span> | <span data-ttu-id="30d9e-195">型</span><span class="sxs-lookup"><span data-stu-id="30d9e-195">Type</span></span>   |<span data-ttu-id="30d9e-196">説明</span><span class="sxs-lookup"><span data-stu-id="30d9e-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30d9e-197">resources</span><span class="sxs-lookup"><span data-stu-id="30d9e-197">resources</span></span>|<span data-ttu-id="30d9e-198">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="30d9e-198">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="30d9e-199">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="30d9e-199">Nullable.</span></span>|
|<span data-ttu-id="30d9e-200">submittedResources</span><span class="sxs-lookup"><span data-stu-id="30d9e-200">submittedResources</span></span>|<span data-ttu-id="30d9e-201">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="30d9e-201">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="30d9e-p110">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="30d9e-p110">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30d9e-204">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30d9e-204">JSON representation</span></span>

<span data-ttu-id="30d9e-205">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="30d9e-205">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
