---
title: governanceRoleAssignment リソースの種類
description: ロールにユーザーまたはグループの割り当てを表します。
localization_priority: Normal
ms.openlocfilehash: 77a5238aa337dd8d273d3156d285e081c4bc8875
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512683"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="f40a2-103">governanceRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f40a2-103">governanceRoleAssignment resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f40a2-104">ロールにユーザーまたはグループの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="f40a2-104">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="f40a2-105">特権を持つユーザーの管理 (PIM) には、割り当ての 2 つの種類がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f40a2-105">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="f40a2-106">アクティブな割り当てでは、リソースに対してダイレクト/有効化済アクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="f40a2-106">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="f40a2-107">対象となる割り当てのないアクセスと直接アクセスの間でのリソースへのアクセス権限の中間の段階を表します。</span><span class="sxs-lookup"><span data-stu-id="f40a2-107">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="f40a2-108">管理者はユーザーまたはグループに割り当てることができます`eligible assignment`アクセス権が必要な事前に、必ず`activation`に、`eligible assignment`は、いくつかの時間のリソースへのインスタント アクセスを得るために必要な。</span><span class="sxs-lookup"><span data-stu-id="f40a2-108">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="f40a2-109">ライセンス認証の後、`active assignment`のアクティブ化の状態を示すためにユーザーまたはグループのメンバーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="f40a2-109">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="f40a2-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f40a2-110">Methods</span></span>

