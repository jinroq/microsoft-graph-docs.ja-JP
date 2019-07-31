---
title: privilegedRoleAssignmentRequest リソースの種類
description: Privilegd Identity Management での役割の割り当て操作の要求を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 881f5e47d7a441a297c21a0463e49496aeaf7a07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965734"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="8dbb7-103">privilegedRoleAssignmentRequest リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8dbb7-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dbb7-104">Privilegd Identity Management での役割の割り当て操作の要求を表します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="8dbb7-105">`privilegedRoleAssignmentRequest`は、役割の割り当てのライフサイクルを管理するために使用される、チケットモデル化されたエンティティです。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="8dbb7-106">これは、ユーザーと管理者の意図または決定を表し、さらに、定期的な schduling の実装、承認ゲートの実装を可能にする柔軟性を備えて`POST`い`LIST`ます。また、直接の公開と操作に加えて、`MY`と`Cancel`の機能`governanceRoleAssignment`をオンにします。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="8dbb7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8dbb7-107">Methods</span></span>

| <span data-ttu-id="8dbb7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8dbb7-108">Method</span></span>       | <span data-ttu-id="8dbb7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8dbb7-109">Return Type</span></span> | <span data-ttu-id="8dbb7-110">説明</span><span class="sxs-lookup"><span data-stu-id="8dbb7-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="8dbb7-111">List</span><span class="sxs-lookup"><span data-stu-id="8dbb7-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="8dbb7-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8dbb7-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="8dbb7-113">役割の割り当て要求を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="8dbb7-114">Create</span><span class="sxs-lookup"><span data-stu-id="8dbb7-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="8dbb7-115">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="8dbb7-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="8dbb7-116">既存または新しい役割の割り当てのライフサイクルを管理するための要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="8dbb7-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="8dbb7-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="8dbb7-118">保留中の役割の割り当て要求を取り消します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="8dbb7-119">My</span><span class="sxs-lookup"><span data-stu-id="8dbb7-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="8dbb7-120">現在の requstor に対する役割の割り当て要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="8dbb7-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8dbb7-121">Properties</span></span>

| <span data-ttu-id="8dbb7-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8dbb7-122">Property</span></span>     | <span data-ttu-id="8dbb7-123">型</span><span class="sxs-lookup"><span data-stu-id="8dbb7-123">Type</span></span>        | <span data-ttu-id="8dbb7-124">説明</span><span class="sxs-lookup"><span data-stu-id="8dbb7-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8dbb7-125">id</span><span class="sxs-lookup"><span data-stu-id="8dbb7-125">id</span></span>|<span data-ttu-id="8dbb7-126">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-126">String</span></span>| <span data-ttu-id="8dbb7-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-127">Read-only.</span></span> <span data-ttu-id="8dbb7-128">役割の割り当て要求の id。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="8dbb7-129">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="8dbb7-129">assignmentState</span></span>|<span data-ttu-id="8dbb7-130">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-130">String</span></span>| <span data-ttu-id="8dbb7-131">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-131">The state of the assignment.</span></span> <span data-ttu-id="8dbb7-132">この値は、 `Eligible`管理者に`Active`よって直接割り当てら`Active`れている場合、またはユーザーによる資格のある割り当てに対してアクティブ化されている場合に、対象となる割り当てに使用できます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="8dbb7-133">duration</span><span class="sxs-lookup"><span data-stu-id="8dbb7-133">duration</span></span>|<span data-ttu-id="8dbb7-134">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-134">String</span></span>| <span data-ttu-id="8dbb7-135">役割の割り当ての期間。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="8dbb7-136">したがっ</span><span class="sxs-lookup"><span data-stu-id="8dbb7-136">reason</span></span>|<span data-ttu-id="8dbb7-137">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-137">String</span></span>| <span data-ttu-id="8dbb7-138">役割の割り当ての理由。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="8dbb7-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbb7-139">requestedDateTime</span></span>|<span data-ttu-id="8dbb7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbb7-140">DateTimeOffset</span></span>| <span data-ttu-id="8dbb7-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-141">Read-only.</span></span> <span data-ttu-id="8dbb7-142">要求の作成時刻。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-142">The request create time.</span></span> <span data-ttu-id="8dbb7-143">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8dbb7-144">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8dbb7-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8dbb7-145">roleId</span><span class="sxs-lookup"><span data-stu-id="8dbb7-145">roleId</span></span>|<span data-ttu-id="8dbb7-146">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-146">String</span></span>| <span data-ttu-id="8dbb7-147">ロールの id。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-147">The id of the role.</span></span>|
|<span data-ttu-id="8dbb7-148">schedule</span><span class="sxs-lookup"><span data-stu-id="8dbb7-148">schedule</span></span>|[<span data-ttu-id="8dbb7-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8dbb7-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="8dbb7-150">役割の割り当て要求の schedule オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="8dbb7-151">status</span><span class="sxs-lookup"><span data-stu-id="8dbb7-151">status</span></span>|<span data-ttu-id="8dbb7-152">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8dbb7-152">String</span></span>| <span data-ttu-id="8dbb7-153">読み取り専用。役割の割り当て要求の状態。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="8dbb7-154">値`NotStarted``Completed``Revoked``RequestExpired`は、、、、、、、、、、、のようになります。`RequestedApproval``Scheduled``Approved``ApprovalDenied``ApprovalAborted``Cancelling``Cancelled`</span><span class="sxs-lookup"><span data-stu-id="8dbb7-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="8dbb7-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="8dbb7-155">ticketNumber</span></span>|<span data-ttu-id="8dbb7-156">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-156">String</span></span>| <span data-ttu-id="8dbb7-157">役割の割り当ての ticketNumber。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="8dbb7-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="8dbb7-158">ticketSystem</span></span>|<span data-ttu-id="8dbb7-159">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-159">String</span></span>| <span data-ttu-id="8dbb7-160">役割の割り当ての ticketSystem。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="8dbb7-161">type</span><span class="sxs-lookup"><span data-stu-id="8dbb7-161">type</span></span>|<span data-ttu-id="8dbb7-162">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-162">String</span></span>| <span data-ttu-id="8dbb7-163">役割の割り当てに対する操作の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-163">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="8dbb7-164">値は次の`AdminAdd`ようになります。管理者が役割にユーザーを追加します。`UserAdd`: ユーザーが役割の割り当てを追加します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-164">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="8dbb7-165">userId</span><span class="sxs-lookup"><span data-stu-id="8dbb7-165">userId</span></span>|<span data-ttu-id="8dbb7-166">String</span><span class="sxs-lookup"><span data-stu-id="8dbb7-166">String</span></span>| <span data-ttu-id="8dbb7-167">ユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dbb7-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8dbb7-168">Relationships</span></span>
| <span data-ttu-id="8dbb7-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8dbb7-169">Relationship</span></span> | <span data-ttu-id="8dbb7-170">型</span><span class="sxs-lookup"><span data-stu-id="8dbb7-170">Type</span></span>        | <span data-ttu-id="8dbb7-171">説明</span><span class="sxs-lookup"><span data-stu-id="8dbb7-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8dbb7-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="8dbb7-172">roleInfo</span></span>|[<span data-ttu-id="8dbb7-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="8dbb7-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="8dbb7-174">役割の割り当て要求の roleInfo オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dbb7-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8dbb7-175">JSON representation</span></span>

<span data-ttu-id="8dbb7-176">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
