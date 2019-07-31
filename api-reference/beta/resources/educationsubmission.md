---
title: educationSubmission リソースの種類
description: 提出物は、割り当てによって所有されます。 提出は、個人 (またはグループ) が割り当てに対して有効になるリソースと、返される成績/フィードバックを表します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 81c194c08ddc5ed8f5acc38ae84a5478bb7e0229
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972524"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="58c17-104">educationSubmission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58c17-104">educationSubmission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58c17-105">提出物は、割り当てによって所有されます。</span><span class="sxs-lookup"><span data-stu-id="58c17-105">Submissions are owned by an assignment.</span></span> <span data-ttu-id="58c17-106">提出は、個人 (またはグループ) が割り当てに対して有効になるリソースと、返される成績/フィードバックを表します。</span><span class="sxs-lookup"><span data-stu-id="58c17-106">A submission represents the resources that an individual (or group) turn in for an assignment and the grade/feedback that is returned.</span></span>
<span data-ttu-id="58c17-107">割り当てが発行されると、提出物は自動的に作成されます。</span><span class="sxs-lookup"><span data-stu-id="58c17-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="58c17-108">送信では、2つのリソースリストが所有されています。</span><span class="sxs-lookup"><span data-stu-id="58c17-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="58c17-109">リソースは、送信されたリソースが、学生が積極的に有効にしたリソースを表している間、ユーザー/グループの作業領域を表します。</span><span class="sxs-lookup"><span data-stu-id="58c17-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="58c17-110">**注:** 状態は読み取り専用で、オブジェクトはアクションによってワークフローを通じて移動されます。</span><span class="sxs-lookup"><span data-stu-id="58c17-110">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="58c17-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="58c17-111">Methods</span></span>

