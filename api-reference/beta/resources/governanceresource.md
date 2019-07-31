---
title: governanceResource リソースの種類
description: 特権 Id 管理 (PIM) によって管理される可能性があるリソースを表します。 Azure リソースの場合は、サブスクリプション、リソースグループ、仮想マシン、SQL データベースなどのリソースを使用できます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a0429de2cacc816eaf1a603a29a08897650da6e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971922"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="cf5e1-104">governanceResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf5e1-104">governanceResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf5e1-105">特権 Id 管理 (PIM) によって管理される可能性があるリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-105">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="cf5e1-106">Azure リソースの場合は、サブスクリプション、リソースグループ、仮想マシン、SQL データベースなどのリソースを使用できます。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-106">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="cf5e1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf5e1-107">Methods</span></span>

| <span data-ttu-id="cf5e1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf5e1-108">Method</span></span>          | <span data-ttu-id="cf5e1-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cf5e1-109">Return Type</span></span> |<span data-ttu-id="cf5e1-110">説明</span><span class="sxs-lookup"><span data-stu-id="cf5e1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf5e1-111">List</span><span class="sxs-lookup"><span data-stu-id="cf5e1-111">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="cf5e1-112">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cf5e1-112">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="cf5e1-113">要求者がアクセスできるリソースのコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-113">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="cf5e1-114">Get</span><span class="sxs-lookup"><span data-stu-id="cf5e1-114">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="cf5e1-115">governanceResource</span><span class="sxs-lookup"><span data-stu-id="cf5e1-115">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="cf5e1-116">Id で指定されたリソースエンティティのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-116">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="cf5e1-117">登録</span><span class="sxs-lookup"><span data-stu-id="cf5e1-117">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="cf5e1-118">管理されていない Azure サブスクリプションまたは管理グループを PIM サービスに登録します。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-118">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="cf5e1-119">`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`</span><span class="sxs-lookup"><span data-stu-id="cf5e1-119">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="cf5e1-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf5e1-120">Properties</span></span>
| <span data-ttu-id="cf5e1-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf5e1-121">Property</span></span>          |<span data-ttu-id="cf5e1-122">型</span><span class="sxs-lookup"><span data-stu-id="cf5e1-122">Type</span></span>         |<span data-ttu-id="cf5e1-123">説明</span><span class="sxs-lookup"><span data-stu-id="cf5e1-123">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="cf5e1-124">id</span><span class="sxs-lookup"><span data-stu-id="cf5e1-124">id</span></span>                 |<span data-ttu-id="cf5e1-125">文字列</span><span class="sxs-lookup"><span data-stu-id="cf5e1-125">String</span></span>     |<span data-ttu-id="cf5e1-126">リソースの id。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-126">The id of the resource.</span></span> <span data-ttu-id="cf5e1-127">GUID 形式です。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-127">It is in GUID format.</span></span>|
|<span data-ttu-id="cf5e1-128">externalId</span><span class="sxs-lookup"><span data-stu-id="cf5e1-128">externalId</span></span>           |<span data-ttu-id="cf5e1-129">String</span><span class="sxs-lookup"><span data-stu-id="cf5e1-129">String</span></span>   |<span data-ttu-id="cf5e1-130">外部システムの元の id を表す、リソースの外部 id。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-130">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="cf5e1-131">たとえば、サブスクリプションリソースの外部 id は "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac" にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-131">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="cf5e1-132">type</span><span class="sxs-lookup"><span data-stu-id="cf5e1-132">type</span></span>               |<span data-ttu-id="cf5e1-133">String</span><span class="sxs-lookup"><span data-stu-id="cf5e1-133">String</span></span>     |<span data-ttu-id="cf5e1-134">必須。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-134">Required.</span></span> <span data-ttu-id="cf5e1-135">リソースの種類。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-135">Resource type.</span></span> <span data-ttu-id="cf5e1-136">たとえば、Azure リソースの場合、この型は "Subscription"、"ResourceGroup"、"Microsoft .Sql/server" などになります。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-136">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="cf5e1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cf5e1-137">displayName</span></span>        |<span data-ttu-id="cf5e1-138">String</span><span class="sxs-lookup"><span data-stu-id="cf5e1-138">String</span></span>     |<span data-ttu-id="cf5e1-139">リソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-139">The display name of the resource.</span></span>|
|<span data-ttu-id="cf5e1-140">status</span><span class="sxs-lookup"><span data-stu-id="cf5e1-140">status</span></span>             |<span data-ttu-id="cf5e1-141">String</span><span class="sxs-lookup"><span data-stu-id="cf5e1-141">String</span></span>     |<span data-ttu-id="cf5e1-142">指定されたリソースの状態。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-142">The status of a given resource.</span></span> <span data-ttu-id="cf5e1-143">たとえば、リソースがロックされているかどうかを表すことが`Active` / `Locked`できます (値:)。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-143">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="cf5e1-144">注: 今後、このプロパティを拡張して、より多くのシナリオをサポートすることができます。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-144">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="cf5e1-145">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5e1-145">registeredDateTime</span></span>|<span data-ttu-id="cf5e1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5e1-146">DateTimeOffset</span></span>      |<span data-ttu-id="cf5e1-147">リソースが PIM に登録されている日時を表します。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-147">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="cf5e1-148">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="cf5e1-148">registeredRoot</span></span>|<span data-ttu-id="cf5e1-149">String</span><span class="sxs-lookup"><span data-stu-id="cf5e1-149">String</span></span>      |<span data-ttu-id="cf5e1-150">PIM に登録されているリソースのルートスコープの externalId。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-150">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="cf5e1-151">ルートスコープには、親、親、または上位の先祖リソースを指定できます。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-151">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="cf5e1-152">Role割り当て数</span><span class="sxs-lookup"><span data-stu-id="cf5e1-152">roleAssignmentCount</span></span>|<span data-ttu-id="cf5e1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="cf5e1-153">Int32</span></span>      |<span data-ttu-id="cf5e1-154">省略可能。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-154">Optional.</span></span> <span data-ttu-id="cf5e1-155">指定したリソースのロール割り当ての数。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-155">The number of role assignments for the given resource.</span></span> <span data-ttu-id="cf5e1-156">プロパティを取得するには、クエリ`$select=roleAssignmentCount`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-156">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="cf5e1-157">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="cf5e1-157">roleDefinitionCount</span></span>|<span data-ttu-id="cf5e1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="cf5e1-158">Int32</span></span>      |<span data-ttu-id="cf5e1-159">省略可能。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-159">Optional.</span></span> <span data-ttu-id="cf5e1-160">指定したリソースのロール定義の数。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-160">The number of role definitions for the given resource.</span></span> <span data-ttu-id="cf5e1-161">プロパティを取得するには、クエリ`$select=roleDefinitionCount`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-161">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="cf5e1-162">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cf5e1-162">permissions</span></span>|[<span data-ttu-id="cf5e1-163">governancePermission</span><span class="sxs-lookup"><span data-stu-id="cf5e1-163">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="cf5e1-164">省略可能。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-164">Optional.</span></span> <span data-ttu-id="cf5e1-165">これは、リソースへの要求者のアクセスの状態を表します。プロパティを取得するには、クエリ`$select=permissions`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-165">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf5e1-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf5e1-166">Relationships</span></span>
| <span data-ttu-id="cf5e1-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf5e1-167">Relationship</span></span>   | <span data-ttu-id="cf5e1-168">型</span><span class="sxs-lookup"><span data-stu-id="cf5e1-168">Type</span></span>                                         |<span data-ttu-id="cf5e1-169">説明</span><span class="sxs-lookup"><span data-stu-id="cf5e1-169">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="cf5e1-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="cf5e1-170">roleAssignments</span></span> |<span data-ttu-id="cf5e1-171">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cf5e1-171">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="cf5e1-172">リソースのロール割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-172">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="cf5e1-173">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="cf5e1-173">roleDefinitions</span></span> |<span data-ttu-id="cf5e1-174">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cf5e1-174">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="cf5e1-175">リソースのロール日のコレクション。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-175">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="cf5e1-176">Rolerequests 要求</span><span class="sxs-lookup"><span data-stu-id="cf5e1-176">roleAssignmentRequests</span></span> |<span data-ttu-id="cf5e1-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cf5e1-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="cf5e1-178">リソースに対する役割の割り当て要求のコレクション。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-178">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="cf5e1-179">roleSettings</span><span class="sxs-lookup"><span data-stu-id="cf5e1-179">roleSettings</span></span> |<span data-ttu-id="cf5e1-180">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cf5e1-180">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="cf5e1-181">リソースのロール設定のコレクション。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-181">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="cf5e1-182">親行</span><span class="sxs-lookup"><span data-stu-id="cf5e1-182">parent</span></span>          |[<span data-ttu-id="cf5e1-183">governanceResource</span><span class="sxs-lookup"><span data-stu-id="cf5e1-183">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="cf5e1-184">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-184">Read-only.</span></span> <span data-ttu-id="cf5e1-185">親リソース。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-185">The parent resource.</span></span> <span data-ttu-id="cf5e1-186">シナリオ`pimforazurerbac`の場合は、リソースが属するサブスクリプションを表すことができます。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-186">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf5e1-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf5e1-187">JSON representation</span></span>

<span data-ttu-id="cf5e1-188">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf5e1-188">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "registeredRoot": "String",
  "roleAssignmentCount": 12356,
  "roleDefinitionCount": 12356,
  "permissions": {
    "@odata.type": "microsoft.graph.governancePermission"
  }
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
  "suppressions": []
}
-->
