---
title: governanceRoleAssignment リソースの種類
description: ユーザーまたはグループの役割への割り当てを表します。
localization_priority: Normal
ms.openlocfilehash: 77a5238aa337dd8d273d3156d285e081c4bc8875
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547443"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="21f23-103">governanceRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21f23-103">governanceRoleAssignment resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21f23-104">ユーザーまたはグループの役割への割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="21f23-104">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="21f23-105">Privileged Identity Management (PIM) は、次の2種類の割り当てをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="21f23-105">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="21f23-106">アクティブな割り当て-リソースへの直接/アクティブ化されたアクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="21f23-106">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="21f23-107">対象となる割り当て-リソースへの特権アクセスの中間段階であり、アクセスなしと直接アクセスの間の関係を表します。</span><span class="sxs-lookup"><span data-stu-id="21f23-107">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="21f23-108">管理者は、ユーザーまたは`eligible assignment`グループを事前に割り当てることができます。 `activation`また、 `eligible assignment`アクセスが必要になったときに、に対して、で数時間にリソースへの即時アクセスを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="21f23-108">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="21f23-109">アクティブ化した`active assignment`後、ユーザー/グループメンバーに対してが作成され、アクティブ化された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="21f23-109">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="21f23-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="21f23-110">Methods</span></span>

