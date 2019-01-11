---
title: governanceRoleAssignment リソースの種類
description: ロールにユーザーまたはグループの割り当てを表します。
localization_priority: Normal
ms.openlocfilehash: d873b122f319ca82882727f065818b33f7f9d44d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882692"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="7f695-103">governanceRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f695-103">governanceRoleAssignment resource type</span></span>
> <span data-ttu-id="7f695-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f695-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f695-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f695-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f695-106">ロールにユーザーまたはグループの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="7f695-106">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="7f695-107">特権を持つユーザーの管理 (PIM) には、割り当ての 2 つの種類がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7f695-107">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="7f695-108">アクティブな割り当てでは、リソースに対してダイレクト/有効化済アクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="7f695-108">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="7f695-109">対象となる割り当てのないアクセスと直接アクセスの間でのリソースへのアクセス権限の中間の段階を表します。</span><span class="sxs-lookup"><span data-stu-id="7f695-109">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="7f695-110">管理者はユーザーまたはグループに割り当てることができます`eligible assignment`アクセス権が必要な事前に、必ず`activation`に、`eligible assignment`は、いくつかの時間のリソースへのインスタント アクセスを得るために必要な。</span><span class="sxs-lookup"><span data-stu-id="7f695-110">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="7f695-111">ライセンス認証の後、`active assignment`のアクティブ化の状態を示すためにユーザーまたはグループのメンバーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="7f695-111">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="7f695-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f695-112">Methods</span></span>

