---
title: governanceResource リソースの種類
description: 特権を持つユーザー情報管理 (PIM) で管理できるリソースを表します。 Azure のリソースでは、サブスクリプション、リソース グループ、およびなど、仮想マシン、SQL データベースなどのリソースとなります。
ms.openlocfilehash: 9e47f1295f9498796d51414a0a97acbe51fe1aae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070755"
---
# <a name="governanceresource-resource-type"></a><span data-ttu-id="1991c-104">governanceResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1991c-104">governanceResource resource type</span></span>

> <span data-ttu-id="1991c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1991c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1991c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1991c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1991c-107">特権を持つユーザー情報管理 (PIM) で管理できるリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="1991c-107">Represents resources that could be managed by Privileged Identity Management (PIM).</span></span> <span data-ttu-id="1991c-108">Azure のリソースでは、サブスクリプション、リソース グループ、およびなど、仮想マシン、SQL データベースなどのリソースとなります。</span><span class="sxs-lookup"><span data-stu-id="1991c-108">For Azure resources, it can be a subscription, a resource group, and a resource such as a virtual machine, a SQL database, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="1991c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1991c-109">Methods</span></span>

| <span data-ttu-id="1991c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="1991c-110">Method</span></span>          | <span data-ttu-id="1991c-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1991c-111">Return Type</span></span> |<span data-ttu-id="1991c-112">説明</span><span class="sxs-lookup"><span data-stu-id="1991c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1991c-113">List</span><span class="sxs-lookup"><span data-stu-id="1991c-113">List</span></span>](../api/governanceresource-list.md) | <span data-ttu-id="1991c-114">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1991c-114">[governanceResource](../resources/governanceresource.md) collection</span></span>|<span data-ttu-id="1991c-115">リクエスターへのアクセス権を持つリソースの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="1991c-115">List a collection of resources the requestor has access to.</span></span>|
|[<span data-ttu-id="1991c-116">Get</span><span class="sxs-lookup"><span data-stu-id="1991c-116">Get</span></span>](../api/governanceresource-get.md) | [<span data-ttu-id="1991c-117">governanceResource</span><span class="sxs-lookup"><span data-stu-id="1991c-117">governanceResource</span></span>](../resources/governanceresource.md) |<span data-ttu-id="1991c-118">Id で指定されたリソースのエンティティのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1991c-118">Read properties and relationships of a resource entity specified by id.</span></span>|

