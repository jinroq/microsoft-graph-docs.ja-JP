---
title: governanceRoleDefinition リソースの種類
description: 役割の定義を表します。 Azure のリソースの所有者、閲覧者、投稿者など、Azure の RBAC の役割を表すことができます。
ms.openlocfilehash: 057d74276b41abad47eb60ce48a99f1160c401ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068113"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="0cd6b-104">governanceRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cd6b-104">governanceRoleDefinition resource type</span></span>

> <span data-ttu-id="0cd6b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cd6b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-106">Use of these APIs in production applications is not supported.</span></span> 


<span data-ttu-id="0cd6b-107">役割の定義を表します。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-107">Represents the role definitions.</span></span> <span data-ttu-id="0cd6b-108">Azure のリソースの所有者、閲覧者、投稿者など、Azure の RBAC の役割を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-108">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="0cd6b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cd6b-109">Methods</span></span>

| <span data-ttu-id="0cd6b-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cd6b-110">Method</span></span>          | <span data-ttu-id="0cd6b-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0cd6b-111">Return Type</span></span> |<span data-ttu-id="0cd6b-112">説明</span><span class="sxs-lookup"><span data-stu-id="0cd6b-112">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="0cd6b-113">List</span><span class="sxs-lookup"><span data-stu-id="0cd6b-113">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="0cd6b-114">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0cd6b-114">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="0cd6b-115">リソースの役割の定義の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-115">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="0cd6b-116">Get</span><span class="sxs-lookup"><span data-stu-id="0cd6b-116">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="0cd6b-117">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0cd6b-117">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="0cd6b-118">Id で指定されたロールの定義のエンティティのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-118">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="0cd6b-119">No `POST`、 `PUT`、 `PATCH`、`DELETE`でサポートされています`roleDefinitions`ここではエンティティのセットです。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-119">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="0cd6b-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cd6b-120">Properties</span></span>
| <span data-ttu-id="0cd6b-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cd6b-121">Property</span></span>  | <span data-ttu-id="0cd6b-122">型</span><span class="sxs-lookup"><span data-stu-id="0cd6b-122">Type</span></span>      |<span data-ttu-id="0cd6b-123">説明</span><span class="sxs-lookup"><span data-stu-id="0cd6b-123">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="0cd6b-124">id</span><span class="sxs-lookup"><span data-stu-id="0cd6b-124">id</span></span>         |<span data-ttu-id="0cd6b-125">String</span><span class="sxs-lookup"><span data-stu-id="0cd6b-125">String</span></span>     |<span data-ttu-id="0cd6b-126">役割の定義の id です。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-126">The id of the role definition.</span></span> |
|<span data-ttu-id="0cd6b-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="0cd6b-127">resourceId</span></span> |<span data-ttu-id="0cd6b-128">String</span><span class="sxs-lookup"><span data-stu-id="0cd6b-128">String</span></span>     |<span data-ttu-id="0cd6b-129">必須。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-129">Required.</span></span> <span data-ttu-id="0cd6b-130">役割の定義に関連付けられているリソースの id です。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-130">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="0cd6b-131">externalId</span><span class="sxs-lookup"><span data-stu-id="0cd6b-131">externalId</span></span>   |<span data-ttu-id="0cd6b-132">String</span><span class="sxs-lookup"><span data-stu-id="0cd6b-132">String</span></span>     |<span data-ttu-id="0cd6b-133">役割の定義の外部の id です。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-133">The external id of the role definition.</span></span>|
|<span data-ttu-id="0cd6b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0cd6b-134">displayName</span></span>|<span data-ttu-id="0cd6b-135">String</span><span class="sxs-lookup"><span data-stu-id="0cd6b-135">String</span></span>     |<span data-ttu-id="0cd6b-136">役割の定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-136">The display name of the role definition.</span></span>|
|<span data-ttu-id="0cd6b-137">subjectCount</span><span class="sxs-lookup"><span data-stu-id="0cd6b-137">subjectCount</span></span>|<span data-ttu-id="0cd6b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0cd6b-138">Int32</span></span>     |<span data-ttu-id="0cd6b-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-139">Optional.</span></span> <span data-ttu-id="0cd6b-140">ロールに割り当てられている被験者の数です。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-140">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="0cd6b-141">リソースへのアクセスの要求元の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-141">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="0cd6b-142">プロパティを取得するには、明示的に使用をしてください。`$select=subjectCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-142">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="0cd6b-143">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="0cd6b-143">eligibleAssignmentCount</span></span>|<span data-ttu-id="0cd6b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0cd6b-144">Int32</span></span>|<span data-ttu-id="0cd6b-145">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-145">Optional.</span></span> <span data-ttu-id="0cd6b-146">役割の定義に関連付けられている対象のロールの割り当ての数です。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-146">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="0cd6b-147">プロパティを取得するには、明示的に使用をしてください。`$select=eligibleAssignmentCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-147">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="0cd6b-148">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="0cd6b-148">activeAssignmentCount</span></span>|<span data-ttu-id="0cd6b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0cd6b-149">Int32</span></span>    |<span data-ttu-id="0cd6b-150">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-150">Optional.</span></span> <span data-ttu-id="0cd6b-151">役割の定義に関連付けられているアクティブなロールの割り当ての数です。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-151">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="0cd6b-152">プロパティを取得するには、明示的に使用をしてください。`$select=activeAssignmentCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-152">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="0cd6b-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0cd6b-153">Relationships</span></span>
| <span data-ttu-id="0cd6b-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0cd6b-154">Relationship</span></span> | <span data-ttu-id="0cd6b-155">型</span><span class="sxs-lookup"><span data-stu-id="0cd6b-155">Type</span></span>   |<span data-ttu-id="0cd6b-156">説明</span><span class="sxs-lookup"><span data-stu-id="0cd6b-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cd6b-157">リソース</span><span class="sxs-lookup"><span data-stu-id="0cd6b-157">resource</span></span>|[<span data-ttu-id="0cd6b-158">governanceResource</span><span class="sxs-lookup"><span data-stu-id="0cd6b-158">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="0cd6b-159">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-159">Read-only.</span></span> <span data-ttu-id="0cd6b-160">役割の定義に関連付けられているリソースです。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-160">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="0cd6b-161">roleSetting</span><span class="sxs-lookup"><span data-stu-id="0cd6b-161">roleSetting</span></span>|[<span data-ttu-id="0cd6b-162">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="0cd6b-162">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="0cd6b-163">役割の定義に関連付けられている役割の設定をします。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-163">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cd6b-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cd6b-164">JSON representation</span></span>

<span data-ttu-id="0cd6b-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0cd6b-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->