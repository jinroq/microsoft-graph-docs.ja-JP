---
title: governanceRoleAssignmentRequest リソースの種類
description: Privilegd Identity Management での役割の割り当て操作の要求を表します。
localization_priority: Normal
ms.openlocfilehash: d5d5f34d417b5d5cbd5eca9bb32ad49c17ef70e5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333687"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="54e54-103">governanceRoleAssignmentRequest リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54e54-103">governanceRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54e54-104">Privilegd Identity Management での役割の割り当て操作の要求を表します。</span><span class="sxs-lookup"><span data-stu-id="54e54-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="54e54-105">`governanceRoleAssignmentRequest`は、役割の割り当てのライフサイクルを管理するために使用される、チケットモデル化されたエンティティです。</span><span class="sxs-lookup"><span data-stu-id="54e54-105">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="54e54-106">ユーザーと管理者の意図または決定を表しており、直接公開`POST`、 `PUT`および`DELETE`操作と比較して、定期的な schduling、承認ゲートなどの実装を可能にする柔軟性も提供します。オン`governanceRoleAssignment`にします。</span><span class="sxs-lookup"><span data-stu-id="54e54-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="54e54-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="54e54-107">Methods</span></span>

| <span data-ttu-id="54e54-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="54e54-108">Method</span></span>          |<span data-ttu-id="54e54-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="54e54-109">Return Type</span></span>  |<span data-ttu-id="54e54-110">説明</span><span class="sxs-lookup"><span data-stu-id="54e54-110">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="54e54-111">取得</span><span class="sxs-lookup"><span data-stu-id="54e54-111">Get</span></span>](../api/governanceroleassignmentrequest-get.md) | [<span data-ttu-id="54e54-112">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="54e54-112">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="54e54-113">ID で指定された役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="54e54-113">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="54e54-114">List</span><span class="sxs-lookup"><span data-stu-id="54e54-114">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="54e54-115">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="54e54-115">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="54e54-116">リソースに対して役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="54e54-116">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="54e54-117">Create</span><span class="sxs-lookup"><span data-stu-id="54e54-117">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="54e54-118">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="54e54-118">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="54e54-119">既存または新しい役割の割り当てのライフサイクルを管理するための要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="54e54-119">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="54e54-120">Cancel</span><span class="sxs-lookup"><span data-stu-id="54e54-120">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="54e54-121">保留中の役割の割り当て要求を取り消します。</span><span class="sxs-lookup"><span data-stu-id="54e54-121">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="54e54-122">更新する</span><span class="sxs-lookup"><span data-stu-id="54e54-122">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="54e54-123">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="54e54-123">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="54e54-124">要求がの`PendingAdminDecision`状態にある場合、管理者は要求に関する決定を更新します。</span><span class="sxs-lookup"><span data-stu-id="54e54-124">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="54e54-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54e54-125">Properties</span></span>
| <span data-ttu-id="54e54-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54e54-126">Property</span></span>                  | <span data-ttu-id="54e54-127">型</span><span class="sxs-lookup"><span data-stu-id="54e54-127">Type</span></span>          |<span data-ttu-id="54e54-128">説明</span><span class="sxs-lookup"><span data-stu-id="54e54-128">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="54e54-129">id</span><span class="sxs-lookup"><span data-stu-id="54e54-129">id</span></span>                         |<span data-ttu-id="54e54-130">String</span><span class="sxs-lookup"><span data-stu-id="54e54-130">String</span></span>         |<span data-ttu-id="54e54-131">役割の割り当て要求の id。</span><span class="sxs-lookup"><span data-stu-id="54e54-131">The id of the role assignment request.</span></span>|
|<span data-ttu-id="54e54-132">resourceId</span><span class="sxs-lookup"><span data-stu-id="54e54-132">resourceId</span></span>                 |<span data-ttu-id="54e54-133">String</span><span class="sxs-lookup"><span data-stu-id="54e54-133">String</span></span>         |<span data-ttu-id="54e54-134">必須。</span><span class="sxs-lookup"><span data-stu-id="54e54-134">Required.</span></span> <span data-ttu-id="54e54-135">役割の割り当て要求が関連付けられているリソースの id。</span><span class="sxs-lookup"><span data-stu-id="54e54-135">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="54e54-136">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="54e54-136">roleDefinitionId</span></span>           |<span data-ttu-id="54e54-137">String</span><span class="sxs-lookup"><span data-stu-id="54e54-137">String</span></span>         |<span data-ttu-id="54e54-138">必須。</span><span class="sxs-lookup"><span data-stu-id="54e54-138">Required.</span></span> <span data-ttu-id="54e54-139">役割の割り当て要求が関連付けられているロール定義の id。</span><span class="sxs-lookup"><span data-stu-id="54e54-139">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="54e54-140">subjectId</span><span class="sxs-lookup"><span data-stu-id="54e54-140">subjectId</span></span>                  |<span data-ttu-id="54e54-141">String</span><span class="sxs-lookup"><span data-stu-id="54e54-141">String</span></span>         |<span data-ttu-id="54e54-142">必須。</span><span class="sxs-lookup"><span data-stu-id="54e54-142">Required.</span></span> <span data-ttu-id="54e54-143">役割の割り当て要求が関連付けられているサブジェクトの id。</span><span class="sxs-lookup"><span data-stu-id="54e54-143">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="54e54-144">type</span><span class="sxs-lookup"><span data-stu-id="54e54-144">type</span></span>                       |<span data-ttu-id="54e54-145">String</span><span class="sxs-lookup"><span data-stu-id="54e54-145">String</span></span>         |<span data-ttu-id="54e54-146">必須。</span><span class="sxs-lookup"><span data-stu-id="54e54-146">Required.</span></span> <span data-ttu-id="54e54-147">役割の割り当てに対する操作の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="54e54-147">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="54e54-148">値には、</span><span class="sxs-lookup"><span data-stu-id="54e54-148">The value can be</span></span> <ul><li><span data-ttu-id="54e54-149">`AdminAdd`: ユーザー/グループを役割に割り当てる。</span><span class="sxs-lookup"><span data-stu-id="54e54-149">`AdminAdd`: Adminstrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="54e54-150">`UserAdd`: ユーザーが適格な割り当てをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="54e54-150">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="54e54-151">`AdminUpdate`: 既存の役割の割り当ての変更を行う</span><span class="sxs-lookup"><span data-stu-id="54e54-151">`AdminUpdate`: Adminstrators change existing role assignments</span></span></li><li><span data-ttu-id="54e54-152">`AdminRemove`: [ユーザーまたはグループを役割から削除する]。</span><span class="sxs-lookup"><span data-stu-id="54e54-152">`AdminRemove`: Adminstrators remove users/groups from roles;</span></span><li><span data-ttu-id="54e54-153">`UserRemove`: ユーザーはアクティブな割り当てを無効にします。</span><span class="sxs-lookup"><span data-stu-id="54e54-153">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="54e54-154">`UserExtend`: ユーザーが期限切れの割り当てを拡張するよう要求します。</span><span class="sxs-lookup"><span data-stu-id="54e54-154">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="54e54-155">`AdminExtend`: 管理者は期限切れの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="54e54-155">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="54e54-156">`UserRenew`: ユーザーは、期限切れの割り当ての更新を要求します。</span><span class="sxs-lookup"><span data-stu-id="54e54-156">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="54e54-157">`AdminRenew`: 管理者は期限切れの割り当てを拡張します。</span><span class="sxs-lookup"><span data-stu-id="54e54-157">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="54e54-158">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="54e54-158">assignmentState</span></span>|<span data-ttu-id="54e54-159">String</span><span class="sxs-lookup"><span data-stu-id="54e54-159">String</span></span>  |<span data-ttu-id="54e54-160">必須。</span><span class="sxs-lookup"><span data-stu-id="54e54-160">Required.</span></span> <span data-ttu-id="54e54-161">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="54e54-161">The state of the assignment.</span></span> <span data-ttu-id="54e54-162">値には、</span><span class="sxs-lookup"><span data-stu-id="54e54-162">The value can be</span></span> <ul><li> <span data-ttu-id="54e54-163">`Eligible`適格な割り当ての場合</span><span class="sxs-lookup"><span data-stu-id="54e54-163">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="54e54-164">`Active`-管理者によって`Active`直接割り当てられている場合、またはユーザーによる資格のある割り当てでアクティブ化されている場合。</span><span class="sxs-lookup"><span data-stu-id="54e54-164">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="54e54-165">requesteddatetime</span><span class="sxs-lookup"><span data-stu-id="54e54-165">requestedDateTime</span></span>          |<span data-ttu-id="54e54-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54e54-166">DateTimeOffset</span></span> |<span data-ttu-id="54e54-167">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="54e54-167">Read-only.</span></span> <span data-ttu-id="54e54-168">要求の作成時刻。</span><span class="sxs-lookup"><span data-stu-id="54e54-168">The request create time.</span></span> <span data-ttu-id="54e54-169">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="54e54-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="54e54-170">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="54e54-170">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="54e54-171">スケジューリング</span><span class="sxs-lookup"><span data-stu-id="54e54-171">schedule</span></span>                   |[<span data-ttu-id="54e54-172">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="54e54-172">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="54e54-173">役割の割り当て要求の schedule オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="54e54-173">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="54e54-174">したがっ</span><span class="sxs-lookup"><span data-stu-id="54e54-174">reason</span></span>                     |<span data-ttu-id="54e54-175">String</span><span class="sxs-lookup"><span data-stu-id="54e54-175">String</span></span>         |<span data-ttu-id="54e54-176">必要な理由についての要求を作成するときに、ユーザーと管理者によって提供されるメッセージ。</span><span class="sxs-lookup"><span data-stu-id="54e54-176">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="54e54-177">status</span><span class="sxs-lookup"><span data-stu-id="54e54-177">status</span></span>                     |[<span data-ttu-id="54e54-178">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="54e54-178">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="54e54-179">役割の割り当て要求の状態。</span><span class="sxs-lookup"><span data-stu-id="54e54-179">The status of the role assignment request.</span></span>|
|<span data-ttu-id="54e54-180">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="54e54-180">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="54e54-181">String</span><span class="sxs-lookup"><span data-stu-id="54e54-181">String</span></span>        |<span data-ttu-id="54e54-182">これが役割のアクティブ化要求である場合は、参照`eligible assignment`されているの id を表します。それ以外の場合、 `null`値はです。</span><span class="sxs-lookup"><span data-stu-id="54e54-182">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |



## <a name="relationships"></a><span data-ttu-id="54e54-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54e54-183">Relationships</span></span>
| <span data-ttu-id="54e54-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54e54-184">Relationship</span></span> | <span data-ttu-id="54e54-185">型</span><span class="sxs-lookup"><span data-stu-id="54e54-185">Type</span></span>                                |<span data-ttu-id="54e54-186">説明</span><span class="sxs-lookup"><span data-stu-id="54e54-186">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="54e54-187">リソース</span><span class="sxs-lookup"><span data-stu-id="54e54-187">resource</span></span>      |[<span data-ttu-id="54e54-188">governanceResource</span><span class="sxs-lookup"><span data-stu-id="54e54-188">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="54e54-189">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54e54-189">Read-only.</span></span> <span data-ttu-id="54e54-190">要求が目的とするリソース。</span><span class="sxs-lookup"><span data-stu-id="54e54-190">The resource that the request aims to.</span></span> |
|<span data-ttu-id="54e54-191">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="54e54-191">roleDefinition</span></span>|[<span data-ttu-id="54e54-192">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="54e54-192">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="54e54-193">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54e54-193">Read-only.</span></span> <span data-ttu-id="54e54-194">要求が目的としているロール定義。</span><span class="sxs-lookup"><span data-stu-id="54e54-194">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="54e54-195">subject</span><span class="sxs-lookup"><span data-stu-id="54e54-195">subject</span></span>       |[<span data-ttu-id="54e54-196">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="54e54-196">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="54e54-197">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54e54-197">Read-only.</span></span> <span data-ttu-id="54e54-198">ユーザー/グループプリンシパル。</span><span class="sxs-lookup"><span data-stu-id="54e54-198">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="54e54-199">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54e54-199">JSON representation</span></span>

<span data-ttu-id="54e54-200">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54e54-200">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "suppressions": []
}
-->