<span data-ttu-id="1991c-119">No `POST`、 `PUT`、 `PATCH`、`DELETE`でサポートされている`roleDefinitions`ここではエンティティのセットです。</span><span class="sxs-lookup"><span data-stu-id="1991c-119">No `POST`, `PUT`, `PATCH`, `DELETE` are supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="1991c-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1991c-120">Properties</span></span>
| <span data-ttu-id="1991c-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1991c-121">Property</span></span>          |<span data-ttu-id="1991c-122">型</span><span class="sxs-lookup"><span data-stu-id="1991c-122">Type</span></span>         |<span data-ttu-id="1991c-123">説明</span><span class="sxs-lookup"><span data-stu-id="1991c-123">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="1991c-124">id</span><span class="sxs-lookup"><span data-stu-id="1991c-124">id</span></span>                 |<span data-ttu-id="1991c-125">String</span><span class="sxs-lookup"><span data-stu-id="1991c-125">String</span></span>     |<span data-ttu-id="1991c-126">リソースの id です。</span><span class="sxs-lookup"><span data-stu-id="1991c-126">The id of the resource.</span></span> <span data-ttu-id="1991c-127">GUID 形式であります。</span><span class="sxs-lookup"><span data-stu-id="1991c-127">It is in GUID format.</span></span>|
|<span data-ttu-id="1991c-128">externalId</span><span class="sxs-lookup"><span data-stu-id="1991c-128">externalId</span></span>           |<span data-ttu-id="1991c-129">String</span><span class="sxs-lookup"><span data-stu-id="1991c-129">String</span></span>   |<span data-ttu-id="1991c-130">外部データベースの元の id を表すリソースの外部の id です。</span><span class="sxs-lookup"><span data-stu-id="1991c-130">The external id of the resource, representing its original id in the external database.</span></span> <span data-ttu-id="1991c-131">たとえば、サブスクリプション リソースの外部 id には、「サブスクリプション/c14ae696-5e0c-4e5d-88cc-bef6637737ac」ができます。</span><span class="sxs-lookup"><span data-stu-id="1991c-131">For example, a subscription resource's external id can be "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac".</span></span> |
|<span data-ttu-id="1991c-132">type</span><span class="sxs-lookup"><span data-stu-id="1991c-132">type</span></span>               |<span data-ttu-id="1991c-133">String</span><span class="sxs-lookup"><span data-stu-id="1991c-133">String</span></span>     |<span data-ttu-id="1991c-134">必須。</span><span class="sxs-lookup"><span data-stu-id="1991c-134">Required.</span></span> <span data-ttu-id="1991c-135">リソースの種類。</span><span class="sxs-lookup"><span data-stu-id="1991c-135">Resource type.</span></span> <span data-ttu-id="1991c-136">たとえば、Azure のリソースの種類可能性があります「サブスクリプション」、「リソース グループ」、"Microsoft.Sql/server"など。</span><span class="sxs-lookup"><span data-stu-id="1991c-136">For example, for Azure resources, the type could be "Subscription", "ResourceGroup", "Microsoft.Sql/server", etc.</span></span>|
|<span data-ttu-id="1991c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1991c-137">displayName</span></span>        |<span data-ttu-id="1991c-138">String</span><span class="sxs-lookup"><span data-stu-id="1991c-138">String</span></span>     |<span data-ttu-id="1991c-139">リソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="1991c-139">The display name of the resource.</span></span>|
|<span data-ttu-id="1991c-140">status</span><span class="sxs-lookup"><span data-stu-id="1991c-140">status</span></span>             |<span data-ttu-id="1991c-141">String</span><span class="sxs-lookup"><span data-stu-id="1991c-141">String</span></span>     |<span data-ttu-id="1991c-142">特定のリソースの状態です。</span><span class="sxs-lookup"><span data-stu-id="1991c-142">The status of a given resource.</span></span> <span data-ttu-id="1991c-143">たとえば、リソースをロックするかどうかを表すことが、(値: `Active` / `Locked`)。</span><span class="sxs-lookup"><span data-stu-id="1991c-143">For example, it could represent whether the resource is locked or not (values: `Active`/`Locked`).</span></span> <span data-ttu-id="1991c-144">メモ: このプロパティ拡張することが、将来的に複数のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="1991c-144">Note: This property may be extended in the future to support more scenarios.</span></span>|
|<span data-ttu-id="1991c-145">onboardDateTime</span><span class="sxs-lookup"><span data-stu-id="1991c-145">onboardDateTime</span></span>|<span data-ttu-id="1991c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1991c-146">DateTimeOffset</span></span>      |<span data-ttu-id="1991c-147">PIM で管理するためのリソースの開始時に日時を表します。</span><span class="sxs-lookup"><span data-stu-id="1991c-147">It represents the date time when the resource starts to be managed by PIM.</span></span>|
|<span data-ttu-id="1991c-148">roleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="1991c-148">roleAssignmentCount</span></span>|<span data-ttu-id="1991c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1991c-149">Int32</span></span>      |<span data-ttu-id="1991c-150">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1991c-150">Optional.</span></span> <span data-ttu-id="1991c-151">特定のリソースに対するロールの割り当ての数です。</span><span class="sxs-lookup"><span data-stu-id="1991c-151">The number of role assignments for the given resource.</span></span> <span data-ttu-id="1991c-152">プロパティを取得するには、明示的に使用をしてください。`$select=roleAssignmentCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="1991c-152">To get the property, please explictly use `$select=roleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="1991c-153">roleDefinitionCount</span><span class="sxs-lookup"><span data-stu-id="1991c-153">roleDefinitionCount</span></span>|<span data-ttu-id="1991c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1991c-154">Int32</span></span>      |<span data-ttu-id="1991c-155">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1991c-155">Optional.</span></span> <span data-ttu-id="1991c-156">指定されたリソースの役割の定義の数です。</span><span class="sxs-lookup"><span data-stu-id="1991c-156">The number of role definitions for the given resource.</span></span> <span data-ttu-id="1991c-157">プロパティを取得するには、明示的に使用をしてください。`$select=roleDefinitionCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="1991c-157">To get the property, please explictly use `$select=roleDefinitionCount` in the query.</span></span>|
|<span data-ttu-id="1991c-158">permissions</span><span class="sxs-lookup"><span data-stu-id="1991c-158">permissions</span></span>|[<span data-ttu-id="1991c-159">governancePermission</span><span class="sxs-lookup"><span data-stu-id="1991c-159">governancePermission</span></span>](../resources/governancepermission.md)      |<span data-ttu-id="1991c-160">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1991c-160">Optional.</span></span> <span data-ttu-id="1991c-161">リソースへのアクセスの要求元の状態を表します。プロパティを取得するには、明示的に使用をしてください。`$select=permissions`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="1991c-161">It represents the status of the requestor's access to the resource.To get the property, please explictly use `$select=permissions` in the query.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1991c-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1991c-162">Relationships</span></span>
| <span data-ttu-id="1991c-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1991c-163">Relationship</span></span>   | <span data-ttu-id="1991c-164">型</span><span class="sxs-lookup"><span data-stu-id="1991c-164">Type</span></span>                                         |<span data-ttu-id="1991c-165">説明</span><span class="sxs-lookup"><span data-stu-id="1991c-165">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="1991c-166">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="1991c-166">roleAssignments</span></span> |<span data-ttu-id="1991c-167">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1991c-167">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="1991c-168">リソースに対するロールの割り当てのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1991c-168">The collection of role assignments for the resource.</span></span>|
|<span data-ttu-id="1991c-169">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="1991c-169">roleDefinitions</span></span> |<span data-ttu-id="1991c-170">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1991c-170">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="1991c-171">リソースのロール定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1991c-171">The collection of role defintions for the resource.</span></span>|
|<span data-ttu-id="1991c-172">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="1991c-172">roleAssignmentRequests</span></span> |<span data-ttu-id="1991c-173">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1991c-173">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="1991c-174">リソースの役割の割り当て要求のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1991c-174">The collection of role assignment requests for the resource.</span></span>|
|<span data-ttu-id="1991c-175">roleSettings</span><span class="sxs-lookup"><span data-stu-id="1991c-175">roleSettings</span></span> |<span data-ttu-id="1991c-176">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1991c-176">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="1991c-177">リソースのロールの設定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1991c-177">The collection of role settings for the resource.</span></span>|
|<span data-ttu-id="1991c-178">親</span><span class="sxs-lookup"><span data-stu-id="1991c-178">parent</span></span>          |[<span data-ttu-id="1991c-179">governanceResource</span><span class="sxs-lookup"><span data-stu-id="1991c-179">governanceResource</span></span>](../resources/governanceresource.md)           |<span data-ttu-id="1991c-180">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1991c-180">Read-only.</span></span> <span data-ttu-id="1991c-181">親リソースです。</span><span class="sxs-lookup"><span data-stu-id="1991c-181">The parent resource.</span></span> <span data-ttu-id="1991c-182">`pimforazurerbac`シナリオでは、サブスクリプションに属しているリソースを表すことができます。</span><span class="sxs-lookup"><span data-stu-id="1991c-182">for `pimforazurerbac` scenario, it can represent the subscription the resource belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1991c-183">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1991c-183">JSON representation</span></span>

<span data-ttu-id="1991c-184">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1991c-184">Here is a JSON representation of the resource.</span></span>

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
  "status": "String"
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