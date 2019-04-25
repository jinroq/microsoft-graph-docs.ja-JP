---
title: governanceRoleDefinition リソースの種類
description: ロール定義を表します。 azure リソースの場合は、所有者、リーダー、共同作成者など、azure RBAC の役割を表すことができます。
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547448"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="66631-104">governanceRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66631-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="66631-105">ロール定義を表します。</span><span class="sxs-lookup"><span data-stu-id="66631-105">Represents the role definitions.</span></span> <span data-ttu-id="66631-106">azure リソースの場合は、所有者、リーダー、共同作成者など、azure RBAC の役割を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="66631-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="66631-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="66631-107">Methods</span></span>

| <span data-ttu-id="66631-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="66631-108">Method</span></span>          | <span data-ttu-id="66631-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="66631-109">Return Type</span></span> |<span data-ttu-id="66631-110">説明</span><span class="sxs-lookup"><span data-stu-id="66631-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="66631-111">List</span><span class="sxs-lookup"><span data-stu-id="66631-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="66631-112">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="66631-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="66631-113">リソースのロール定義のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="66631-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="66631-114">取得</span><span class="sxs-lookup"><span data-stu-id="66631-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="66631-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="66631-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="66631-116">id で指定されたロール定義エンティティのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="66631-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="66631-117">`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`</span><span class="sxs-lookup"><span data-stu-id="66631-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="66631-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66631-118">Properties</span></span>
| <span data-ttu-id="66631-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66631-119">Property</span></span>  | <span data-ttu-id="66631-120">型</span><span class="sxs-lookup"><span data-stu-id="66631-120">Type</span></span>      |<span data-ttu-id="66631-121">説明</span><span class="sxs-lookup"><span data-stu-id="66631-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="66631-122">id</span><span class="sxs-lookup"><span data-stu-id="66631-122">id</span></span>         |<span data-ttu-id="66631-123">String</span><span class="sxs-lookup"><span data-stu-id="66631-123">String</span></span>     |<span data-ttu-id="66631-124">ロール定義の id。</span><span class="sxs-lookup"><span data-stu-id="66631-124">The id of the role definition.</span></span> |
|<span data-ttu-id="66631-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="66631-125">resourceId</span></span> |<span data-ttu-id="66631-126">String</span><span class="sxs-lookup"><span data-stu-id="66631-126">String</span></span>     |<span data-ttu-id="66631-127">必須。</span><span class="sxs-lookup"><span data-stu-id="66631-127">Required.</span></span> <span data-ttu-id="66631-128">ロール定義に関連付けられているリソースの id。</span><span class="sxs-lookup"><span data-stu-id="66631-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="66631-129">externalId</span><span class="sxs-lookup"><span data-stu-id="66631-129">externalId</span></span>   |<span data-ttu-id="66631-130">String</span><span class="sxs-lookup"><span data-stu-id="66631-130">String</span></span>     |<span data-ttu-id="66631-131">ロール定義の外部 id。</span><span class="sxs-lookup"><span data-stu-id="66631-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="66631-132">displayName</span><span class="sxs-lookup"><span data-stu-id="66631-132">displayName</span></span>|<span data-ttu-id="66631-133">String</span><span class="sxs-lookup"><span data-stu-id="66631-133">String</span></span>     |<span data-ttu-id="66631-134">ロール定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="66631-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="66631-135">subjectcount</span><span class="sxs-lookup"><span data-stu-id="66631-135">subjectCount</span></span>|<span data-ttu-id="66631-136">Int32</span><span class="sxs-lookup"><span data-stu-id="66631-136">Int32</span></span>     |<span data-ttu-id="66631-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="66631-137">Optional.</span></span> <span data-ttu-id="66631-138">役割に割り当てられているサブジェクトの数。</span><span class="sxs-lookup"><span data-stu-id="66631-138">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="66631-139">これは、リソースへの要求者のアクセスの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="66631-139">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="66631-140">プロパティを取得するには、クエリ`$select=subjectCount`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="66631-140">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="66631-141">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="66631-141">eligibleAssignmentCount</span></span>|<span data-ttu-id="66631-142">Int32</span><span class="sxs-lookup"><span data-stu-id="66631-142">Int32</span></span>|<span data-ttu-id="66631-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="66631-143">Optional.</span></span> <span data-ttu-id="66631-144">役割の定義に関連付けられている対象の役割の割り当ての数。</span><span class="sxs-lookup"><span data-stu-id="66631-144">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="66631-145">プロパティを取得するには、クエリ`$select=eligibleAssignmentCount`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="66631-145">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="66631-146">active割り当てカウント</span><span class="sxs-lookup"><span data-stu-id="66631-146">activeAssignmentCount</span></span>|<span data-ttu-id="66631-147">Int32</span><span class="sxs-lookup"><span data-stu-id="66631-147">Int32</span></span>    |<span data-ttu-id="66631-148">省略可能。</span><span class="sxs-lookup"><span data-stu-id="66631-148">Optional.</span></span> <span data-ttu-id="66631-149">ロール定義に関連付けられているアクティブなロール割り当ての数。</span><span class="sxs-lookup"><span data-stu-id="66631-149">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="66631-150">プロパティを取得するには、クエリ`$select=activeAssignmentCount`で明示的にを使用してください。</span><span class="sxs-lookup"><span data-stu-id="66631-150">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="66631-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66631-151">Relationships</span></span>
| <span data-ttu-id="66631-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66631-152">Relationship</span></span> | <span data-ttu-id="66631-153">型</span><span class="sxs-lookup"><span data-stu-id="66631-153">Type</span></span>   |<span data-ttu-id="66631-154">説明</span><span class="sxs-lookup"><span data-stu-id="66631-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66631-155">リソース</span><span class="sxs-lookup"><span data-stu-id="66631-155">resource</span></span>|[<span data-ttu-id="66631-156">governanceResource</span><span class="sxs-lookup"><span data-stu-id="66631-156">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="66631-157">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66631-157">Read-only.</span></span> <span data-ttu-id="66631-158">ロール定義に関連付けられているリソース。</span><span class="sxs-lookup"><span data-stu-id="66631-158">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="66631-159">rolesetting</span><span class="sxs-lookup"><span data-stu-id="66631-159">roleSetting</span></span>|[<span data-ttu-id="66631-160">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="66631-160">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="66631-161">ロール定義に関連付けられているロール設定。</span><span class="sxs-lookup"><span data-stu-id="66631-161">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66631-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66631-162">JSON representation</span></span>

<span data-ttu-id="66631-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66631-163">Here is a JSON representation of the resource.</span></span>

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
