---
title: educationSubmission リソースの種類
description: 提出物は、割り当てによって所有されます。 提出は、個人 (またはグループ) が割り当てに対して有効になるリソースと、返される成績/フィードバックを表します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39adc3f394d106860406b3dd22bbf9a1c600280f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334129"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="66489-104">educationSubmission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66489-104">educationSubmission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66489-105">提出物は、割り当てによって所有されます。</span><span class="sxs-lookup"><span data-stu-id="66489-105">Submissions are owned by an assignment.</span></span> <span data-ttu-id="66489-106">提出は、個人 (またはグループ) が割り当てに対して有効になるリソースと、返される成績/フィードバックを表します。</span><span class="sxs-lookup"><span data-stu-id="66489-106">A submission represents the resources that an individual (or group) turn in for an assignment and the grade/feedback that is returned.</span></span>
<span data-ttu-id="66489-107">割り当てが発行されると、提出物は自動的に作成されます。</span><span class="sxs-lookup"><span data-stu-id="66489-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="66489-108">送信では、2つのリソースリストが所有されています。</span><span class="sxs-lookup"><span data-stu-id="66489-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="66489-109">リソースは、送信されたリソースが、学生が積極的に有効にしたリソースを表している間、ユーザー/グループの作業領域を表します。</span><span class="sxs-lookup"><span data-stu-id="66489-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="66489-110">**注:** 状態は読み取り専用で、オブジェクトはアクションによってワークフローを通じて移動されます。</span><span class="sxs-lookup"><span data-stu-id="66489-110">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="66489-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="66489-111">Methods</span></span>