| <span data-ttu-id="58c17-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="58c17-112">Method</span></span>           | <span data-ttu-id="58c17-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="58c17-113">Return Type</span></span>    |<span data-ttu-id="58c17-114">説明</span><span class="sxs-lookup"><span data-stu-id="58c17-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58c17-115">EducationSubmission を取得する</span><span class="sxs-lookup"><span data-stu-id="58c17-115">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="58c17-116">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="58c17-116">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="58c17-117">**EducationSubmission**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="58c17-117">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="58c17-118">リソースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="58c17-118">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="58c17-119">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58c17-119">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="58c17-120">**EducationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="58c17-120">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="58c17-121">SubmittedResources を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="58c17-121">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="58c17-122">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58c17-122">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="58c17-123">**EducationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="58c17-123">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="58c17-124">Update</span><span class="sxs-lookup"><span data-stu-id="58c17-124">Update</span></span>](../api/educationsubmission-update.md) | [<span data-ttu-id="58c17-125">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="58c17-125">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="58c17-126">**EducationSubmission**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="58c17-126">Update an **educationSubmission** object.</span></span> |
|[<span data-ttu-id="58c17-127">Return</span><span class="sxs-lookup"><span data-stu-id="58c17-127">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="58c17-128">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="58c17-128">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="58c17-129">教師は、return を使用して、成績/フィードバックを学生に表示できることを示します。</span><span class="sxs-lookup"><span data-stu-id="58c17-129">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="58c17-130">Submit</span><span class="sxs-lookup"><span data-stu-id="58c17-130">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="58c17-131">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="58c17-131">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="58c17-132">学生は、submit を使用して割り当てを有効にします。</span><span class="sxs-lookup"><span data-stu-id="58c17-132">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="58c17-133">これにより、リソースが [対象] の [ **Submittedresources** ] フォルダーにコピーされ、状態が更新されます。</span><span class="sxs-lookup"><span data-stu-id="58c17-133">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="58c17-134">送信取り消し</span><span class="sxs-lookup"><span data-stu-id="58c17-134">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="58c17-135">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="58c17-135">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="58c17-136">学生は、未送信を使用して、提出物の状態を送信前から作業に移行します。</span><span class="sxs-lookup"><span data-stu-id="58c17-136">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="58c17-137">これにより、リソースが**workingResources**フォルダーにコピーされて、状況を更新して更新します。</span><span class="sxs-lookup"><span data-stu-id="58c17-137">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="58c17-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58c17-138">Properties</span></span>
| <span data-ttu-id="58c17-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58c17-139">Property</span></span>     | <span data-ttu-id="58c17-140">型</span><span class="sxs-lookup"><span data-stu-id="58c17-140">Type</span></span>   |<span data-ttu-id="58c17-141">説明</span><span class="sxs-lookup"><span data-stu-id="58c17-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58c17-142">feedback</span><span class="sxs-lookup"><span data-stu-id="58c17-142">feedback</span></span>|[<span data-ttu-id="58c17-143">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="58c17-143">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="58c17-144">教師のメモを生徒に返すフィードバックプロパティを保持します。</span><span class="sxs-lookup"><span data-stu-id="58c17-144">Holds the feedback property which stores the teacher's notes back to students.</span></span>|
|<span data-ttu-id="58c17-145">grade</span><span class="sxs-lookup"><span data-stu-id="58c17-145">grade</span></span>|[<span data-ttu-id="58c17-146">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="58c17-146">educationAssignmentGrade</span></span>](educationassignmentgrade.md)|<span data-ttu-id="58c17-147">教師がこの送信に割り当てる成績情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="58c17-147">Holds the grade information a teacher assigns to this submission.</span></span>|
|<span data-ttu-id="58c17-148">id</span><span class="sxs-lookup"><span data-stu-id="58c17-148">id</span></span>|<span data-ttu-id="58c17-149">String</span><span class="sxs-lookup"><span data-stu-id="58c17-149">String</span></span>| <span data-ttu-id="58c17-150">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="58c17-150">Read-only.</span></span>|
|<span data-ttu-id="58c17-151">受信者</span><span class="sxs-lookup"><span data-stu-id="58c17-151">recipient</span></span>|[<span data-ttu-id="58c17-152">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="58c17-152">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="58c17-153">この提出物が割り当てられるユーザー。</span><span class="sxs-lookup"><span data-stu-id="58c17-153">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="58c17-154">releasedBy</span><span class="sxs-lookup"><span data-stu-id="58c17-154">releasedBy</span></span>|[<span data-ttu-id="58c17-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="58c17-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="58c17-156">この提出の状態をリリース済みに移動したユーザー。</span><span class="sxs-lookup"><span data-stu-id="58c17-156">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="58c17-157">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="58c17-157">releasedDateTime</span></span>|<span data-ttu-id="58c17-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58c17-158">DateTimeOffset</span></span>|<span data-ttu-id="58c17-159">提出物がいつリリースされたかを示します。</span><span class="sxs-lookup"><span data-stu-id="58c17-159">Moment in time when the submission was released.</span></span> <span data-ttu-id="58c17-160">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="58c17-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="58c17-161">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58c17-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="58c17-162">returnedBy</span><span class="sxs-lookup"><span data-stu-id="58c17-162">returnedBy</span></span>|[<span data-ttu-id="58c17-163">identitySet</span><span class="sxs-lookup"><span data-stu-id="58c17-163">identitySet</span></span>](identityset.md)|<span data-ttu-id="58c17-164">この提出の状態を取得したユーザー。</span><span class="sxs-lookup"><span data-stu-id="58c17-164">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="58c17-165">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="58c17-165">returnedDateTime</span></span>|<span data-ttu-id="58c17-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58c17-166">DateTimeOffset</span></span>|<span data-ttu-id="58c17-167">送信が返された瞬間の時間。</span><span class="sxs-lookup"><span data-stu-id="58c17-167">Moment in time when the submission was returned.</span></span> <span data-ttu-id="58c17-168">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="58c17-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="58c17-169">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58c17-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="58c17-170">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="58c17-170">resourcesFolderUrl</span></span>|<span data-ttu-id="58c17-171">String</span><span class="sxs-lookup"><span data-stu-id="58c17-171">String</span></span>|<span data-ttu-id="58c17-172">この送信のすべてのファイルリソースを格納する必要があるフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="58c17-172">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="58c17-173">status</span><span class="sxs-lookup"><span data-stu-id="58c17-173">status</span></span>|<span data-ttu-id="58c17-174">string</span><span class="sxs-lookup"><span data-stu-id="58c17-174">string</span></span>| <span data-ttu-id="58c17-175">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="58c17-175">Read-Only.</span></span> <span data-ttu-id="58c17-176">使用可能な値: `working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="58c17-176">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="58c17-177">submittedBy</span><span class="sxs-lookup"><span data-stu-id="58c17-177">submittedBy</span></span>|[<span data-ttu-id="58c17-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="58c17-178">identitySet</span></span>](identityset.md)|<span data-ttu-id="58c17-179">リソースを送信済み状態に移行したユーザー。</span><span class="sxs-lookup"><span data-stu-id="58c17-179">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="58c17-180">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="58c17-180">submittedDateTime</span></span>|<span data-ttu-id="58c17-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58c17-181">DateTimeOffset</span></span>|<span data-ttu-id="58c17-182">提出された状態に提出された時点の状態。</span><span class="sxs-lookup"><span data-stu-id="58c17-182">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="58c17-183">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="58c17-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="58c17-184">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58c17-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="58c17-185">未提出者</span><span class="sxs-lookup"><span data-stu-id="58c17-185">unsubmittedBy</span></span>|[<span data-ttu-id="58c17-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="58c17-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="58c17-187">提出されたリソースを作業中の状態に移行したユーザー。</span><span class="sxs-lookup"><span data-stu-id="58c17-187">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="58c17-188">非 Submitteddatetime</span><span class="sxs-lookup"><span data-stu-id="58c17-188">unsubmittedDateTime</span></span>|<span data-ttu-id="58c17-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58c17-189">DateTimeOffset</span></span>|<span data-ttu-id="58c17-190">提出物が送信されてから作業中の状態に移行した時点の状態です。</span><span class="sxs-lookup"><span data-stu-id="58c17-190">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="58c17-191">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="58c17-191">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="58c17-192">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58c17-192">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="58c17-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58c17-193">Relationships</span></span>
| <span data-ttu-id="58c17-194">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58c17-194">Relationship</span></span> | <span data-ttu-id="58c17-195">型</span><span class="sxs-lookup"><span data-stu-id="58c17-195">Type</span></span>   |<span data-ttu-id="58c17-196">説明</span><span class="sxs-lookup"><span data-stu-id="58c17-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58c17-197">リソース</span><span class="sxs-lookup"><span data-stu-id="58c17-197">resources</span></span>|<span data-ttu-id="58c17-198">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58c17-198">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="58c17-199">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="58c17-199">Nullable.</span></span>|
|<span data-ttu-id="58c17-200">submittedResources</span><span class="sxs-lookup"><span data-stu-id="58c17-200">submittedResources</span></span>|<span data-ttu-id="58c17-201">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58c17-201">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="58c17-p110">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="58c17-p110">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58c17-204">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58c17-204">JSON representation</span></span>

<span data-ttu-id="58c17-205">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58c17-205">The following is a JSON representation of the resource.</span></span>

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