| <span data-ttu-id="7f695-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f695-113">Method</span></span>          | <span data-ttu-id="7f695-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f695-114">Return Type</span></span> |<span data-ttu-id="7f695-115">説明</span><span class="sxs-lookup"><span data-stu-id="7f695-115">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="7f695-116">Get</span><span class="sxs-lookup"><span data-stu-id="7f695-116">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="7f695-117">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7f695-117">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="7f695-118">ロール割り当てのエンティティのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f695-118">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="7f695-119">List</span><span class="sxs-lookup"><span data-stu-id="7f695-119">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="7f695-120">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7f695-120">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="7f695-121">リソースの役割の割り当ての一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="7f695-121">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="7f695-122">Export</span><span class="sxs-lookup"><span data-stu-id="7f695-122">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="7f695-123">オクテット ストリーム</span><span class="sxs-lookup"><span data-stu-id="7f695-123">octet-stream</span></span> |<span data-ttu-id="7f695-124">リソースの役割の割り当てのコレクションをダウンロードし、名前を付けて、`.csv`ファイルです。</span><span class="sxs-lookup"><span data-stu-id="7f695-124">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="7f695-125">No `POST`、 `PUT`、 `PATCH`、または`DELETE`の操作はサポートされて、`roleAssignments`のエンティティ セット。</span><span class="sxs-lookup"><span data-stu-id="7f695-125">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="7f695-126">任意の作成では、更新、および削除の操作で`governanceRoleAssignment`で行われます`governanceRoleAssignmentRequest`。</span><span class="sxs-lookup"><span data-stu-id="7f695-126">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="7f695-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f695-127">Properties</span></span>
| <span data-ttu-id="7f695-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f695-128">Property</span></span>  | <span data-ttu-id="7f695-129">種類</span><span class="sxs-lookup"><span data-stu-id="7f695-129">Type</span></span>      |<span data-ttu-id="7f695-130">説明</span><span class="sxs-lookup"><span data-stu-id="7f695-130">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="7f695-131">ID</span><span class="sxs-lookup"><span data-stu-id="7f695-131">id</span></span>         |<span data-ttu-id="7f695-132">String</span><span class="sxs-lookup"><span data-stu-id="7f695-132">String</span></span>     |<span data-ttu-id="7f695-133">役割の割り当ての ID です。</span><span class="sxs-lookup"><span data-stu-id="7f695-133">The ID of the role assignment.</span></span> <span data-ttu-id="7f695-134">GUID 形式であります。</span><span class="sxs-lookup"><span data-stu-id="7f695-134">It is in GUID format.</span></span>|
|<span data-ttu-id="7f695-135">resourceId</span><span class="sxs-lookup"><span data-stu-id="7f695-135">resourceId</span></span> |<span data-ttu-id="7f695-136">String</span><span class="sxs-lookup"><span data-stu-id="7f695-136">String</span></span>     |<span data-ttu-id="7f695-137">必須。</span><span class="sxs-lookup"><span data-stu-id="7f695-137">Required.</span></span> <span data-ttu-id="7f695-138">ロールの割り当てに関連付けられているリソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="7f695-138">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="7f695-139">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7f695-139">roleDefinitionId</span></span>|<span data-ttu-id="7f695-140">String</span><span class="sxs-lookup"><span data-stu-id="7f695-140">String</span></span>|<span data-ttu-id="7f695-141">必須。</span><span class="sxs-lookup"><span data-stu-id="7f695-141">Required.</span></span> <span data-ttu-id="7f695-142">ロールの割り当てに関連付けられている役割の定義の ID です。</span><span class="sxs-lookup"><span data-stu-id="7f695-142">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="7f695-143">subjectId</span><span class="sxs-lookup"><span data-stu-id="7f695-143">subjectId</span></span>|<span data-ttu-id="7f695-144">String</span><span class="sxs-lookup"><span data-stu-id="7f695-144">String</span></span>       |<span data-ttu-id="7f695-145">必須。</span><span class="sxs-lookup"><span data-stu-id="7f695-145">Required.</span></span> <span data-ttu-id="7f695-146">ロールの割り当てに関連付けられているサブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="7f695-146">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="7f695-147">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="7f695-147">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="7f695-148">String</span><span class="sxs-lookup"><span data-stu-id="7f695-148">String</span></span>|<span data-ttu-id="7f695-149">場合は、`active assignment`のアクティブ化のために作成されると、 `eligible assignment`、その ID を表す`eligible assignment`です。値は、それ以外の場合、 `null`。</span><span class="sxs-lookup"><span data-stu-id="7f695-149">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="7f695-150">externalId</span><span class="sxs-lookup"><span data-stu-id="7f695-150">externalId</span></span>   |<span data-ttu-id="7f695-151">String</span><span class="sxs-lookup"><span data-stu-id="7f695-151">String</span></span>     |<span data-ttu-id="7f695-152">外部 ID プロバイダーの役割の割り当てを識別するために使用されるリソースです。</span><span class="sxs-lookup"><span data-stu-id="7f695-152">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="7f695-153">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7f695-153">startDateTime</span></span>|<span data-ttu-id="7f695-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f695-154">DateTimeOffset</span></span>|<span data-ttu-id="7f695-155">役割の割り当ての開始時刻。</span><span class="sxs-lookup"><span data-stu-id="7f695-155">The start time of the role assignment.</span></span> <span data-ttu-id="7f695-156">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7f695-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f695-157">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7f695-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7f695-158">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7f695-158">endDateTime</span></span>|<span data-ttu-id="7f695-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f695-159">DateTimeOffset</span></span>|<span data-ttu-id="7f695-160">非永続的なロールの割り当てでは、これは、時間とロールの割り当て、期限切れにします。</span><span class="sxs-lookup"><span data-stu-id="7f695-160">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="7f695-161">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7f695-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f695-162">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7f695-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7f695-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7f695-163">assignmentState</span></span>|<span data-ttu-id="7f695-164">String</span><span class="sxs-lookup"><span data-stu-id="7f695-164">String</span></span>  |<span data-ttu-id="7f695-165">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="7f695-165">The state of the assignment.</span></span> <span data-ttu-id="7f695-166">値は、します。</span><span class="sxs-lookup"><span data-stu-id="7f695-166">The value can be</span></span> <ul><li> <span data-ttu-id="7f695-167">`Eligible`対象となる割り当ての</span><span class="sxs-lookup"><span data-stu-id="7f695-167">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="7f695-168">`Active`-直接割り当てられている場合`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</span><span class="sxs-lookup"><span data-stu-id="7f695-168">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="7f695-169">memberType</span><span class="sxs-lookup"><span data-stu-id="7f695-169">memberType</span></span>|<span data-ttu-id="7f695-170">String</span><span class="sxs-lookup"><span data-stu-id="7f695-170">String</span></span>      |<span data-ttu-id="7f695-171">メンバーの型。</span><span class="sxs-lookup"><span data-stu-id="7f695-171">The type of member.</span></span> <span data-ttu-id="7f695-172">値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="7f695-172">The value can be:</span></span> <ul><li><span data-ttu-id="7f695-173">`Inherited`ロールの割り当ては、親のリソースのスコープから継承します。</span><span class="sxs-lookup"><span data-stu-id="7f695-173">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="7f695-174">`Group`ロールの割り当ては継承されませんが、グループの割り当てのメンバーシップは、</span><span class="sxs-lookup"><span data-stu-id="7f695-174">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="7f695-175">`User`-ロールの割り当ては、どちらも継承も割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="7f695-175">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="7f695-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f695-176">Relationships</span></span>
| <span data-ttu-id="7f695-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f695-177">Relationship</span></span> | <span data-ttu-id="7f695-178">型</span><span class="sxs-lookup"><span data-stu-id="7f695-178">Type</span></span>   |<span data-ttu-id="7f695-179">説明</span><span class="sxs-lookup"><span data-stu-id="7f695-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f695-180">リソース</span><span class="sxs-lookup"><span data-stu-id="7f695-180">resource</span></span>|[<span data-ttu-id="7f695-181">governanceResource</span><span class="sxs-lookup"><span data-stu-id="7f695-181">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="7f695-182">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7f695-182">Read-only.</span></span> <span data-ttu-id="7f695-183">ロールの割り当てに関連付けられているリソースです。</span><span class="sxs-lookup"><span data-stu-id="7f695-183">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="7f695-184">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f695-184">roleDefinition</span></span>|[<span data-ttu-id="7f695-185">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f695-185">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="7f695-186">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7f695-186">Read-only.</span></span> <span data-ttu-id="7f695-187">ロールの割り当てに関連付けられているロールの定義。</span><span class="sxs-lookup"><span data-stu-id="7f695-187">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="7f695-188">subject</span><span class="sxs-lookup"><span data-stu-id="7f695-188">subject</span></span>|[<span data-ttu-id="7f695-189">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="7f695-189">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="7f695-190">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7f695-190">Read-only.</span></span> <span data-ttu-id="7f695-191">ロールの割り当てに関連付けられている件名です。</span><span class="sxs-lookup"><span data-stu-id="7f695-191">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="7f695-192">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7f695-192">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="7f695-193">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7f695-193">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="7f695-194">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7f695-194">Read-only.</span></span> <span data-ttu-id="7f695-195">場合は、`active assignment`のアクティブ化のために作成されると、 `eligible assignment`、そのオブジェクトを表す`eligible assignment`です。値は、それ以外の場合、 `null`。</span><span class="sxs-lookup"><span data-stu-id="7f695-195">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7f695-196">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f695-196">JSON representation</span></span>

<span data-ttu-id="7f695-197">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f695-197">Here is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