| <span data-ttu-id="66489-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="66489-112">Method</span></span>           | <span data-ttu-id="66489-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="66489-113">Return Type</span></span>    |<span data-ttu-id="66489-114">説明</span><span class="sxs-lookup"><span data-stu-id="66489-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66489-115">educationSubmission を取得する</span><span class="sxs-lookup"><span data-stu-id="66489-115">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="66489-116">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="66489-116">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="66489-117">**educationSubmission**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="66489-117">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="66489-118">リソースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="66489-118">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="66489-119">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="66489-119">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="66489-120">**educationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="66489-120">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="66489-121">submittedresources を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="66489-121">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="66489-122">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="66489-122">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="66489-123">**educationSubmissionResource**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="66489-123">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="66489-124">更新する</span><span class="sxs-lookup"><span data-stu-id="66489-124">Update</span></span>](../api/educationsubmission-update.md) | [<span data-ttu-id="66489-125">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="66489-125">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="66489-126">**educationSubmission**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="66489-126">Update an **educationSubmission** object.</span></span> |
|[<span data-ttu-id="66489-127">Return</span><span class="sxs-lookup"><span data-stu-id="66489-127">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="66489-128">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="66489-128">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="66489-129">教師は、return を使用して、成績/フィードバックを学生に表示できることを示します。</span><span class="sxs-lookup"><span data-stu-id="66489-129">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="66489-130">Submit</span><span class="sxs-lookup"><span data-stu-id="66489-130">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="66489-131">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="66489-131">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="66489-132">学生は、submit を使用して割り当てを有効にします。</span><span class="sxs-lookup"><span data-stu-id="66489-132">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="66489-133">これにより、リソースが [対象] の [ **submittedresources** ] フォルダーにコピーされ、状態が更新されます。</span><span class="sxs-lookup"><span data-stu-id="66489-133">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="66489-134">送信取り消し</span><span class="sxs-lookup"><span data-stu-id="66489-134">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="66489-135">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="66489-135">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="66489-136">学生は、未送信を使用して、提出物の状態を送信前から作業に移行します。</span><span class="sxs-lookup"><span data-stu-id="66489-136">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="66489-137">これにより、リソースが**workingResources**フォルダーにコピーされて、状況を更新して更新します。</span><span class="sxs-lookup"><span data-stu-id="66489-137">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="66489-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66489-138">Properties</span></span>
| <span data-ttu-id="66489-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66489-139">Property</span></span>     | <span data-ttu-id="66489-140">型</span><span class="sxs-lookup"><span data-stu-id="66489-140">Type</span></span>   |<span data-ttu-id="66489-141">説明</span><span class="sxs-lookup"><span data-stu-id="66489-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66489-142">feedback</span><span class="sxs-lookup"><span data-stu-id="66489-142">feedback</span></span>|[<span data-ttu-id="66489-143">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="66489-143">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="66489-144">教師のメモを生徒に返すフィードバックプロパティを保持します。</span><span class="sxs-lookup"><span data-stu-id="66489-144">Holds the feedback property which stores the teacher's notes back to students.</span></span>|
|<span data-ttu-id="66489-145">grade</span><span class="sxs-lookup"><span data-stu-id="66489-145">grade</span></span>|[<span data-ttu-id="66489-146">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="66489-146">educationAssignmentGrade</span></span>](educationassignmentgrade.md)|<span data-ttu-id="66489-147">教師がこの送信に割り当てる成績情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="66489-147">Holds the grade information a teacher assigns to this submission.</span></span>|
|<span data-ttu-id="66489-148">id</span><span class="sxs-lookup"><span data-stu-id="66489-148">id</span></span>|<span data-ttu-id="66489-149">String</span><span class="sxs-lookup"><span data-stu-id="66489-149">String</span></span>| <span data-ttu-id="66489-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="66489-150">Read-only.</span></span>|
|<span data-ttu-id="66489-151">受信者</span><span class="sxs-lookup"><span data-stu-id="66489-151">recipient</span></span>|[<span data-ttu-id="66489-152">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="66489-152">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="66489-153">この提出物が割り当てられるユーザー。</span><span class="sxs-lookup"><span data-stu-id="66489-153">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="66489-154">releasedby</span><span class="sxs-lookup"><span data-stu-id="66489-154">releasedBy</span></span>|[<span data-ttu-id="66489-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="66489-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="66489-156">この提出の状態をリリース済みに移動したユーザー。</span><span class="sxs-lookup"><span data-stu-id="66489-156">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="66489-157">releaseddatetime</span><span class="sxs-lookup"><span data-stu-id="66489-157">releasedDateTime</span></span>|<span data-ttu-id="66489-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66489-158">DateTimeOffset</span></span>|<span data-ttu-id="66489-159">提出物がいつリリースされたかを示します。</span><span class="sxs-lookup"><span data-stu-id="66489-159">Moment in time when the submission was released.</span></span> <span data-ttu-id="66489-160">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="66489-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66489-161">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="66489-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="66489-162">returnedBy</span><span class="sxs-lookup"><span data-stu-id="66489-162">returnedBy</span></span>|[<span data-ttu-id="66489-163">identitySet</span><span class="sxs-lookup"><span data-stu-id="66489-163">identitySet</span></span>](identityset.md)|<span data-ttu-id="66489-164">この提出の状態を取得したユーザー。</span><span class="sxs-lookup"><span data-stu-id="66489-164">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="66489-165">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="66489-165">returnedDateTime</span></span>|<span data-ttu-id="66489-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66489-166">DateTimeOffset</span></span>|<span data-ttu-id="66489-167">送信が返された瞬間の時間。</span><span class="sxs-lookup"><span data-stu-id="66489-167">Moment in time when the submission was returned.</span></span> <span data-ttu-id="66489-168">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="66489-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66489-169">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="66489-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="66489-170">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="66489-170">resourcesFolderUrl</span></span>|<span data-ttu-id="66489-171">String</span><span class="sxs-lookup"><span data-stu-id="66489-171">String</span></span>|<span data-ttu-id="66489-172">この送信のすべてのファイルリソースを格納する必要があるフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="66489-172">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="66489-173">status</span><span class="sxs-lookup"><span data-stu-id="66489-173">status</span></span>|<span data-ttu-id="66489-174">string</span><span class="sxs-lookup"><span data-stu-id="66489-174">string</span></span>| <span data-ttu-id="66489-175">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66489-175">Read-Only.</span></span> <span data-ttu-id="66489-176">使用可能な値: `working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="66489-176">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="66489-177">submittedby</span><span class="sxs-lookup"><span data-stu-id="66489-177">submittedBy</span></span>|[<span data-ttu-id="66489-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="66489-178">identitySet</span></span>](identityset.md)|<span data-ttu-id="66489-179">リソースを送信済み状態に移行したユーザー。</span><span class="sxs-lookup"><span data-stu-id="66489-179">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="66489-180">submitteddatetime</span><span class="sxs-lookup"><span data-stu-id="66489-180">submittedDateTime</span></span>|<span data-ttu-id="66489-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66489-181">DateTimeOffset</span></span>|<span data-ttu-id="66489-182">提出された状態に提出された時点の状態。</span><span class="sxs-lookup"><span data-stu-id="66489-182">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="66489-183">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="66489-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66489-184">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="66489-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="66489-185">未提出者</span><span class="sxs-lookup"><span data-stu-id="66489-185">unsubmittedBy</span></span>|[<span data-ttu-id="66489-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="66489-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="66489-187">提出されたリソースを作業中の状態に移行したユーザー。</span><span class="sxs-lookup"><span data-stu-id="66489-187">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="66489-188">非 submitteddatetime</span><span class="sxs-lookup"><span data-stu-id="66489-188">unsubmittedDateTime</span></span>|<span data-ttu-id="66489-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66489-189">DateTimeOffset</span></span>|<span data-ttu-id="66489-190">提出物が送信されてから作業中の状態に移行した時点の状態です。</span><span class="sxs-lookup"><span data-stu-id="66489-190">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="66489-191">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="66489-191">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66489-192">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="66489-192">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="66489-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66489-193">Relationships</span></span>
| <span data-ttu-id="66489-194">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66489-194">Relationship</span></span> | <span data-ttu-id="66489-195">型</span><span class="sxs-lookup"><span data-stu-id="66489-195">Type</span></span>   |<span data-ttu-id="66489-196">説明</span><span class="sxs-lookup"><span data-stu-id="66489-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66489-197">リソース</span><span class="sxs-lookup"><span data-stu-id="66489-197">resources</span></span>|<span data-ttu-id="66489-198">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="66489-198">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="66489-199">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="66489-199">Nullable.</span></span>|
|<span data-ttu-id="66489-200">submittedresources</span><span class="sxs-lookup"><span data-stu-id="66489-200">submittedResources</span></span>|<span data-ttu-id="66489-201">[educationSubmissionResource](educationsubmissionresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="66489-201">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="66489-p110">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="66489-p110">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66489-204">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66489-204">JSON representation</span></span>

<span data-ttu-id="66489-205">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66489-205">The following is a JSON representation of the resource.</span></span>

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
