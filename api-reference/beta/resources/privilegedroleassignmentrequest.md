---
title: privilegedRoleAssignmentRequest リソースの種類
description: Privilegd Id 管理の役割の割り当て操作の要求を表します。
localization_priority: Normal
ms.openlocfilehash: c0e0bbfa76b7ffb4e122d381d45dd4092f0843c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509008"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="988ee-103">privilegedRoleAssignmentRequest リソースの種類</span><span class="sxs-lookup"><span data-stu-id="988ee-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="988ee-104">Privilegd Id 管理の役割の割り当て操作の要求を表します。</span><span class="sxs-lookup"><span data-stu-id="988ee-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="988ee-105">`privilegedRoleAssignmentRequest`チケット モデルのエンティティはロールの割り当てのライフ サイクルを管理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="988ee-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="988ee-106">・繰り返し schduling、承認のゲートを直接公開するのと比較した場合のように実装を有効にする柔軟性も提供してユーザーや管理者などの意図と意思決定を表す`POST`と`LIST`の操作だけでなく`MY`と`Cancel`の機能`governanceRoleAssignment`。</span><span class="sxs-lookup"><span data-stu-id="988ee-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="988ee-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="988ee-107">Methods</span></span>

| <span data-ttu-id="988ee-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="988ee-108">Method</span></span>       | <span data-ttu-id="988ee-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="988ee-109">Return Type</span></span> | <span data-ttu-id="988ee-110">説明</span><span class="sxs-lookup"><span data-stu-id="988ee-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="988ee-111">List</span><span class="sxs-lookup"><span data-stu-id="988ee-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="988ee-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="988ee-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="988ee-113">役割の割り当て要求を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="988ee-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="988ee-114">Create</span><span class="sxs-lookup"><span data-stu-id="988ee-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="988ee-115">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="988ee-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="988ee-116">既存または新しい役割の割り当てのライフ サイクルを管理するために要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="988ee-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="988ee-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="988ee-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="988ee-118">保留中の役割の割り当て要求をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="988ee-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="988ee-119">My</span><span class="sxs-lookup"><span data-stu-id="988ee-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="988ee-120">現在の requstor の役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="988ee-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="988ee-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="988ee-121">Properties</span></span>

