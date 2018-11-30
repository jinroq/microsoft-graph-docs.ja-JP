---
title: privilegedRoleAssignmentRequest リソースの種類
description: Privilegd Id 管理の役割の割り当て操作の要求を表します。
ms.openlocfilehash: b715c88157a7df52dabcb4c746dfe70bc2523d18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072922"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="8e364-103">privilegedRoleAssignmentRequest リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8e364-103">privilegedRoleAssignmentRequest resource type</span></span>

> <span data-ttu-id="8e364-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8e364-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e364-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e364-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e364-106">Privilegd Id 管理の役割の割り当て操作の要求を表します。</span><span class="sxs-lookup"><span data-stu-id="8e364-106">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="8e364-107">`privilegedRoleAssignmentRequest`チケット モデルのエンティティはロールの割り当てのライフ サイクルを管理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="8e364-107">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="8e364-108">・繰り返し schduling、承認のゲートを直接公開するのと比較した場合のように実装を有効にする柔軟性も提供してユーザーや管理者などの意図と意思決定を表す`POST`と`LIST`の操作だけでなく`MY`と`Cancel`の機能`governanceRoleAssignment`。</span><span class="sxs-lookup"><span data-stu-id="8e364-108">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="8e364-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8e364-109">Methods</span></span>

| <span data-ttu-id="8e364-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="8e364-110">Method</span></span>       | <span data-ttu-id="8e364-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8e364-111">Return Type</span></span> | <span data-ttu-id="8e364-112">説明</span><span class="sxs-lookup"><span data-stu-id="8e364-112">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="8e364-113">List</span><span class="sxs-lookup"><span data-stu-id="8e364-113">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="8e364-114">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8e364-114">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="8e364-115">役割の割り当て要求を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8e364-115">List role assignment requests.</span></span>|
|[<span data-ttu-id="8e364-116">作成</span><span class="sxs-lookup"><span data-stu-id="8e364-116">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="8e364-117">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="8e364-117">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="8e364-118">既存または新しい役割の割り当てのライフ サイクルを管理するために要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="8e364-118">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="8e364-119">キャンセル</span><span class="sxs-lookup"><span data-stu-id="8e364-119">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="8e364-120">保留中の役割の割り当て要求をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="8e364-120">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="8e364-121">My</span><span class="sxs-lookup"><span data-stu-id="8e364-121">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="8e364-122">現在の requstor の役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="8e364-122">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e364-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e364-123">Properties</span></span>

| <span data-ttu-id="8e364-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e364-124">Property</span></span>     | <span data-ttu-id="8e364-125">型</span><span class="sxs-lookup"><span data-stu-id="8e364-125">Type</span></span>        | <span data-ttu-id="8e364-126">説明</span><span class="sxs-lookup"><span data-stu-id="8e364-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e364-127">id</span><span class="sxs-lookup"><span data-stu-id="8e364-127">id</span></span>|<span data-ttu-id="8e364-128">String</span><span class="sxs-lookup"><span data-stu-id="8e364-128">String</span></span>| <span data-ttu-id="8e364-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8e364-129">Read-only.</span></span> <span data-ttu-id="8e364-130">役割の割り当て要求の id。</span><span class="sxs-lookup"><span data-stu-id="8e364-130">The id of the role assignment request.</span></span>|
|<span data-ttu-id="8e364-131">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8e364-131">assignmentState</span></span>|<span data-ttu-id="8e364-132">String</span><span class="sxs-lookup"><span data-stu-id="8e364-132">String</span></span>| <span data-ttu-id="8e364-133">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="8e364-133">The state of the assignment.</span></span> <span data-ttu-id="8e364-134">値は、`Eligible`対象となる割り当ての`Active`が直接割り当てられている場合 -`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</span><span class="sxs-lookup"><span data-stu-id="8e364-134">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="8e364-135">duration</span><span class="sxs-lookup"><span data-stu-id="8e364-135">duration</span></span>|<span data-ttu-id="8e364-136">String</span><span class="sxs-lookup"><span data-stu-id="8e364-136">String</span></span>| <span data-ttu-id="8e364-137">役割の割り当ての期間です。</span><span class="sxs-lookup"><span data-stu-id="8e364-137">The duration of a role assignment.</span></span>|
|<span data-ttu-id="8e364-138">理由</span><span class="sxs-lookup"><span data-stu-id="8e364-138">reason</span></span>|<span data-ttu-id="8e364-139">String</span><span class="sxs-lookup"><span data-stu-id="8e364-139">String</span></span>| <span data-ttu-id="8e364-140">ロールの割り当ての理由です。</span><span class="sxs-lookup"><span data-stu-id="8e364-140">The reason for the role assignment.</span></span>|
|<span data-ttu-id="8e364-141">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e364-141">requestedDateTime</span></span>|<span data-ttu-id="8e364-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e364-142">DateTimeOffset</span></span>| <span data-ttu-id="8e364-143">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8e364-143">Read-only.</span></span> <span data-ttu-id="8e364-144">要求は、時間を作成します。</span><span class="sxs-lookup"><span data-stu-id="8e364-144">The request create time.</span></span> <span data-ttu-id="8e364-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="8e364-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8e364-146">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8e364-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8e364-147">roleId</span><span class="sxs-lookup"><span data-stu-id="8e364-147">roleId</span></span>|<span data-ttu-id="8e364-148">String</span><span class="sxs-lookup"><span data-stu-id="8e364-148">String</span></span>| <span data-ttu-id="8e364-149">ロールの id です。</span><span class="sxs-lookup"><span data-stu-id="8e364-149">The id of the role.</span></span>|
|<span data-ttu-id="8e364-150">スケジュール</span><span class="sxs-lookup"><span data-stu-id="8e364-150">schedule</span></span>|[<span data-ttu-id="8e364-151">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8e364-151">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="8e364-152">役割の割り当て要求のスケジュール オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8e364-152">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="8e364-153">status</span><span class="sxs-lookup"><span data-stu-id="8e364-153">status</span></span>|<span data-ttu-id="8e364-154">String</span><span class="sxs-lookup"><span data-stu-id="8e364-154">String</span></span>| <span data-ttu-id="8e364-155">役割の割り当て要求の読み取り only.The 状態です。</span><span class="sxs-lookup"><span data-stu-id="8e364-155">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="8e364-156">値は、 `NotStarted`、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="8e364-156">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="8e364-157">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="8e364-157">ticketNumber</span></span>|<span data-ttu-id="8e364-158">String</span><span class="sxs-lookup"><span data-stu-id="8e364-158">String</span></span>| <span data-ttu-id="8e364-159">ロールの割り当てを ticketNumber。</span><span class="sxs-lookup"><span data-stu-id="8e364-159">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="8e364-160">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="8e364-160">ticketSystem</span></span>|<span data-ttu-id="8e364-161">String</span><span class="sxs-lookup"><span data-stu-id="8e364-161">String</span></span>| <span data-ttu-id="8e364-162">ロールの割り当てを ticketSystem。</span><span class="sxs-lookup"><span data-stu-id="8e364-162">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="8e364-163">type</span><span class="sxs-lookup"><span data-stu-id="8e364-163">type</span></span>|<span data-ttu-id="8e364-164">String</span><span class="sxs-lookup"><span data-stu-id="8e364-164">String</span></span>| <span data-ttu-id="8e364-165">表す、ロールの割り当ての操作の種類です。</span><span class="sxs-lookup"><span data-stu-id="8e364-165">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="8e364-166">値は、 `AdminAdd`: 管理者のユーザー ロールを追加します。`UserAdd`: ユーザーは、役割の割り当てを追加します。</span><span class="sxs-lookup"><span data-stu-id="8e364-166">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="8e364-167">userId</span><span class="sxs-lookup"><span data-stu-id="8e364-167">userId</span></span>|<span data-ttu-id="8e364-168">String</span><span class="sxs-lookup"><span data-stu-id="8e364-168">String</span></span>| <span data-ttu-id="8e364-169">ユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="8e364-169">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e364-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8e364-170">Relationships</span></span>
| <span data-ttu-id="8e364-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8e364-171">Relationship</span></span> | <span data-ttu-id="8e364-172">型</span><span class="sxs-lookup"><span data-stu-id="8e364-172">Type</span></span>        | <span data-ttu-id="8e364-173">説明</span><span class="sxs-lookup"><span data-stu-id="8e364-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e364-174">roleInfo</span><span class="sxs-lookup"><span data-stu-id="8e364-174">roleInfo</span></span>|[<span data-ttu-id="8e364-175">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="8e364-175">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="8e364-176">役割の割り当て要求の roleInfo オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8e364-176">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e364-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8e364-177">JSON representation</span></span>

<span data-ttu-id="8e364-178">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e364-178">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->