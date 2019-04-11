---
title: deviceAndAppManagementRoleDefinition リソースの種類
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29ba1b9555d8e01b9a2f9bd80e476e1cf0ba5c7d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793540"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="50a38-109">deviceAndAppManagementRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50a38-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="50a38-110">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50a38-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50a38-111">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50a38-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50a38-112">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="50a38-112">The Role Definition resource.</span></span> <span data-ttu-id="50a38-113">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="50a38-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="50a38-114">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="50a38-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="50a38-115">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="50a38-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="50a38-116">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="50a38-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="50a38-117">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="50a38-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="50a38-118">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="50a38-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="50a38-119">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="50a38-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="50a38-120">Methods</span></span>
|<span data-ttu-id="50a38-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="50a38-121">Method</span></span>|<span data-ttu-id="50a38-122">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="50a38-122">Return Type</span></span>|<span data-ttu-id="50a38-123">説明</span><span class="sxs-lookup"><span data-stu-id="50a38-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50a38-124">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="50a38-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="50a38-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50a38-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="50a38-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="50a38-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="50a38-127">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50a38-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="50a38-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50a38-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="50a38-129">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="50a38-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="50a38-130">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="50a38-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="50a38-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50a38-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="50a38-132">新しい [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="50a38-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="50a38-133">deviceAndAppManagementRoleDefinition の削除</span><span class="sxs-lookup"><span data-stu-id="50a38-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="50a38-134">なし</span><span class="sxs-lookup"><span data-stu-id="50a38-134">None</span></span>|<span data-ttu-id="50a38-135">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の削除</span><span class="sxs-lookup"><span data-stu-id="50a38-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="50a38-136">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="50a38-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="50a38-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50a38-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="50a38-138">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="50a38-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50a38-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50a38-139">Properties</span></span>
|<span data-ttu-id="50a38-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50a38-140">Property</span></span>|<span data-ttu-id="50a38-141">型</span><span class="sxs-lookup"><span data-stu-id="50a38-141">Type</span></span>|<span data-ttu-id="50a38-142">説明</span><span class="sxs-lookup"><span data-stu-id="50a38-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a38-143">id</span><span class="sxs-lookup"><span data-stu-id="50a38-143">id</span></span>|<span data-ttu-id="50a38-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="50a38-144">String</span></span>|<span data-ttu-id="50a38-145">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="50a38-145">Key of the entity.</span></span> <span data-ttu-id="50a38-146">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="50a38-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="50a38-147">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="50a38-148">displayName</span><span class="sxs-lookup"><span data-stu-id="50a38-148">displayName</span></span>|<span data-ttu-id="50a38-149">String</span><span class="sxs-lookup"><span data-stu-id="50a38-149">String</span></span>|<span data-ttu-id="50a38-150">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="50a38-150">Display Name of the Role definition.</span></span> <span data-ttu-id="50a38-151">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="50a38-152">説明</span><span class="sxs-lookup"><span data-stu-id="50a38-152">description</span></span>|<span data-ttu-id="50a38-153">String</span><span class="sxs-lookup"><span data-stu-id="50a38-153">String</span></span>|<span data-ttu-id="50a38-154">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="50a38-154">Description of the Role definition.</span></span> <span data-ttu-id="50a38-155">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="50a38-156">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50a38-156">permissions</span></span>|<span data-ttu-id="50a38-157">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50a38-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="50a38-158">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="50a38-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="50a38-159">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="50a38-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="50a38-160">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="50a38-161">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="50a38-161">rolePermissions</span></span>|<span data-ttu-id="50a38-162">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50a38-162">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="50a38-163">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="50a38-163">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="50a38-164">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="50a38-164">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="50a38-165">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="50a38-166">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50a38-166">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="50a38-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="50a38-167">Boolean</span></span>|<span data-ttu-id="50a38-168">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="50a38-168">Type of Role.</span></span> <span data-ttu-id="50a38-169">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="50a38-169">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="50a38-170">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-170">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="50a38-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="50a38-171">isBuiltIn</span></span>|<span data-ttu-id="50a38-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="50a38-172">Boolean</span></span>|<span data-ttu-id="50a38-173">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="50a38-173">Type of Role.</span></span> <span data-ttu-id="50a38-174">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="50a38-174">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="50a38-175">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-175">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="50a38-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50a38-176">roleScopeTagIds</span></span>|<span data-ttu-id="50a38-177">String コレクション</span><span class="sxs-lookup"><span data-stu-id="50a38-177">String collection</span></span>|<span data-ttu-id="50a38-178">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="50a38-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50a38-179">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-179">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="50a38-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="50a38-180">Relationships</span></span>
|<span data-ttu-id="50a38-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="50a38-181">Relationship</span></span>|<span data-ttu-id="50a38-182">型</span><span class="sxs-lookup"><span data-stu-id="50a38-182">Type</span></span>|<span data-ttu-id="50a38-183">説明</span><span class="sxs-lookup"><span data-stu-id="50a38-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a38-184">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="50a38-184">roleAssignments</span></span>|<span data-ttu-id="50a38-185">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50a38-185">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="50a38-186">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="50a38-186">List of Role assignments for this role definition.</span></span> <span data-ttu-id="50a38-187">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50a38-187">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50a38-188">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50a38-188">JSON Representation</span></span>
<span data-ttu-id="50a38-189">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="50a38-189">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
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