| <span data-ttu-id="988ee-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="988ee-122">Property</span></span>     | <span data-ttu-id="988ee-123">型</span><span class="sxs-lookup"><span data-stu-id="988ee-123">Type</span></span>        | <span data-ttu-id="988ee-124">説明</span><span class="sxs-lookup"><span data-stu-id="988ee-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="988ee-125">id</span><span class="sxs-lookup"><span data-stu-id="988ee-125">id</span></span>|<span data-ttu-id="988ee-126">String</span><span class="sxs-lookup"><span data-stu-id="988ee-126">String</span></span>| <span data-ttu-id="988ee-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ee-127">Read-only.</span></span> <span data-ttu-id="988ee-128">役割の割り当て要求の id。</span><span class="sxs-lookup"><span data-stu-id="988ee-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="988ee-129">assignmentState</span><span class="sxs-lookup"><span data-stu-id="988ee-129">assignmentState</span></span>|<span data-ttu-id="988ee-130">String</span><span class="sxs-lookup"><span data-stu-id="988ee-130">String</span></span>| <span data-ttu-id="988ee-131">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="988ee-131">The state of the assignment.</span></span> <span data-ttu-id="988ee-132">値は、`Eligible`対象となる割り当ての`Active`が直接割り当てられている場合 -`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</span><span class="sxs-lookup"><span data-stu-id="988ee-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="988ee-133">duration</span><span class="sxs-lookup"><span data-stu-id="988ee-133">duration</span></span>|<span data-ttu-id="988ee-134">String</span><span class="sxs-lookup"><span data-stu-id="988ee-134">String</span></span>| <span data-ttu-id="988ee-135">役割の割り当ての期間です。</span><span class="sxs-lookup"><span data-stu-id="988ee-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="988ee-136">理由</span><span class="sxs-lookup"><span data-stu-id="988ee-136">reason</span></span>|<span data-ttu-id="988ee-137">String</span><span class="sxs-lookup"><span data-stu-id="988ee-137">String</span></span>| <span data-ttu-id="988ee-138">ロールの割り当ての理由です。</span><span class="sxs-lookup"><span data-stu-id="988ee-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="988ee-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="988ee-139">requestedDateTime</span></span>|<span data-ttu-id="988ee-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="988ee-140">DateTimeOffset</span></span>| <span data-ttu-id="988ee-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ee-141">Read-only.</span></span> <span data-ttu-id="988ee-142">要求は、時間を作成します。</span><span class="sxs-lookup"><span data-stu-id="988ee-142">The request create time.</span></span> <span data-ttu-id="988ee-143">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="988ee-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="988ee-144">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="988ee-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="988ee-145">roleId</span><span class="sxs-lookup"><span data-stu-id="988ee-145">roleId</span></span>|<span data-ttu-id="988ee-146">String</span><span class="sxs-lookup"><span data-stu-id="988ee-146">String</span></span>| <span data-ttu-id="988ee-147">ロールの id です。</span><span class="sxs-lookup"><span data-stu-id="988ee-147">The id of the role.</span></span>|
|<span data-ttu-id="988ee-148">Schedule</span><span class="sxs-lookup"><span data-stu-id="988ee-148">schedule</span></span>|[<span data-ttu-id="988ee-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="988ee-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="988ee-150">役割の割り当て要求のスケジュール オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="988ee-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="988ee-151">status</span><span class="sxs-lookup"><span data-stu-id="988ee-151">status</span></span>|<span data-ttu-id="988ee-152">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="988ee-152">String</span></span>| <span data-ttu-id="988ee-153">役割の割り当て要求の読み取り only.The 状態です。</span><span class="sxs-lookup"><span data-stu-id="988ee-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="988ee-154">値は、 `NotStarted`、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="988ee-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="988ee-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="988ee-155">ticketNumber</span></span>|<span data-ttu-id="988ee-156">String</span><span class="sxs-lookup"><span data-stu-id="988ee-156">String</span></span>| <span data-ttu-id="988ee-157">ロールの割り当てを ticketNumber。</span><span class="sxs-lookup"><span data-stu-id="988ee-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="988ee-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="988ee-158">ticketSystem</span></span>|<span data-ttu-id="988ee-159">String</span><span class="sxs-lookup"><span data-stu-id="988ee-159">String</span></span>| <span data-ttu-id="988ee-160">ロールの割り当てを ticketSystem。</span><span class="sxs-lookup"><span data-stu-id="988ee-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="988ee-161">type</span><span class="sxs-lookup"><span data-stu-id="988ee-161">type</span></span>|<span data-ttu-id="988ee-162">String</span><span class="sxs-lookup"><span data-stu-id="988ee-162">String</span></span>| <span data-ttu-id="988ee-163">表す、ロールの割り当ての操作の種類です。</span><span class="sxs-lookup"><span data-stu-id="988ee-163">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="988ee-164">値は、 `AdminAdd`: 管理者のユーザー ロールを追加します。`UserAdd`: ユーザーは、役割の割り当てを追加します。</span><span class="sxs-lookup"><span data-stu-id="988ee-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="988ee-165">userId</span><span class="sxs-lookup"><span data-stu-id="988ee-165">userId</span></span>|<span data-ttu-id="988ee-166">String</span><span class="sxs-lookup"><span data-stu-id="988ee-166">String</span></span>| <span data-ttu-id="988ee-167">ユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="988ee-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="988ee-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="988ee-168">Relationships</span></span>
| <span data-ttu-id="988ee-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="988ee-169">Relationship</span></span> | <span data-ttu-id="988ee-170">型</span><span class="sxs-lookup"><span data-stu-id="988ee-170">Type</span></span>        | <span data-ttu-id="988ee-171">説明</span><span class="sxs-lookup"><span data-stu-id="988ee-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="988ee-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="988ee-172">roleInfo</span></span>|[<span data-ttu-id="988ee-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="988ee-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="988ee-174">役割の割り当て要求の roleInfo オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="988ee-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="988ee-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="988ee-175">JSON representation</span></span>

<span data-ttu-id="988ee-176">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="988ee-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
