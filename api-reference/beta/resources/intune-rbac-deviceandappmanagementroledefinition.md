---
title: deviceAndAppManagementRoleDefinition リソースの種類
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cc3bd898799ef2c2da6fca5a0043fc86ee5bd8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411982"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="6e425-109">deviceAndAppManagementRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e425-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="6e425-110">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6e425-110">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e425-111">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e425-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e425-112">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6e425-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e425-113">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="6e425-113">The Role Definition resource.</span></span> <span data-ttu-id="6e425-114">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="6e425-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="6e425-115">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="6e425-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="6e425-116">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="6e425-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="6e425-117">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="6e425-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="6e425-118">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e425-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="6e425-119">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="6e425-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="6e425-120">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6e425-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="6e425-121">Methods</span></span>
|<span data-ttu-id="6e425-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="6e425-122">Method</span></span>|<span data-ttu-id="6e425-123">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6e425-123">Return Type</span></span>|<span data-ttu-id="6e425-124">説明</span><span class="sxs-lookup"><span data-stu-id="6e425-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e425-125">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="6e425-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="6e425-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6e425-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="6e425-127">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6e425-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="6e425-128">deviceAndAppManagementRoleDefinition の取得</span><span class="sxs-lookup"><span data-stu-id="6e425-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="6e425-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6e425-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="6e425-130">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6e425-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="6e425-131">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="6e425-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="6e425-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6e425-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="6e425-133">新しい [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6e425-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="6e425-134">deviceAndAppManagementRoleDefinition の削除</span><span class="sxs-lookup"><span data-stu-id="6e425-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="6e425-135">なし</span><span class="sxs-lookup"><span data-stu-id="6e425-135">None</span></span>|<span data-ttu-id="6e425-136">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の削除</span><span class="sxs-lookup"><span data-stu-id="6e425-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="6e425-137">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="6e425-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="6e425-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6e425-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="6e425-139">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6e425-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e425-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e425-140">Properties</span></span>
|<span data-ttu-id="6e425-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e425-141">Property</span></span>|<span data-ttu-id="6e425-142">型</span><span class="sxs-lookup"><span data-stu-id="6e425-142">Type</span></span>|<span data-ttu-id="6e425-143">説明</span><span class="sxs-lookup"><span data-stu-id="6e425-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e425-144">id</span><span class="sxs-lookup"><span data-stu-id="6e425-144">id</span></span>|<span data-ttu-id="6e425-145">String</span><span class="sxs-lookup"><span data-stu-id="6e425-145">String</span></span>|<span data-ttu-id="6e425-146">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6e425-146">Key of the entity.</span></span> <span data-ttu-id="6e425-147">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="6e425-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="6e425-148">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6e425-149">displayName</span><span class="sxs-lookup"><span data-stu-id="6e425-149">displayName</span></span>|<span data-ttu-id="6e425-150">String</span><span class="sxs-lookup"><span data-stu-id="6e425-150">String</span></span>|<span data-ttu-id="6e425-151">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="6e425-151">Display Name of the Role definition.</span></span> <span data-ttu-id="6e425-152">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6e425-153">説明</span><span class="sxs-lookup"><span data-stu-id="6e425-153">description</span></span>|<span data-ttu-id="6e425-154">String</span><span class="sxs-lookup"><span data-stu-id="6e425-154">String</span></span>|<span data-ttu-id="6e425-155">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="6e425-155">Description of the Role definition.</span></span> <span data-ttu-id="6e425-156">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6e425-157">permissions</span><span class="sxs-lookup"><span data-stu-id="6e425-157">permissions</span></span>|<span data-ttu-id="6e425-158">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6e425-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="6e425-159">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="6e425-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="6e425-160">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e425-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="6e425-161">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6e425-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="6e425-162">rolePermissions</span></span>|<span data-ttu-id="6e425-163">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6e425-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="6e425-164">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="6e425-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="6e425-165">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e425-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="6e425-166">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6e425-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6e425-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="6e425-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e425-168">Boolean</span></span>|<span data-ttu-id="6e425-169">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="6e425-169">Type of Role.</span></span> <span data-ttu-id="6e425-170">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="6e425-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="6e425-171">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6e425-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="6e425-172">isBuiltIn</span></span>|<span data-ttu-id="6e425-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e425-173">Boolean</span></span>|<span data-ttu-id="6e425-174">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="6e425-174">Type of Role.</span></span> <span data-ttu-id="6e425-175">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="6e425-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="6e425-176">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6e425-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e425-177">roleScopeTagIds</span></span>|<span data-ttu-id="6e425-178">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6e425-178">String collection</span></span>|<span data-ttu-id="6e425-179">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="6e425-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e425-180">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-180">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e425-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6e425-181">Relationships</span></span>
|<span data-ttu-id="6e425-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6e425-182">Relationship</span></span>|<span data-ttu-id="6e425-183">型</span><span class="sxs-lookup"><span data-stu-id="6e425-183">Type</span></span>|<span data-ttu-id="6e425-184">説明</span><span class="sxs-lookup"><span data-stu-id="6e425-184">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e425-185">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="6e425-185">roleAssignments</span></span>|<span data-ttu-id="6e425-186">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6e425-186">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="6e425-187">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="6e425-187">List of Role assignments for this role definition.</span></span> <span data-ttu-id="6e425-188">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6e425-188">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e425-189">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e425-189">JSON Representation</span></span>
<span data-ttu-id="6e425-190">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6e425-190">Here is a JSON representation of the resource.</span></span>
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




