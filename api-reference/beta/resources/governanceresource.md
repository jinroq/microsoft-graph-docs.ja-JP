---
title: governanceResource リソースの種類
description: 特権 id 管理 (PIM) によって管理される可能性があるリソースを表します。 Azure リソースの場合は、サブスクリプション、リソースグループ、仮想マシン、SQL データベースなどのリソースを使用できます。
localization_priority: Normal
ms.openlocfilehash: 92a738350a47cc9eaf436382d020330fac89db1f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547426"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="b6b02-104">governanceResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b6b02-104">governanceResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6b02-105">特権 id 管理 (PIM) によって管理される可能性があるリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="b6b02-105">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="b6b02-106">Azure リソースの場合は、サブスクリプション、リソースグループ、仮想マシン、SQL データベースなどのリソースを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b6b02-106">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="b6b02-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b6b02-107">Methods</span></span>

| <span data-ttu-id="b6b02-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b6b02-108">Method</span></span>          | <span data-ttu-id="b6b02-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b6b02-109">Return Type</span></span> |<span data-ttu-id="b6b02-110">説明</span><span class="sxs-lookup"><span data-stu-id="b6b02-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6b02-111">List</span><span class="sxs-lookup"><span data-stu-id="b6b02-111">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="b6b02-112">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6b02-112">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="b6b02-113">要求者がアクセスできるリソースのコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b6b02-113">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="b6b02-114">取得</span><span class="sxs-lookup"><span data-stu-id="b6b02-114">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="b6b02-115">governanceResource</span><span class="sxs-lookup"><span data-stu-id="b6b02-115">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="b6b02-116">id で指定されたリソースエンティティのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b6b02-116">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="b6b02-117">登録</span><span class="sxs-lookup"><span data-stu-id="b6b02-117">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="b6b02-118">管理されていない Azure サブスクリプションまたは管理グループを PIM サービスに登録します。</span><span class="sxs-lookup"><span data-stu-id="b6b02-118">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="b6b02-119">`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`</span><span class="sxs-lookup"><span data-stu-id="b6b02-119">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="b6b02-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6b02-120">Properties</span></span>
| <span data-ttu-id="b6b02-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6b02-121">Property</span></span>          |<span data-ttu-id="b6b02-122">型</span><span class="sxs-lookup"><span data-stu-id="b6b02-122">Type</span></span>         |<span data-ttu-id="b6b02-123">説明</span><span class="sxs-lookup"><span data-stu-id="b6b02-123">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="b6b02-124">id</span><span class="sxs-lookup"><span data-stu-id="b6b02-124">id</span></span>                 |<span data-ttu-id="b6b02-125">String</span><span class="sxs-lookup"><span data-stu-id="b6b02-125">String</span></span>     |<span data-ttu-id="b6b02-126">リソースの id。</span><span class="sxs-lookup"><span data-stu-id="b6b02-126">The id of the resource.</span></span> <span data-ttu-id="b6b02-127">GUID 形式です。</span><span class="sxs-lookup"><span data-stu-id="b6b02-127">It is in GUID format.</span></span>|
|<span data-ttu-id="b6b02-128">externalId</span><span class="sxs-lookup"><span data-stu-id="b6b02-128">externalId</span></span>           |<span data-ttu-id="b6b02-129">String</span><span class="sxs-lookup"><span data-stu-id="b6b02-129">String</span></span>   |<span data-ttu-id="b6b02-130">外部システムの元の id を表す、リソースの外部 id。</span><span class="sxs-lookup"><span data-stu-id="b6b02-130">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="b6b02-131">たとえば、サブスクリプションリソースの外部 id は "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac" にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6b02-131">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="b6b02-132">type</span><span class="sxs-lookup"><span data-stu-id="b6b02-132">type</span></span>               |<span data-ttu-id="b6b02-133">String</span><span class="sxs-lookup"><span data-stu-id="b6b02-133">String</span></span>     |<span data-ttu-id="b6b02-134">必須。</span><span class="sxs-lookup"><span data-stu-id="b6b02-134">Required.</span></span> <span data-ttu-id="b6b02-135">リソースの種類。</span><span class="sxs-lookup"><span data-stu-id="b6b02-135">Resource type.</span></span> <span data-ttu-id="b6b02-136">たとえば、Azure リソースの場合、この型は "Subscription"、"ResourceGroup"、"Microsoft .sql/server" などになります。</span><span class="sxs-lookup"><span data-stu-id="b6b02-136">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="b6b02-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b6b02-137">displayName</span></span>        |<span data-ttu-id="b6b02-138">String</span><span class="sxs-lookup"><span data-stu-id="b6b02-138">String</span></span>     |<span data-ttu-id="b6b02-139">リソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="b6b02-139">The display name of the resource.</span></span>|
|<span data-ttu-id="b6b02-140">status</span><span class="sxs-lookup"><span data-stu-id="b6b02-140">status</span></span>             |<span data-ttu-id="b6b02-141">String</span><span class="sxs-lookup"><span data-stu-id="b6b02-141">String</span></span>     |<span data-ttu-id="b6b02-142">指定されたリソースの状態。</span><span class="sxs-lookup"><span data-stu-id="b6b02-142">The status of a given resource.</span></span> <span data-ttu-id="b6b02-143">たとえば、リソースがロックされているかどうかを表すことが`Active` / `Locked`できます (値:)。</span><span class="sxs-lookup"><span data-stu-id="b6b02-143">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="b6b02-144">注: 今後、このプロパティを拡張して、より多くのシナリオをサポートすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6b02-144">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="b6b02-145">registereddatetime</span><span class="sxs-lookup"><span data-stu-id="b6b02-145">registeredDateTime</span></span>|<span data-ttu-id="b6b02-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6b02-146">DateTimeOffset</span></span>      |<span data-ttu-id="b6b02-147">リソースが PIM に登録されている日時を表します。</span><span class="sxs-lookup"><span data-stu-id="b6b02-147">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="b6b02-148">registeredroot</span><span class="sxs-lookup"><span data-stu-id="b6b02-148">registeredRoot</span></span>|<span data-ttu-id="b6b02-149">String</span><span class="sxs-lookup"><span data-stu-id="b6b02-149">String</span></span>      |<span data-ttu-id="b6b02-150">PIM に登録されているリソースのルートスコープの externalid。</span><span class="sxs-lookup"><span data-stu-id="b6b02-150">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="b6b02-151">ルートスコープには、親、親、または上位の先祖リソースを指定できます。</span><span class="sxs-lookup"><span data-stu-id="b6b02-151">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="b6b02-152">role割り当て数</span><span class="sxs-lookup"><span data-stu-id="b6b02-152">roleAssignmentCount</span></span>|<span data-ttu-id="b6b02-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b02-153">Int32</span></span>      |<span data-ttu-id="b6b02-154">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b6b02-154">Optional.</span></span> <span data-ttu-id="b6b02-155">指定したリソースのロール割り当ての数。</span><span class="sxs-lookup"><span data-stu-id="b6b02-155">The number of role assignments for the given resource.</span></span> <span data-ttu-id="b6b02-156">プロパティを取得するには、クエリ`$select=roleAssignmentCount`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="b6b02-156">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="b6b02-157">roledefinitioncount</span><span class="sxs-lookup"><span data-stu-id="b6b02-157">roleDefinitionCount</span></span>|<span data-ttu-id="b6b02-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b02-158">Int32</span></span>      |<span data-ttu-id="b6b02-159">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b6b02-159">Optional.</span></span> <span data-ttu-id="b6b02-160">指定したリソースのロール定義の数。</span><span class="sxs-lookup"><span data-stu-id="b6b02-160">The number of role definitions for the given resource.</span></span> <span data-ttu-id="b6b02-161">プロパティを取得するには、クエリ`$select=roleDefinitionCount`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="b6b02-161">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="b6b02-162">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6b02-162">permissions</span></span>|[<span data-ttu-id="b6b02-163">governancePermission</span><span class="sxs-lookup"><span data-stu-id="b6b02-163">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="b6b02-164">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b6b02-164">Optional.</span></span> <span data-ttu-id="b6b02-165">これは、リソースへの要求者のアクセスの状態を表します。プロパティを取得するには、クエリ`$select=permissions`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="b6b02-165">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6b02-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b6b02-166">Relationships</span></span>
| <span data-ttu-id="b6b02-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b6b02-167">Relationship</span></span>   | <span data-ttu-id="b6b02-168">型</span><span class="sxs-lookup"><span data-stu-id="b6b02-168">Type</span></span>                                         |<span data-ttu-id="b6b02-169">説明</span><span class="sxs-lookup"><span data-stu-id="b6b02-169">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="b6b02-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="b6b02-170">roleAssignments</span></span> |<span data-ttu-id="b6b02-171">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6b02-171">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="b6b02-172">リソースのロール割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="b6b02-172">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="b6b02-173">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="b6b02-173">roleDefinitions</span></span> |<span data-ttu-id="b6b02-174">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6b02-174">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="b6b02-175">リソースのロール日のコレクション。</span><span class="sxs-lookup"><span data-stu-id="b6b02-175">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="b6b02-176">rolerequests 要求</span><span class="sxs-lookup"><span data-stu-id="b6b02-176">roleAssignmentRequests</span></span> |<span data-ttu-id="b6b02-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6b02-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="b6b02-178">リソースに対する役割の割り当て要求のコレクション。</span><span class="sxs-lookup"><span data-stu-id="b6b02-178">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="b6b02-179">rolesettings</span><span class="sxs-lookup"><span data-stu-id="b6b02-179">roleSettings</span></span> |<span data-ttu-id="b6b02-180">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b6b02-180">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="b6b02-181">リソースのロール設定のコレクション。</span><span class="sxs-lookup"><span data-stu-id="b6b02-181">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="b6b02-182">親行</span><span class="sxs-lookup"><span data-stu-id="b6b02-182">parent</span></span>          |[<span data-ttu-id="b6b02-183">governanceResource</span><span class="sxs-lookup"><span data-stu-id="b6b02-183">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="b6b02-184">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b6b02-184">Read-only.</span></span> <span data-ttu-id="b6b02-185">親リソース。</span><span class="sxs-lookup"><span data-stu-id="b6b02-185">The parent resource.</span></span> <span data-ttu-id="b6b02-186">シナリオ`pimforazurerbac`の場合は、リソースが属するサブスクリプションを表すことができます。</span><span class="sxs-lookup"><span data-stu-id="b6b02-186">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6b02-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b6b02-187">JSON representation</span></span>

<span data-ttu-id="b6b02-188">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6b02-188">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
