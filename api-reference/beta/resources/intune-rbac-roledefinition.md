---
title: roleDefinition リソース タイプ
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e2394fdd260f895d9da3dc36df8579490f0382b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982906"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="e63e9-109">roleDefinition リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="e63e9-109">roleDefinition resource type</span></span>

> <span data-ttu-id="e63e9-110">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e63e9-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e63e9-111">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e63e9-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e63e9-112">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e63e9-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e63e9-113">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="e63e9-113">The Role Definition resource.</span></span> <span data-ttu-id="e63e9-114">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="e63e9-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="e63e9-115">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="e63e9-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="e63e9-116">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="e63e9-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="e63e9-117">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="e63e9-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="e63e9-118">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e63e9-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="e63e9-119">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="e63e9-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="e63e9-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="e63e9-120">Methods</span></span>
|<span data-ttu-id="e63e9-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="e63e9-121">Method</span></span>|<span data-ttu-id="e63e9-122">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e63e9-122">Return Type</span></span>|<span data-ttu-id="e63e9-123">説明</span><span class="sxs-lookup"><span data-stu-id="e63e9-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e63e9-124">List roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="e63e9-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e63e9-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="e63e9-126">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e63e9-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="e63e9-127">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="e63e9-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e63e9-129">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e63e9-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="e63e9-130">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="e63e9-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e63e9-132">新しい [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e63e9-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="e63e9-133">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="e63e9-134">なし</span><span class="sxs-lookup"><span data-stu-id="e63e9-134">None</span></span>|<span data-ttu-id="e63e9-135">[roleDefinition](../resources/intune-rbac-roledefinition.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e63e9-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="e63e9-136">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="e63e9-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e63e9-138">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e63e9-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e63e9-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e63e9-139">Properties</span></span>
|<span data-ttu-id="e63e9-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e63e9-140">Property</span></span>|<span data-ttu-id="e63e9-141">型</span><span class="sxs-lookup"><span data-stu-id="e63e9-141">Type</span></span>|<span data-ttu-id="e63e9-142">説明</span><span class="sxs-lookup"><span data-stu-id="e63e9-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e63e9-143">ID</span><span class="sxs-lookup"><span data-stu-id="e63e9-143">id</span></span>|<span data-ttu-id="e63e9-144">String</span><span class="sxs-lookup"><span data-stu-id="e63e9-144">String</span></span>|<span data-ttu-id="e63e9-145">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e63e9-145">Key of the entity.</span></span> <span data-ttu-id="e63e9-146">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="e63e9-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e63e9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e63e9-147">displayName</span></span>|<span data-ttu-id="e63e9-148">String</span><span class="sxs-lookup"><span data-stu-id="e63e9-148">String</span></span>|<span data-ttu-id="e63e9-149">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="e63e9-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="e63e9-150">説明</span><span class="sxs-lookup"><span data-stu-id="e63e9-150">description</span></span>|<span data-ttu-id="e63e9-151">String</span><span class="sxs-lookup"><span data-stu-id="e63e9-151">String</span></span>|<span data-ttu-id="e63e9-152">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="e63e9-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="e63e9-153">permissions</span><span class="sxs-lookup"><span data-stu-id="e63e9-153">permissions</span></span>|<span data-ttu-id="e63e9-154">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e63e9-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e63e9-155">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="e63e9-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e63e9-156">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e63e9-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e63e9-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e63e9-157">rolePermissions</span></span>|<span data-ttu-id="e63e9-158">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e63e9-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e63e9-159">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="e63e9-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e63e9-160">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e63e9-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e63e9-161">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e63e9-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="e63e9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e63e9-162">Boolean</span></span>|<span data-ttu-id="e63e9-163">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="e63e9-163">Type of Role.</span></span> <span data-ttu-id="e63e9-164">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="e63e9-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="e63e9-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e63e9-165">isBuiltIn</span></span>|<span data-ttu-id="e63e9-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="e63e9-166">Boolean</span></span>|<span data-ttu-id="e63e9-167">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="e63e9-167">Type of Role.</span></span> <span data-ttu-id="e63e9-168">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="e63e9-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e63e9-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e63e9-169">Relationships</span></span>
|<span data-ttu-id="e63e9-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e63e9-170">Relationship</span></span>|<span data-ttu-id="e63e9-171">型</span><span class="sxs-lookup"><span data-stu-id="e63e9-171">Type</span></span>|<span data-ttu-id="e63e9-172">説明</span><span class="sxs-lookup"><span data-stu-id="e63e9-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e63e9-173">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="e63e9-173">roleAssignments</span></span>|<span data-ttu-id="e63e9-174">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e63e9-174">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="e63e9-175">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="e63e9-175">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e63e9-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e63e9-176">JSON Representation</span></span>
<span data-ttu-id="e63e9-177">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e63e9-177">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true
}
```





