---
title: governanceResource リソースの種類
description: 特権を持つユーザー情報管理 (PIM) で管理できるリソースを表します。 Azure のリソースでは、サブスクリプション、リソース グループ、およびなど、仮想マシン、SQL データベースなどのリソースとなります。
ms.openlocfilehash: 6a048680c3b9bb614287e764d547a20bd09b5d25
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191131"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="65ce2-104">governanceResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65ce2-104">governanceResource resource type</span></span>

> <span data-ttu-id="65ce2-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65ce2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65ce2-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65ce2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65ce2-107">特権を持つユーザー情報管理 (PIM) で管理できるリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="65ce2-107">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="65ce2-108">Azure のリソースでは、サブスクリプション、リソース グループ、およびなど、仮想マシン、SQL データベースなどのリソースとなります。</span><span class="sxs-lookup"><span data-stu-id="65ce2-108">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="65ce2-109">Methods</span><span class="sxs-lookup"><span data-stu-id="65ce2-109">Methods</span></span>

| <span data-ttu-id="65ce2-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="65ce2-110">Method</span></span>          | <span data-ttu-id="65ce2-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="65ce2-111">Return Type</span></span> |<span data-ttu-id="65ce2-112">説明</span><span class="sxs-lookup"><span data-stu-id="65ce2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65ce2-113">List</span><span class="sxs-lookup"><span data-stu-id="65ce2-113">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="65ce2-114">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65ce2-114">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="65ce2-115">リクエスターへのアクセス権を持つリソースの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="65ce2-115">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="65ce2-116">Get</span><span class="sxs-lookup"><span data-stu-id="65ce2-116">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="65ce2-117">governanceResource</span><span class="sxs-lookup"><span data-stu-id="65ce2-117">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="65ce2-118">Id で指定されたリソースのエンティティのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65ce2-118">Read properties and relationships of a resource entity specified by id.</span></span>|
|[<span data-ttu-id="65ce2-119">登録</span><span class="sxs-lookup"><span data-stu-id="65ce2-119">Register</span></span>](../api/governanceresource-register.md) | |<span data-ttu-id="65ce2-120">アンマネージ Azure サブスクリプションまたは管理グループに PIM サービスを登録します。</span><span class="sxs-lookup"><span data-stu-id="65ce2-120">Register an unmanaged Azure subscription or management group to PIM service.</span></span> |

