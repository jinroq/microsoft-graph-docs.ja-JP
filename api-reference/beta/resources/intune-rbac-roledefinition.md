---
title: roleDefinition リソース タイプ
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba38f9293ce4a21d031a3c70e8d3bdbe5667f997
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173718"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="c3ab0-109">roleDefinition リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c3ab0-109">roleDefinition resource type</span></span>

> <span data-ttu-id="c3ab0-110">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3ab0-111">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3ab0-112">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-112">The Role Definition resource.</span></span> <span data-ttu-id="c3ab0-113">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="c3ab0-114">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="c3ab0-115">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="c3ab0-116">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="c3ab0-117">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="c3ab0-118">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="c3ab0-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="c3ab0-119">Methods</span></span>
|<span data-ttu-id="c3ab0-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="c3ab0-120">Method</span></span>|<span data-ttu-id="c3ab0-121">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c3ab0-121">Return Type</span></span>|<span data-ttu-id="c3ab0-122">説明</span><span class="sxs-lookup"><span data-stu-id="c3ab0-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3ab0-123">List roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="c3ab0-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3ab0-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="c3ab0-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="c3ab0-126">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="c3ab0-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="c3ab0-128">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="c3ab0-129">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="c3ab0-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="c3ab0-131">新しい [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="c3ab0-132">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="c3ab0-133">なし</span><span class="sxs-lookup"><span data-stu-id="c3ab0-133">None</span></span>|<span data-ttu-id="c3ab0-134">[roleDefinition](../resources/intune-rbac-roledefinition.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="c3ab0-135">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="c3ab0-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="c3ab0-137">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3ab0-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3ab0-138">Properties</span></span>
|<span data-ttu-id="c3ab0-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3ab0-139">Property</span></span>|<span data-ttu-id="c3ab0-140">型</span><span class="sxs-lookup"><span data-stu-id="c3ab0-140">Type</span></span>|<span data-ttu-id="c3ab0-141">説明</span><span class="sxs-lookup"><span data-stu-id="c3ab0-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ab0-142">id</span><span class="sxs-lookup"><span data-stu-id="c3ab0-142">id</span></span>|<span data-ttu-id="c3ab0-143">文字列</span><span class="sxs-lookup"><span data-stu-id="c3ab0-143">String</span></span>|<span data-ttu-id="c3ab0-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-144">Key of the entity.</span></span> <span data-ttu-id="c3ab0-145">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c3ab0-146">displayName</span><span class="sxs-lookup"><span data-stu-id="c3ab0-146">displayName</span></span>|<span data-ttu-id="c3ab0-147">String</span><span class="sxs-lookup"><span data-stu-id="c3ab0-147">String</span></span>|<span data-ttu-id="c3ab0-148">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="c3ab0-149">説明</span><span class="sxs-lookup"><span data-stu-id="c3ab0-149">description</span></span>|<span data-ttu-id="c3ab0-150">String</span><span class="sxs-lookup"><span data-stu-id="c3ab0-150">String</span></span>|<span data-ttu-id="c3ab0-151">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="c3ab0-152">permissions</span><span class="sxs-lookup"><span data-stu-id="c3ab0-152">permissions</span></span>|<span data-ttu-id="c3ab0-153">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3ab0-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c3ab0-154">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c3ab0-155">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="c3ab0-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c3ab0-156">rolePermissions</span></span>|<span data-ttu-id="c3ab0-157">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3ab0-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c3ab0-158">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c3ab0-159">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-159">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="c3ab0-160">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c3ab0-160">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="c3ab0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3ab0-161">Boolean</span></span>|<span data-ttu-id="c3ab0-162">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-162">Type of Role.</span></span> <span data-ttu-id="c3ab0-163">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="c3ab0-164">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c3ab0-164">isBuiltIn</span></span>|<span data-ttu-id="c3ab0-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3ab0-165">Boolean</span></span>|<span data-ttu-id="c3ab0-166">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-166">Type of Role.</span></span> <span data-ttu-id="c3ab0-167">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-167">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="c3ab0-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3ab0-168">roleScopeTagIds</span></span>|<span data-ttu-id="c3ab0-169">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c3ab0-169">String collection</span></span>|<span data-ttu-id="c3ab0-170">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-170">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3ab0-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3ab0-171">Relationships</span></span>
|<span data-ttu-id="c3ab0-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3ab0-172">Relationship</span></span>|<span data-ttu-id="c3ab0-173">型</span><span class="sxs-lookup"><span data-stu-id="c3ab0-173">Type</span></span>|<span data-ttu-id="c3ab0-174">説明</span><span class="sxs-lookup"><span data-stu-id="c3ab0-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ab0-175">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="c3ab0-175">roleAssignments</span></span>|<span data-ttu-id="c3ab0-176">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3ab0-176">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="c3ab0-177">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-177">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3ab0-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3ab0-178">JSON Representation</span></span>
<span data-ttu-id="c3ab0-179">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3ab0-179">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




