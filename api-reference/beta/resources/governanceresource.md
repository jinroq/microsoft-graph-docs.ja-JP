---
title: governanceResource リソースの種類
description: 特権を持つユーザー情報管理 (PIM) で管理できるリソースを表します。 Azure のリソースでは、サブスクリプション、リソース グループ、およびなど、仮想マシン、SQL データベースなどのリソースとなります。
localization_priority: Normal
ms.openlocfilehash: 92a738350a47cc9eaf436382d020330fac89db1f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528558"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="f5aa6-104">governanceResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5aa6-104">governanceResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5aa6-105">特権を持つユーザー情報管理 (PIM) で管理できるリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-105">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="f5aa6-106">Azure のリソースでは、サブスクリプション、リソース グループ、およびなど、仮想マシン、SQL データベースなどのリソースとなります。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-106">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="f5aa6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5aa6-107">Methods</span></span>

| <span data-ttu-id="f5aa6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5aa6-108">Method</span></span>          | <span data-ttu-id="f5aa6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5aa6-109">Return Type</span></span> |<span data-ttu-id="f5aa6-110">説明</span><span class="sxs-lookup"><span data-stu-id="f5aa6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5aa6-111">List</span><span class="sxs-lookup"><span data-stu-id="f5aa6-111">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="f5aa6-112">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5aa6-112">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="f5aa6-113">リクエスターへのアクセス権を持つリソースの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-113">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="f5aa6-114">Get</span><span class="sxs-lookup"><span data-stu-id="f5aa6-114">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="f5aa6-115">governanceResource</span><span class="sxs-lookup"><span data-stu-id="f5aa6-115">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="f5aa6-116">Id で指定されたリソースのエンティティのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-116">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="f5aa6-117">REGISTER</span><span class="sxs-lookup"><span data-stu-id="f5aa6-117">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="f5aa6-118">アンマネージ Azure サブスクリプションまたは管理グループに PIM サービスを登録します。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-118">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="f5aa6-119">No `POST`、 `PUT`、 `PATCH`、`DELETE`でサポートされている`roleDefinitions`ここではエンティティのセットです。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-119">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="f5aa6-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5aa6-120">Properties</span></span>
| <span data-ttu-id="f5aa6-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5aa6-121">Property</span></span>          |<span data-ttu-id="f5aa6-122">型</span><span class="sxs-lookup"><span data-stu-id="f5aa6-122">Type</span></span>         |<span data-ttu-id="f5aa6-123">説明</span><span class="sxs-lookup"><span data-stu-id="f5aa6-123">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="f5aa6-124">id</span><span class="sxs-lookup"><span data-stu-id="f5aa6-124">id</span></span>                 |<span data-ttu-id="f5aa6-125">String</span><span class="sxs-lookup"><span data-stu-id="f5aa6-125">String</span></span>     |<span data-ttu-id="f5aa6-126">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-126">The id of the resource.</span></span> <span data-ttu-id="f5aa6-127">GUID 形式であります。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-127">It is in GUID format.</span></span>|
|<span data-ttu-id="f5aa6-128">externalId</span><span class="sxs-lookup"><span data-stu-id="f5aa6-128">externalId</span></span>           |<span data-ttu-id="f5aa6-129">String</span><span class="sxs-lookup"><span data-stu-id="f5aa6-129">String</span></span>   |<span data-ttu-id="f5aa6-130">外部システムで、元の id を表すリソースの外部の id です。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-130">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="f5aa6-131">たとえば、サブスクリプション リソースの外部 id には、「サブスクリプション/c14ae696-5e0c-4e5d-88cc-bef6637737ac」ができます。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-131">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="f5aa6-132">type</span><span class="sxs-lookup"><span data-stu-id="f5aa6-132">type</span></span>               |<span data-ttu-id="f5aa6-133">String</span><span class="sxs-lookup"><span data-stu-id="f5aa6-133">String</span></span>     |<span data-ttu-id="f5aa6-134">必須。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-134">Required.</span></span> <span data-ttu-id="f5aa6-135">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5aa6-135">Resource type.</span></span> <span data-ttu-id="f5aa6-136">たとえば、Azure のリソースの種類可能性があります「サブスクリプション」、「リソース グループ」、"Microsoft.Sql/server"など。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-136">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="f5aa6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f5aa6-137">displayName</span></span>        |<span data-ttu-id="f5aa6-138">String</span><span class="sxs-lookup"><span data-stu-id="f5aa6-138">String</span></span>     |<span data-ttu-id="f5aa6-139">リソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-139">The display name of the resource.</span></span>|
|<span data-ttu-id="f5aa6-140">status</span><span class="sxs-lookup"><span data-stu-id="f5aa6-140">status</span></span>             |<span data-ttu-id="f5aa6-141">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f5aa6-141">String</span></span>     |<span data-ttu-id="f5aa6-142">特定のリソースの状態です。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-142">The status of a given resource.</span></span> <span data-ttu-id="f5aa6-143">たとえば、リソースをロックするかどうかを表すことが、(値: `Active` / `Locked`)。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-143">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="f5aa6-144">メモ: このプロパティ拡張することが、将来的に複数のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-144">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="f5aa6-145">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="f5aa6-145">registeredDateTime</span></span>|<span data-ttu-id="f5aa6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5aa6-146">DateTimeOffset</span></span>      |<span data-ttu-id="f5aa6-147">PIM にリソースを登録するときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-147">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="f5aa6-148">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="f5aa6-148">registeredRoot</span></span>|<span data-ttu-id="f5aa6-149">String</span><span class="sxs-lookup"><span data-stu-id="f5aa6-149">String</span></span>      |<span data-ttu-id="f5aa6-150">PIM に登録されているリソースのルート スコープの externalId です。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-150">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="f5aa6-151">ルート スコープには、親、親の親、または先祖の高いリソースができます。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-151">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="f5aa6-152">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="f5aa6-152">roleAssignmentCount</span></span>|<span data-ttu-id="f5aa6-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f5aa6-153">Int32</span></span>      |<span data-ttu-id="f5aa6-154">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-154">Optional.</span></span> <span data-ttu-id="f5aa6-155">特定のリソースに対するロールの割り当ての数です。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-155">The number of role assignments for the given resource.</span></span> <span data-ttu-id="f5aa6-156">プロパティを取得するには、明示的に使用をしてください。`$select=roleAssignmentCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-156">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="f5aa6-157">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="f5aa6-157">roleDefinitionCount</span></span>|<span data-ttu-id="f5aa6-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f5aa6-158">Int32</span></span>      |<span data-ttu-id="f5aa6-159">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-159">Optional.</span></span> <span data-ttu-id="f5aa6-160">指定されたリソースの役割の定義の数です。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-160">The number of role definitions for the given resource.</span></span> <span data-ttu-id="f5aa6-161">プロパティを取得するには、明示的に使用をしてください。`$select=roleDefinitionCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-161">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="f5aa6-162">permissions</span><span class="sxs-lookup"><span data-stu-id="f5aa6-162">permissions</span></span>|[<span data-ttu-id="f5aa6-163">governancePermission</span><span class="sxs-lookup"><span data-stu-id="f5aa6-163">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="f5aa6-164">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-164">Optional.</span></span> <span data-ttu-id="f5aa6-165">リソースへのアクセスの要求元の状態を表します。プロパティを取得するには、明示的に使用をしてください。`$select=permissions`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-165">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5aa6-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5aa6-166">Relationships</span></span>
| <span data-ttu-id="f5aa6-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5aa6-167">Relationship</span></span>   | <span data-ttu-id="f5aa6-168">型</span><span class="sxs-lookup"><span data-stu-id="f5aa6-168">Type</span></span>                                         |<span data-ttu-id="f5aa6-169">説明</span><span class="sxs-lookup"><span data-stu-id="f5aa6-169">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="f5aa6-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="f5aa6-170">roleAssignments</span></span> |<span data-ttu-id="f5aa6-171">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5aa6-171">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="f5aa6-172">リソースに対するロールの割り当てのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-172">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="f5aa6-173">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="f5aa6-173">roleDefinitions</span></span> |<span data-ttu-id="f5aa6-174">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5aa6-174">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="f5aa6-175">リソースのロール定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-175">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="f5aa6-176">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f5aa6-176">roleAssignmentRequests</span></span> |<span data-ttu-id="f5aa6-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5aa6-177">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="f5aa6-178">リソースの役割の割り当て要求のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-178">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="f5aa6-179">roleSettings</span><span class="sxs-lookup"><span data-stu-id="f5aa6-179">roleSettings</span></span> |<span data-ttu-id="f5aa6-180">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5aa6-180">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="f5aa6-181">リソースのロールの設定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-181">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="f5aa6-182">Parent</span><span class="sxs-lookup"><span data-stu-id="f5aa6-182">parent</span></span>          |[<span data-ttu-id="f5aa6-183">governanceResource</span><span class="sxs-lookup"><span data-stu-id="f5aa6-183">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="f5aa6-184">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-184">Read-only.</span></span> <span data-ttu-id="f5aa6-185">親リソースです。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-185">The parent resource.</span></span> <span data-ttu-id="f5aa6-186">`pimforazurerbac`シナリオでは、サブスクリプションに属しているリソースを表すことができます。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-186">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5aa6-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5aa6-187">JSON representation</span></span>

<span data-ttu-id="f5aa6-188">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5aa6-188">The following is a JSON representation of the resource.</span></span>

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
