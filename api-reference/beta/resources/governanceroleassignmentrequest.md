---
title: governanceRoleAssignmentRequest リソースの種類
description: Privilegd Id 管理の役割の割り当て操作の要求を表します。
localization_priority: Normal
ms.openlocfilehash: 242f1d311a2d304d0d8dab0a4e24f9294722ab6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509575"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="03686-103">governanceRoleAssignmentRequest リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03686-103">governanceRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03686-104">Privilegd Id 管理の役割の割り当て操作の要求を表します。</span><span class="sxs-lookup"><span data-stu-id="03686-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="03686-105">`governanceRoleAssignmentRequest`チケット モデルのエンティティはロールの割り当てのライフ サイクルを管理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="03686-105">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="03686-106">・繰り返し schduling、承認のゲートを直接公開するのと比較した場合のように実装を有効にする柔軟性も提供してユーザーや管理者などの意図と意思決定を表す`POST`、 `PUT`、および`DELETE`の操作`governanceRoleAssignment`。</span><span class="sxs-lookup"><span data-stu-id="03686-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="03686-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="03686-107">Methods</span></span>

| <span data-ttu-id="03686-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="03686-108">Method</span></span>          |<span data-ttu-id="03686-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="03686-109">Return Type</span></span>  |<span data-ttu-id="03686-110">説明</span><span class="sxs-lookup"><span data-stu-id="03686-110">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="03686-111">Get</span><span class="sxs-lookup"><span data-stu-id="03686-111">Get</span></span>](../api/governanceroleassignmentrequest-get.md) | [<span data-ttu-id="03686-112">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="03686-112">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="03686-113">ID で指定されたロールの割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="03686-113">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="03686-114">List</span><span class="sxs-lookup"><span data-stu-id="03686-114">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="03686-115">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="03686-115">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="03686-116">リソースの役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="03686-116">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="03686-117">Create</span><span class="sxs-lookup"><span data-stu-id="03686-117">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="03686-118">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="03686-118">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="03686-119">既存または新しい役割の割り当てのライフ サイクルを管理するために要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="03686-119">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="03686-120">Cancel</span><span class="sxs-lookup"><span data-stu-id="03686-120">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="03686-121">保留中の役割の割り当て要求をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="03686-121">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="03686-122">Update</span><span class="sxs-lookup"><span data-stu-id="03686-122">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="03686-123">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="03686-123">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="03686-124">管理者は、要求の状態の場合に要求の決定を更新`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="03686-124">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="03686-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03686-125">Properties</span></span>
| <span data-ttu-id="03686-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03686-126">Property</span></span>                  | <span data-ttu-id="03686-127">型</span><span class="sxs-lookup"><span data-stu-id="03686-127">Type</span></span>          |<span data-ttu-id="03686-128">説明</span><span class="sxs-lookup"><span data-stu-id="03686-128">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="03686-129">id</span><span class="sxs-lookup"><span data-stu-id="03686-129">id</span></span>                         |<span data-ttu-id="03686-130">String</span><span class="sxs-lookup"><span data-stu-id="03686-130">String</span></span>         |<span data-ttu-id="03686-131">役割の割り当て要求の id。</span><span class="sxs-lookup"><span data-stu-id="03686-131">The id of the role assignment request.</span></span>|
|<span data-ttu-id="03686-132">resourceId</span><span class="sxs-lookup"><span data-stu-id="03686-132">resourceId</span></span>                 |<span data-ttu-id="03686-133">String</span><span class="sxs-lookup"><span data-stu-id="03686-133">String</span></span>         |<span data-ttu-id="03686-134">必須。</span><span class="sxs-lookup"><span data-stu-id="03686-134">Required.</span></span> <span data-ttu-id="03686-135">役割の割り当て要求に関連付けられているリソースの id です。</span><span class="sxs-lookup"><span data-stu-id="03686-135">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="03686-136">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="03686-136">roleDefinitionId</span></span>           |<span data-ttu-id="03686-137">String</span><span class="sxs-lookup"><span data-stu-id="03686-137">String</span></span>         |<span data-ttu-id="03686-138">必須。</span><span class="sxs-lookup"><span data-stu-id="03686-138">Required.</span></span> <span data-ttu-id="03686-139">役割の割り当て要求に関連付けられている役割の定義の id です。</span><span class="sxs-lookup"><span data-stu-id="03686-139">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="03686-140">subjectId</span><span class="sxs-lookup"><span data-stu-id="03686-140">subjectId</span></span>                  |<span data-ttu-id="03686-141">String</span><span class="sxs-lookup"><span data-stu-id="03686-141">String</span></span>         |<span data-ttu-id="03686-142">必須。</span><span class="sxs-lookup"><span data-stu-id="03686-142">Required.</span></span> <span data-ttu-id="03686-143">役割の割り当て要求に関連付けられているサブジェクトの id です。</span><span class="sxs-lookup"><span data-stu-id="03686-143">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="03686-144">type</span><span class="sxs-lookup"><span data-stu-id="03686-144">type</span></span>                       |<span data-ttu-id="03686-145">String</span><span class="sxs-lookup"><span data-stu-id="03686-145">String</span></span>         |<span data-ttu-id="03686-146">必須。</span><span class="sxs-lookup"><span data-stu-id="03686-146">Required.</span></span> <span data-ttu-id="03686-147">表す、ロールの割り当ての操作の種類です。</span><span class="sxs-lookup"><span data-stu-id="03686-147">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="03686-148">値は、します。</span><span class="sxs-lookup"><span data-stu-id="03686-148">The value can be</span></span> <ul><li><span data-ttu-id="03686-149">`AdminAdd`: 管理者の役割にユーザーまたはグループを割り当てる</span><span class="sxs-lookup"><span data-stu-id="03686-149">`AdminAdd`: Adminstrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="03686-150">`UserAdd`: ユーザーが対象の割り当てを有効化します。</span><span class="sxs-lookup"><span data-stu-id="03686-150">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="03686-151">`AdminUpdate`: 管理者は、既存のロールの割り当てを変更します。</span><span class="sxs-lookup"><span data-stu-id="03686-151">`AdminUpdate`: Adminstrators change existing role assignments</span></span></li><li><span data-ttu-id="03686-152">`AdminRemove`: 管理者の役割からユーザーまたはグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="03686-152">`AdminRemove`: Adminstrators remove users/groups from roles;</span></span><li><span data-ttu-id="03686-153">`UserRemove`: ユーザーは、作業中の割り当てを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="03686-153">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="03686-154">`UserExtend`: ユーザーが、有効期限切れの割り当てを拡張する要求します。</span><span class="sxs-lookup"><span data-stu-id="03686-154">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="03686-155">`AdminExtend`: 管理者は、期限切れの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="03686-155">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="03686-156">`UserRenew`: ユーザーの要求が期限切れの割り当てを更新するには</span><span class="sxs-lookup"><span data-stu-id="03686-156">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="03686-157">`AdminRenew`: 管理者は、期限切れの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="03686-157">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="03686-158">assignmentState</span><span class="sxs-lookup"><span data-stu-id="03686-158">assignmentState</span></span>|<span data-ttu-id="03686-159">String</span><span class="sxs-lookup"><span data-stu-id="03686-159">String</span></span>  |<span data-ttu-id="03686-160">必須。</span><span class="sxs-lookup"><span data-stu-id="03686-160">Required.</span></span> <span data-ttu-id="03686-161">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="03686-161">The state of the assignment.</span></span> <span data-ttu-id="03686-162">値は、します。</span><span class="sxs-lookup"><span data-stu-id="03686-162">The value can be</span></span> <ul><li> <span data-ttu-id="03686-163">`Eligible`対象となる割り当ての</span><span class="sxs-lookup"><span data-stu-id="03686-163">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="03686-164">`Active`-直接割り当てられている場合`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</span><span class="sxs-lookup"><span data-stu-id="03686-164">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="03686-165">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="03686-165">requestedDateTime</span></span>          |<span data-ttu-id="03686-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03686-166">DateTimeOffset</span></span> |<span data-ttu-id="03686-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="03686-167">Read-only.</span></span> <span data-ttu-id="03686-168">要求は、時間を作成します。</span><span class="sxs-lookup"><span data-stu-id="03686-168">The request create time.</span></span> <span data-ttu-id="03686-169">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="03686-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03686-170">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="03686-170">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="03686-171">Schedule</span><span class="sxs-lookup"><span data-stu-id="03686-171">schedule</span></span>                   |[<span data-ttu-id="03686-172">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="03686-172">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="03686-173">役割の割り当て要求のスケジュール オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="03686-173">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="03686-174">理由</span><span class="sxs-lookup"><span data-stu-id="03686-174">reason</span></span>                     |<span data-ttu-id="03686-175">String</span><span class="sxs-lookup"><span data-stu-id="03686-175">String</span></span>         |<span data-ttu-id="03686-176">ユーザーおよび管理者によって提供されるメッセージが必要な理由についての要求を作成するとします。</span><span class="sxs-lookup"><span data-stu-id="03686-176">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="03686-177">status</span><span class="sxs-lookup"><span data-stu-id="03686-177">status</span></span>                     |[<span data-ttu-id="03686-178">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="03686-178">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="03686-179">役割の割り当て要求のステータス。</span><span class="sxs-lookup"><span data-stu-id="03686-179">The status of the role assignment request.</span></span>|
|<span data-ttu-id="03686-180">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="03686-180">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="03686-181">String</span><span class="sxs-lookup"><span data-stu-id="03686-181">String</span></span>        |<span data-ttu-id="03686-182">Id を表すロールのアクティブ化の要求の場合は、`eligible assignment`で参照されます。値は、それ以外の場合、 `null`。</span><span class="sxs-lookup"><span data-stu-id="03686-182">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |



## <a name="relationships"></a><span data-ttu-id="03686-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="03686-183">Relationships</span></span>
| <span data-ttu-id="03686-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="03686-184">Relationship</span></span> | <span data-ttu-id="03686-185">型</span><span class="sxs-lookup"><span data-stu-id="03686-185">Type</span></span>                                |<span data-ttu-id="03686-186">説明</span><span class="sxs-lookup"><span data-stu-id="03686-186">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="03686-187">リソース</span><span class="sxs-lookup"><span data-stu-id="03686-187">resource</span></span>      |[<span data-ttu-id="03686-188">governanceResource</span><span class="sxs-lookup"><span data-stu-id="03686-188">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="03686-189">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="03686-189">Read-only.</span></span> <span data-ttu-id="03686-190">要求することを目的とするリソースです。</span><span class="sxs-lookup"><span data-stu-id="03686-190">The resource that the request aims to.</span></span> |
|<span data-ttu-id="03686-191">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="03686-191">roleDefinition</span></span>|[<span data-ttu-id="03686-192">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="03686-192">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="03686-193">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="03686-193">Read-only.</span></span> <span data-ttu-id="03686-194">役割の定義を要求することを目的とします。</span><span class="sxs-lookup"><span data-stu-id="03686-194">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="03686-195">subject</span><span class="sxs-lookup"><span data-stu-id="03686-195">subject</span></span>       |[<span data-ttu-id="03686-196">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="03686-196">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="03686-197">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="03686-197">Read-only.</span></span> <span data-ttu-id="03686-198">ユーザ/グループのプリンシパルです。</span><span class="sxs-lookup"><span data-stu-id="03686-198">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="03686-199">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03686-199">JSON representation</span></span>

<span data-ttu-id="03686-200">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="03686-200">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "type": "String",
  "assignmentState": "String",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
