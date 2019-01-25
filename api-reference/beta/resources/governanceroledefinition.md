---
title: governanceRoleDefinition リソースの種類
description: 役割の定義を表します。 Azure のリソースの所有者、閲覧者、投稿者など、Azure の RBAC の役割を表すことができます。
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528642"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="656f3-104">governanceRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="656f3-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="656f3-105">役割の定義を表します。</span><span class="sxs-lookup"><span data-stu-id="656f3-105">Represents the role definitions.</span></span> <span data-ttu-id="656f3-106">Azure のリソースの所有者、閲覧者、投稿者など、Azure の RBAC の役割を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="656f3-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="656f3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="656f3-107">Methods</span></span>

| <span data-ttu-id="656f3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="656f3-108">Method</span></span>          | <span data-ttu-id="656f3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="656f3-109">Return Type</span></span> |<span data-ttu-id="656f3-110">説明</span><span class="sxs-lookup"><span data-stu-id="656f3-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="656f3-111">List</span><span class="sxs-lookup"><span data-stu-id="656f3-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="656f3-112">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="656f3-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="656f3-113">リソースの役割の定義の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="656f3-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="656f3-114">Get</span><span class="sxs-lookup"><span data-stu-id="656f3-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="656f3-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="656f3-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="656f3-116">Id で指定されたロールの定義のエンティティのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="656f3-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="656f3-117">No `POST`、 `PUT`、 `PATCH`、`DELETE`でサポートされています`roleDefinitions`ここではエンティティのセットです。</span><span class="sxs-lookup"><span data-stu-id="656f3-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="656f3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="656f3-118">Properties</span></span>
| <span data-ttu-id="656f3-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="656f3-119">Property</span></span>  | <span data-ttu-id="656f3-120">型</span><span class="sxs-lookup"><span data-stu-id="656f3-120">Type</span></span>      |<span data-ttu-id="656f3-121">説明</span><span class="sxs-lookup"><span data-stu-id="656f3-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="656f3-122">id</span><span class="sxs-lookup"><span data-stu-id="656f3-122">id</span></span>         |<span data-ttu-id="656f3-123">文字列</span><span class="sxs-lookup"><span data-stu-id="656f3-123">String</span></span>     |<span data-ttu-id="656f3-124">役割の定義の id です。</span><span class="sxs-lookup"><span data-stu-id="656f3-124">The id of the role definition.</span></span> |
|<span data-ttu-id="656f3-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="656f3-125">resourceId</span></span> |<span data-ttu-id="656f3-126">String</span><span class="sxs-lookup"><span data-stu-id="656f3-126">String</span></span>     |<span data-ttu-id="656f3-127">必須。</span><span class="sxs-lookup"><span data-stu-id="656f3-127">Required.</span></span> <span data-ttu-id="656f3-128">役割の定義に関連付けられているリソースの id です。</span><span class="sxs-lookup"><span data-stu-id="656f3-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="656f3-129">externalId</span><span class="sxs-lookup"><span data-stu-id="656f3-129">externalId</span></span>   |<span data-ttu-id="656f3-130">String</span><span class="sxs-lookup"><span data-stu-id="656f3-130">String</span></span>     |<span data-ttu-id="656f3-131">役割の定義の外部の id です。</span><span class="sxs-lookup"><span data-stu-id="656f3-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="656f3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="656f3-132">displayName</span></span>|<span data-ttu-id="656f3-133">String</span><span class="sxs-lookup"><span data-stu-id="656f3-133">String</span></span>     |<span data-ttu-id="656f3-134">役割の定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="656f3-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="656f3-135">subjectCount</span><span class="sxs-lookup"><span data-stu-id="656f3-135">subjectCount</span></span>|<span data-ttu-id="656f3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="656f3-136">Int32</span></span>     |<span data-ttu-id="656f3-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="656f3-137">Optional.</span></span> <span data-ttu-id="656f3-138">ロールに割り当てられている被験者の数です。</span><span class="sxs-lookup"><span data-stu-id="656f3-138">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="656f3-139">リソースへのアクセスの要求元の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="656f3-139">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="656f3-140">プロパティを取得するには、明示的に使用をしてください。`$select=subjectCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="656f3-140">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="656f3-141">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="656f3-141">eligibleAssignmentCount</span></span>|<span data-ttu-id="656f3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="656f3-142">Int32</span></span>|<span data-ttu-id="656f3-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="656f3-143">Optional.</span></span> <span data-ttu-id="656f3-144">役割の定義に関連付けられている対象のロールの割り当ての数です。</span><span class="sxs-lookup"><span data-stu-id="656f3-144">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="656f3-145">プロパティを取得するには、明示的に使用をしてください。`$select=eligibleAssignmentCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="656f3-145">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="656f3-146">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="656f3-146">activeAssignmentCount</span></span>|<span data-ttu-id="656f3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="656f3-147">Int32</span></span>    |<span data-ttu-id="656f3-148">省略可能。</span><span class="sxs-lookup"><span data-stu-id="656f3-148">Optional.</span></span> <span data-ttu-id="656f3-149">役割の定義に関連付けられているアクティブなロールの割り当ての数です。</span><span class="sxs-lookup"><span data-stu-id="656f3-149">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="656f3-150">プロパティを取得するには、明示的に使用をしてください。`$select=activeAssignmentCount`クエリにします。</span><span class="sxs-lookup"><span data-stu-id="656f3-150">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="656f3-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="656f3-151">Relationships</span></span>
| <span data-ttu-id="656f3-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="656f3-152">Relationship</span></span> | <span data-ttu-id="656f3-153">型</span><span class="sxs-lookup"><span data-stu-id="656f3-153">Type</span></span>   |<span data-ttu-id="656f3-154">説明</span><span class="sxs-lookup"><span data-stu-id="656f3-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="656f3-155">リソース</span><span class="sxs-lookup"><span data-stu-id="656f3-155">resource</span></span>|[<span data-ttu-id="656f3-156">governanceResource</span><span class="sxs-lookup"><span data-stu-id="656f3-156">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="656f3-157">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="656f3-157">Read-only.</span></span> <span data-ttu-id="656f3-158">役割の定義に関連付けられているリソースです。</span><span class="sxs-lookup"><span data-stu-id="656f3-158">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="656f3-159">roleSetting</span><span class="sxs-lookup"><span data-stu-id="656f3-159">roleSetting</span></span>|[<span data-ttu-id="656f3-160">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="656f3-160">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="656f3-161">役割の定義に関連付けられている役割の設定をします。</span><span class="sxs-lookup"><span data-stu-id="656f3-161">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="656f3-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="656f3-162">JSON representation</span></span>

<span data-ttu-id="656f3-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="656f3-163">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroledefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