| <span data-ttu-id="f40a2-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="f40a2-111">Method</span></span>          | <span data-ttu-id="f40a2-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f40a2-112">Return Type</span></span> |<span data-ttu-id="f40a2-113">説明</span><span class="sxs-lookup"><span data-stu-id="f40a2-113">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="f40a2-114">Get</span><span class="sxs-lookup"><span data-stu-id="f40a2-114">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="f40a2-115">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f40a2-115">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="f40a2-116">ロール割り当てのエンティティのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f40a2-116">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="f40a2-117">List</span><span class="sxs-lookup"><span data-stu-id="f40a2-117">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="f40a2-118">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f40a2-118">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="f40a2-119">リソースの役割の割り当ての一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="f40a2-119">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="f40a2-120">Export</span><span class="sxs-lookup"><span data-stu-id="f40a2-120">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="f40a2-121">オクテット ストリーム</span><span class="sxs-lookup"><span data-stu-id="f40a2-121">octet-stream</span></span> |<span data-ttu-id="f40a2-122">リソースの役割の割り当てのコレクションをダウンロードし、名前を付けて、`.csv`ファイルです。</span><span class="sxs-lookup"><span data-stu-id="f40a2-122">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="f40a2-123">No `POST`、 `PUT`、 `PATCH`、または`DELETE`の操作はサポートされて、`roleAssignments`のエンティティ セット。</span><span class="sxs-lookup"><span data-stu-id="f40a2-123">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="f40a2-124">任意の作成では、更新、および削除の操作で`governanceRoleAssignment`で行われます`governanceRoleAssignmentRequest`。</span><span class="sxs-lookup"><span data-stu-id="f40a2-124">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="f40a2-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f40a2-125">Properties</span></span>
| <span data-ttu-id="f40a2-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f40a2-126">Property</span></span>  | <span data-ttu-id="f40a2-127">型</span><span class="sxs-lookup"><span data-stu-id="f40a2-127">Type</span></span>      |<span data-ttu-id="f40a2-128">説明</span><span class="sxs-lookup"><span data-stu-id="f40a2-128">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="f40a2-129">id</span><span class="sxs-lookup"><span data-stu-id="f40a2-129">id</span></span>         |<span data-ttu-id="f40a2-130">String</span><span class="sxs-lookup"><span data-stu-id="f40a2-130">String</span></span>     |<span data-ttu-id="f40a2-131">役割の割り当ての ID です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-131">The ID of the role assignment.</span></span> <span data-ttu-id="f40a2-132">GUID 形式であります。</span><span class="sxs-lookup"><span data-stu-id="f40a2-132">It is in GUID format.</span></span>|
|<span data-ttu-id="f40a2-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="f40a2-133">resourceId</span></span> |<span data-ttu-id="f40a2-134">String</span><span class="sxs-lookup"><span data-stu-id="f40a2-134">String</span></span>     |<span data-ttu-id="f40a2-135">必須。</span><span class="sxs-lookup"><span data-stu-id="f40a2-135">Required.</span></span> <span data-ttu-id="f40a2-136">ロールの割り当てに関連付けられているリソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-136">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="f40a2-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f40a2-137">roleDefinitionId</span></span>|<span data-ttu-id="f40a2-138">String</span><span class="sxs-lookup"><span data-stu-id="f40a2-138">String</span></span>|<span data-ttu-id="f40a2-139">必須。</span><span class="sxs-lookup"><span data-stu-id="f40a2-139">Required.</span></span> <span data-ttu-id="f40a2-140">ロールの割り当てに関連付けられている役割の定義の ID です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-140">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="f40a2-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="f40a2-141">subjectId</span></span>|<span data-ttu-id="f40a2-142">String</span><span class="sxs-lookup"><span data-stu-id="f40a2-142">String</span></span>       |<span data-ttu-id="f40a2-143">必須。</span><span class="sxs-lookup"><span data-stu-id="f40a2-143">Required.</span></span> <span data-ttu-id="f40a2-144">ロールの割り当てに関連付けられているサブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-144">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="f40a2-145">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="f40a2-145">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="f40a2-146">String</span><span class="sxs-lookup"><span data-stu-id="f40a2-146">String</span></span>|<span data-ttu-id="f40a2-147">場合は、`active assignment`のアクティブ化のために作成されると、 `eligible assignment`、その ID を表す`eligible assignment`です。値は、それ以外の場合、 `null`。</span><span class="sxs-lookup"><span data-stu-id="f40a2-147">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="f40a2-148">externalId</span><span class="sxs-lookup"><span data-stu-id="f40a2-148">externalId</span></span>   |<span data-ttu-id="f40a2-149">String</span><span class="sxs-lookup"><span data-stu-id="f40a2-149">String</span></span>     |<span data-ttu-id="f40a2-150">外部 ID プロバイダーの役割の割り当てを識別するために使用されるリソースです。</span><span class="sxs-lookup"><span data-stu-id="f40a2-150">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="f40a2-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f40a2-151">startDateTime</span></span>|<span data-ttu-id="f40a2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f40a2-152">DateTimeOffset</span></span>|<span data-ttu-id="f40a2-153">役割の割り当ての開始時刻。</span><span class="sxs-lookup"><span data-stu-id="f40a2-153">The start time of the role assignment.</span></span> <span data-ttu-id="f40a2-154">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f40a2-155">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f40a2-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f40a2-156">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f40a2-156">endDateTime</span></span>|<span data-ttu-id="f40a2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f40a2-157">DateTimeOffset</span></span>|<span data-ttu-id="f40a2-158">非永続的なロールの割り当てでは、これは、時間とロールの割り当て、期限切れにします。</span><span class="sxs-lookup"><span data-stu-id="f40a2-158">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="f40a2-159">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f40a2-160">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f40a2-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f40a2-161">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f40a2-161">assignmentState</span></span>|<span data-ttu-id="f40a2-162">String</span><span class="sxs-lookup"><span data-stu-id="f40a2-162">String</span></span>  |<span data-ttu-id="f40a2-163">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-163">The state of the assignment.</span></span> <span data-ttu-id="f40a2-164">値は、します。</span><span class="sxs-lookup"><span data-stu-id="f40a2-164">The value can be</span></span> <ul><li> <span data-ttu-id="f40a2-165">`Eligible`対象となる割り当ての</span><span class="sxs-lookup"><span data-stu-id="f40a2-165">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="f40a2-166">`Active`-直接割り当てられている場合`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</span><span class="sxs-lookup"><span data-stu-id="f40a2-166">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="f40a2-167">memberType</span><span class="sxs-lookup"><span data-stu-id="f40a2-167">memberType</span></span>|<span data-ttu-id="f40a2-168">String</span><span class="sxs-lookup"><span data-stu-id="f40a2-168">String</span></span>      |<span data-ttu-id="f40a2-169">メンバーの型。</span><span class="sxs-lookup"><span data-stu-id="f40a2-169">The type of member.</span></span> <span data-ttu-id="f40a2-170">値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="f40a2-170">The value can be:</span></span> <ul><li><span data-ttu-id="f40a2-171">`Inherited`ロールの割り当ては、親のリソースのスコープから継承します。</span><span class="sxs-lookup"><span data-stu-id="f40a2-171">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="f40a2-172">`Group`ロールの割り当ては継承されませんが、グループの割り当てのメンバーシップは、</span><span class="sxs-lookup"><span data-stu-id="f40a2-172">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="f40a2-173">`User`-ロールの割り当ては、どちらも継承も割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="f40a2-173">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="f40a2-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f40a2-174">Relationships</span></span>
| <span data-ttu-id="f40a2-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f40a2-175">Relationship</span></span> | <span data-ttu-id="f40a2-176">型</span><span class="sxs-lookup"><span data-stu-id="f40a2-176">Type</span></span>   |<span data-ttu-id="f40a2-177">説明</span><span class="sxs-lookup"><span data-stu-id="f40a2-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f40a2-178">リソース</span><span class="sxs-lookup"><span data-stu-id="f40a2-178">resource</span></span>|[<span data-ttu-id="f40a2-179">governanceResource</span><span class="sxs-lookup"><span data-stu-id="f40a2-179">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="f40a2-180">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-180">Read-only.</span></span> <span data-ttu-id="f40a2-181">ロールの割り当てに関連付けられているリソースです。</span><span class="sxs-lookup"><span data-stu-id="f40a2-181">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="f40a2-182">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f40a2-182">roleDefinition</span></span>|[<span data-ttu-id="f40a2-183">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f40a2-183">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="f40a2-184">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-184">Read-only.</span></span> <span data-ttu-id="f40a2-185">ロールの割り当てに関連付けられているロールの定義。</span><span class="sxs-lookup"><span data-stu-id="f40a2-185">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="f40a2-186">subject</span><span class="sxs-lookup"><span data-stu-id="f40a2-186">subject</span></span>|[<span data-ttu-id="f40a2-187">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="f40a2-187">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="f40a2-188">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-188">Read-only.</span></span> <span data-ttu-id="f40a2-189">ロールの割り当てに関連付けられている件名です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-189">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="f40a2-190">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f40a2-190">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="f40a2-191">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f40a2-191">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="f40a2-192">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-192">Read-only.</span></span> <span data-ttu-id="f40a2-193">場合は、`active assignment`のアクティブ化のために作成されると、 `eligible assignment`、そのオブジェクトを表す`eligible assignment`です。値は、それ以外の場合、 `null`。</span><span class="sxs-lookup"><span data-stu-id="f40a2-193">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f40a2-194">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f40a2-194">JSON representation</span></span>

<span data-ttu-id="f40a2-195">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f40a2-195">Here is a JSON representation of the resource.</span></span>


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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