<span data-ttu-id="65ce2-121">No `POST`、 `PUT`、 `PATCH`、`DELETE`でサポートされている`roleDefinitions`ここではエンティティのセットです。</span><span class="sxs-lookup"><span data-stu-id="65ce2-121">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="65ce2-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65ce2-122">Properties</span></span>
| <span data-ttu-id="65ce2-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65ce2-123">Property</span></span>          |<span data-ttu-id="65ce2-124">種類</span><span class="sxs-lookup"><span data-stu-id="65ce2-124">Type</span></span>         |<span data-ttu-id="65ce2-125">説明</span><span class="sxs-lookup"><span data-stu-id="65ce2-125">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="65ce2-126">id</span><span class="sxs-lookup"><span data-stu-id="65ce2-126">id</span></span>                 |<span data-ttu-id="65ce2-127">String</span><span class="sxs-lookup"><span data-stu-id="65ce2-127">String</span></span>     |<span data-ttu-id="65ce2-128">リソースの id です。</span><span class="sxs-lookup"><span data-stu-id="65ce2-128">The id of the resource.</span></span> <span data-ttu-id="65ce2-129">GUID 形式であります。</span><span class="sxs-lookup"><span data-stu-id="65ce2-129">It is in GUID format.</span></span>|
|<span data-ttu-id="65ce2-130">externalId</span><span class="sxs-lookup"><span data-stu-id="65ce2-130">externalId</span></span>           |<span data-ttu-id="65ce2-131">String</span><span class="sxs-lookup"><span data-stu-id="65ce2-131">String</span></span>   |<span data-ttu-id="65ce2-132">外部システムで、元の id を表すリソースの外部の id です。</span><span class="sxs-lookup"><span data-stu-id="65ce2-132">The external id of the resource, representing its original id in the external system.</span></span> <span data-ttu-id="65ce2-133">たとえば、サブスクリプション リソースの外部 id には、「サブスクリプション/c14ae696-5e0c-4e5d-88cc-bef6637737ac」ができます。</span><span class="sxs-lookup"><span data-stu-id="65ce2-133">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="65ce2-134">type</span><span class="sxs-lookup"><span data-stu-id="65ce2-134">type</span></span>               |<span data-ttu-id="65ce2-135">String</span><span class="sxs-lookup"><span data-stu-id="65ce2-135">String</span></span>     |<span data-ttu-id="65ce2-136">必須。</span><span class="sxs-lookup"><span data-stu-id="65ce2-136">Required.</span></span> <span data-ttu-id="65ce2-137">リソースの種類。</span><span class="sxs-lookup"><span data-stu-id="65ce2-137">Resource type.</span></span> <span data-ttu-id="65ce2-138">たとえば、Azure のリソースの種類可能性があります「サブスクリプション」、「リソース グループ」、"Microsoft.Sql/server"など。</span><span class="sxs-lookup"><span data-stu-id="65ce2-138">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="65ce2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="65ce2-139">displayName</span></span>        |<span data-ttu-id="65ce2-140">String</span><span class="sxs-lookup"><span data-stu-id="65ce2-140">String</span></span>     |<span data-ttu-id="65ce2-141">リソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="65ce2-141">The display name of the resource.</span></span>|
|<span data-ttu-id="65ce2-142">status</span><span class="sxs-lookup"><span data-stu-id="65ce2-142">status</span></span>             |<span data-ttu-id="65ce2-143">String</span><span class="sxs-lookup"><span data-stu-id="65ce2-143">String</span></span>     |<span data-ttu-id="65ce2-144">特定のリソースの状態です。</span><span class="sxs-lookup"><span data-stu-id="65ce2-144">The status of a given resource.</span></span> <span data-ttu-id="65ce2-145">たとえば、リソースをロックするかどうかを表すことが、(値: `Active` / `Locked`)。</span><span class="sxs-lookup"><span data-stu-id="65ce2-145">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="65ce2-146">メモ: このプロパティ拡張することが、将来的に複数のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="65ce2-146">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="65ce2-147">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="65ce2-147">registeredDateTime</span></span>|<span data-ttu-id="65ce2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65ce2-148">DateTimeOffset</span></span>      |<span data-ttu-id="65ce2-149">PIM にリソースを登録するときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="65ce2-149">Represents the date time when the resource is registered in PIM.</span></span>|
|<span data-ttu-id="65ce2-150">registeredRoot</span><span class="sxs-lookup"><span data-stu-id="65ce2-150">registeredRoot</span></span>|<span data-ttu-id="65ce2-151">String</span><span class="sxs-lookup"><span data-stu-id="65ce2-151">String</span></span>      |<span data-ttu-id="65ce2-152">PIM に登録されているリソースのルート スコープの externalId です。</span><span class="sxs-lookup"><span data-stu-id="65ce2-152">The externalId of the resource's root scope that is registered in PIM.</span></span> <span data-ttu-id="65ce2-153">ルート スコープには、親、親の親、または先祖の高いリソースができます。</span><span class="sxs-lookup"><span data-stu-id="65ce2-153">The root scope can be the parent, grandparent, or higher ancestor resources.</span></span>|
|<span data-ttu-id="65ce2-154">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="65ce2-154">roleAssignmentCount</span></span>|<span data-ttu-id="65ce2-155">Int32</span><span class="sxs-lookup"><span data-stu-id="65ce2-155">Int32</span></span>      |<span data-ttu-id="65ce2-156">省略可能。</span><span class="sxs-lookup"><span data-stu-id="65ce2-156">Optional.</span></span> <span data-ttu-id="65ce2-157">特定のリソースに対するロールの割り当ての数です。</span><span class="sxs-lookup"><span data-stu-id="65ce2-157">The number of role assignments for the given resource.</span></span> <span data-ttu-id="65ce2-158">プロパティを取得するには、明示的に使用をしてください。`$select=roleAssignmentCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="65ce2-158">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="65ce2-159">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="65ce2-159">roleDefinitionCount</span></span>|<span data-ttu-id="65ce2-160">Int32</span><span class="sxs-lookup"><span data-stu-id="65ce2-160">Int32</span></span>      |<span data-ttu-id="65ce2-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="65ce2-161">Optional.</span></span> <span data-ttu-id="65ce2-162">指定されたリソースの役割の定義の数です。</span><span class="sxs-lookup"><span data-stu-id="65ce2-162">The number of role definitions for the given resource.</span></span> <span data-ttu-id="65ce2-163">プロパティを取得するには、明示的に使用をしてください。`$select=roleDefinitionCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="65ce2-163">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="65ce2-164">permissions</span><span class="sxs-lookup"><span data-stu-id="65ce2-164">permissions</span></span>|[<span data-ttu-id="65ce2-165">governancePermission</span><span class="sxs-lookup"><span data-stu-id="65ce2-165">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="65ce2-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="65ce2-166">Optional.</span></span> <span data-ttu-id="65ce2-167">リソースへのアクセスの要求元の状態を表します。プロパティを取得するには、明示的に使用をしてください。`$select=permissions`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="65ce2-167">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65ce2-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65ce2-168">Relationships</span></span>
| <span data-ttu-id="65ce2-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65ce2-169">Relationship</span></span>   | <span data-ttu-id="65ce2-170">型</span><span class="sxs-lookup"><span data-stu-id="65ce2-170">Type</span></span>                                         |<span data-ttu-id="65ce2-171">説明</span><span class="sxs-lookup"><span data-stu-id="65ce2-171">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="65ce2-172">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="65ce2-172">roleAssignments</span></span> |<span data-ttu-id="65ce2-173">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65ce2-173">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="65ce2-174">リソースに対するロールの割り当てのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="65ce2-174">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="65ce2-175">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="65ce2-175">roleDefinitions</span></span> |<span data-ttu-id="65ce2-176">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65ce2-176">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="65ce2-177">リソースのロール定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="65ce2-177">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="65ce2-178">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="65ce2-178">roleAssignmentRequests</span></span> |<span data-ttu-id="65ce2-179">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65ce2-179">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="65ce2-180">リソースの役割の割り当て要求のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="65ce2-180">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="65ce2-181">roleSettings</span><span class="sxs-lookup"><span data-stu-id="65ce2-181">roleSettings</span></span> |<span data-ttu-id="65ce2-182">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65ce2-182">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="65ce2-183">リソースのロールの設定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="65ce2-183">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="65ce2-184">親</span><span class="sxs-lookup"><span data-stu-id="65ce2-184">parent</span></span>          |[<span data-ttu-id="65ce2-185">governanceResource</span><span class="sxs-lookup"><span data-stu-id="65ce2-185">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="65ce2-186">取得のみ可能な値です。</span><span class="sxs-lookup"><span data-stu-id="65ce2-186">Read-only.</span></span> <span data-ttu-id="65ce2-187">親リソースです。</span><span class="sxs-lookup"><span data-stu-id="65ce2-187">The parent resource.</span></span> <span data-ttu-id="65ce2-188">`pimforazurerbac`シナリオでは、サブスクリプションに属しているリソースを表すことができます。</span><span class="sxs-lookup"><span data-stu-id="65ce2-188">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65ce2-189">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65ce2-189">JSON representation</span></span>

<span data-ttu-id="65ce2-190">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65ce2-190">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