| <span data-ttu-id="21f23-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="21f23-111">Method</span></span>          | <span data-ttu-id="21f23-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="21f23-112">Return Type</span></span> |<span data-ttu-id="21f23-113">説明</span><span class="sxs-lookup"><span data-stu-id="21f23-113">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="21f23-114">Get</span><span class="sxs-lookup"><span data-stu-id="21f23-114">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="21f23-115">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="21f23-115">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="21f23-116">役割割り当てエンティティのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="21f23-116">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="21f23-117">List</span><span class="sxs-lookup"><span data-stu-id="21f23-117">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="21f23-118">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="21f23-118">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="21f23-119">リソースに対する役割の割り当てのコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="21f23-119">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="21f23-120">Export</span><span class="sxs-lookup"><span data-stu-id="21f23-120">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="21f23-121">オクテットストリーム</span><span class="sxs-lookup"><span data-stu-id="21f23-121">octet-stream</span></span> |<span data-ttu-id="21f23-122">リソースに対する役割の割り当てのコレクションをダウンロードし、 `.csv`ファイルとして保存します。</span><span class="sxs-lookup"><span data-stu-id="21f23-122">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="21f23-123">`PATCH` `DELETE` `POST` `PUT`エンティティセットでは、、、、または操作はサポートされていません。 `roleAssignments`</span><span class="sxs-lookup"><span data-stu-id="21f23-123">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="21f23-124">の`governanceRoleAssignment`作成、更新、および削除操作は、によっ`governanceRoleAssignmentRequest`て実行されます。</span><span class="sxs-lookup"><span data-stu-id="21f23-124">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="21f23-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21f23-125">Properties</span></span>
| <span data-ttu-id="21f23-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21f23-126">Property</span></span>  | <span data-ttu-id="21f23-127">型</span><span class="sxs-lookup"><span data-stu-id="21f23-127">Type</span></span>      |<span data-ttu-id="21f23-128">説明</span><span class="sxs-lookup"><span data-stu-id="21f23-128">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="21f23-129">id</span><span class="sxs-lookup"><span data-stu-id="21f23-129">id</span></span>         |<span data-ttu-id="21f23-130">String</span><span class="sxs-lookup"><span data-stu-id="21f23-130">String</span></span>     |<span data-ttu-id="21f23-131">役割の割り当ての ID。</span><span class="sxs-lookup"><span data-stu-id="21f23-131">The ID of the role assignment.</span></span> <span data-ttu-id="21f23-132">GUID 形式です。</span><span class="sxs-lookup"><span data-stu-id="21f23-132">It is in GUID format.</span></span>|
|<span data-ttu-id="21f23-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="21f23-133">resourceId</span></span> |<span data-ttu-id="21f23-134">String</span><span class="sxs-lookup"><span data-stu-id="21f23-134">String</span></span>     |<span data-ttu-id="21f23-135">必須。</span><span class="sxs-lookup"><span data-stu-id="21f23-135">Required.</span></span> <span data-ttu-id="21f23-136">役割の割り当てが関連付けられているリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="21f23-136">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="21f23-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="21f23-137">roleDefinitionId</span></span>|<span data-ttu-id="21f23-138">String</span><span class="sxs-lookup"><span data-stu-id="21f23-138">String</span></span>|<span data-ttu-id="21f23-139">必須。</span><span class="sxs-lookup"><span data-stu-id="21f23-139">Required.</span></span> <span data-ttu-id="21f23-140">役割の割り当てが関連付けられているロール定義の ID。</span><span class="sxs-lookup"><span data-stu-id="21f23-140">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="21f23-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="21f23-141">subjectId</span></span>|<span data-ttu-id="21f23-142">String</span><span class="sxs-lookup"><span data-stu-id="21f23-142">String</span></span>       |<span data-ttu-id="21f23-143">必須。</span><span class="sxs-lookup"><span data-stu-id="21f23-143">Required.</span></span> <span data-ttu-id="21f23-144">役割の割り当てが関連付けられているサブジェクトの ID。</span><span class="sxs-lookup"><span data-stu-id="21f23-144">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="21f23-145">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="21f23-145">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="21f23-146">String</span><span class="sxs-lookup"><span data-stu-id="21f23-146">String</span></span>|<span data-ttu-id="21f23-147">が`active assignment`で、アクティブ化によって作成され`eligible assignment`たものである場合は、 `eligible assignment`その ID を表します。それ以外の場合、 `null`値はです。</span><span class="sxs-lookup"><span data-stu-id="21f23-147">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="21f23-148">externalId</span><span class="sxs-lookup"><span data-stu-id="21f23-148">externalId</span></span>   |<span data-ttu-id="21f23-149">String</span><span class="sxs-lookup"><span data-stu-id="21f23-149">String</span></span>     |<span data-ttu-id="21f23-150">プロバイダーでの役割の割り当てを識別するために使用されるリソースの、外部 ID。</span><span class="sxs-lookup"><span data-stu-id="21f23-150">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="21f23-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="21f23-151">startDateTime</span></span>|<span data-ttu-id="21f23-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21f23-152">DateTimeOffset</span></span>|<span data-ttu-id="21f23-153">役割の割り当ての開始時刻。</span><span class="sxs-lookup"><span data-stu-id="21f23-153">The start time of the role assignment.</span></span> <span data-ttu-id="21f23-154">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="21f23-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="21f23-155">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="21f23-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="21f23-156">endDateTime</span><span class="sxs-lookup"><span data-stu-id="21f23-156">endDateTime</span></span>|<span data-ttu-id="21f23-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21f23-157">DateTimeOffset</span></span>|<span data-ttu-id="21f23-158">非永続的な役割の割り当ての場合、これは、役割の割り当てが期限切れになる時刻です。</span><span class="sxs-lookup"><span data-stu-id="21f23-158">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="21f23-159">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="21f23-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="21f23-160">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="21f23-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="21f23-161">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="21f23-161">assignmentState</span></span>|<span data-ttu-id="21f23-162">String</span><span class="sxs-lookup"><span data-stu-id="21f23-162">String</span></span>  |<span data-ttu-id="21f23-163">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="21f23-163">The state of the assignment.</span></span> <span data-ttu-id="21f23-164">値には、</span><span class="sxs-lookup"><span data-stu-id="21f23-164">The value can be</span></span> <ul><li> <span data-ttu-id="21f23-165">`Eligible`適格な割り当ての場合</span><span class="sxs-lookup"><span data-stu-id="21f23-165">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="21f23-166">`Active`-管理者によって`Active`直接割り当てられている場合、またはユーザーによる資格のある割り当てでアクティブ化されている場合。</span><span class="sxs-lookup"><span data-stu-id="21f23-166">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="21f23-167">memberType</span><span class="sxs-lookup"><span data-stu-id="21f23-167">memberType</span></span>|<span data-ttu-id="21f23-168">String</span><span class="sxs-lookup"><span data-stu-id="21f23-168">String</span></span>      |<span data-ttu-id="21f23-169">メンバーの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="21f23-169">The type of member.</span></span> <span data-ttu-id="21f23-170">値は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="21f23-170">The value can be:</span></span> <ul><li><span data-ttu-id="21f23-171">`Inherited`-役割の割り当ては、親のリソーススコープから継承されます。</span><span class="sxs-lookup"><span data-stu-id="21f23-171">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="21f23-172">`Group`-役割の割り当ては継承されませんが、グループの割り当てのメンバーシップから取得されます。</span><span class="sxs-lookup"><span data-stu-id="21f23-172">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="21f23-173">`User`-役割の割り当ては、継承されたものでも、グループの割り当てにもありません。</span><span class="sxs-lookup"><span data-stu-id="21f23-173">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="21f23-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21f23-174">Relationships</span></span>
| <span data-ttu-id="21f23-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21f23-175">Relationship</span></span> | <span data-ttu-id="21f23-176">型</span><span class="sxs-lookup"><span data-stu-id="21f23-176">Type</span></span>   |<span data-ttu-id="21f23-177">説明</span><span class="sxs-lookup"><span data-stu-id="21f23-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21f23-178">リソース</span><span class="sxs-lookup"><span data-stu-id="21f23-178">resource</span></span>|[<span data-ttu-id="21f23-179">governanceResource</span><span class="sxs-lookup"><span data-stu-id="21f23-179">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="21f23-180">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="21f23-180">Read-only.</span></span> <span data-ttu-id="21f23-181">役割の割り当てに関連付けられているリソース。</span><span class="sxs-lookup"><span data-stu-id="21f23-181">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="21f23-182">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="21f23-182">roleDefinition</span></span>|[<span data-ttu-id="21f23-183">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="21f23-183">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="21f23-184">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="21f23-184">Read-only.</span></span> <span data-ttu-id="21f23-185">役割の割り当てに関連付けられている役割の定義。</span><span class="sxs-lookup"><span data-stu-id="21f23-185">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="21f23-186">subject</span><span class="sxs-lookup"><span data-stu-id="21f23-186">subject</span></span>|[<span data-ttu-id="21f23-187">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="21f23-187">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="21f23-188">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="21f23-188">Read-only.</span></span> <span data-ttu-id="21f23-189">役割の割り当てに関連付けられている件名。</span><span class="sxs-lookup"><span data-stu-id="21f23-189">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="21f23-190">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="21f23-190">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="21f23-191">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="21f23-191">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="21f23-192">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="21f23-192">Read-only.</span></span> <span data-ttu-id="21f23-193">が`active assignment`で、アクティブ化のために作成され`eligible assignment`ている場合は、そのオブジェクト`eligible assignment`を表します。それ以外の場合、 `null`値はです。</span><span class="sxs-lookup"><span data-stu-id="21f23-193">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="21f23-194">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21f23-194">JSON representation</span></span>

<span data-ttu-id="21f23-195">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21f23-195">Here is a JSON representation of the resource.</span></span>


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
