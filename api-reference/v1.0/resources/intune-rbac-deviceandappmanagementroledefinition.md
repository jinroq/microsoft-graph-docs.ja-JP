---
title: deviceAndAppManagementRoleDefinition リソースの種類
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4e231cab152bf4e9952a6dc65fda63013c33732
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037171"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="246dc-109">deviceAndAppManagementRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="246dc-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="246dc-110">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="246dc-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="246dc-111">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="246dc-111">The Role Definition resource.</span></span> <span data-ttu-id="246dc-112">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="246dc-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="246dc-113">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="246dc-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="246dc-114">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="246dc-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="246dc-115">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="246dc-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="246dc-116">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="246dc-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="246dc-117">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="246dc-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="246dc-118">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246dc-118">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="246dc-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="246dc-119">Methods</span></span>
|<span data-ttu-id="246dc-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="246dc-120">Method</span></span>|<span data-ttu-id="246dc-121">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="246dc-121">Return Type</span></span>|<span data-ttu-id="246dc-122">説明</span><span class="sxs-lookup"><span data-stu-id="246dc-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="246dc-123">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="246dc-123">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="246dc-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="246dc-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="246dc-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="246dc-125">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="246dc-126">deviceAndAppManagementRoleDefinition の取得</span><span class="sxs-lookup"><span data-stu-id="246dc-126">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="246dc-127">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="246dc-127">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="246dc-128">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="246dc-128">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="246dc-129">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="246dc-129">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="246dc-130">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="246dc-130">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="246dc-131">新しい [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="246dc-131">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="246dc-132">deviceAndAppManagementRoleDefinition の削除</span><span class="sxs-lookup"><span data-stu-id="246dc-132">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="246dc-133">なし</span><span class="sxs-lookup"><span data-stu-id="246dc-133">None</span></span>|<span data-ttu-id="246dc-134">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の削除</span><span class="sxs-lookup"><span data-stu-id="246dc-134">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="246dc-135">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="246dc-135">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="246dc-136">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="246dc-136">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="246dc-137">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="246dc-137">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="246dc-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="246dc-138">Properties</span></span>
|<span data-ttu-id="246dc-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="246dc-139">Property</span></span>|<span data-ttu-id="246dc-140">型</span><span class="sxs-lookup"><span data-stu-id="246dc-140">Type</span></span>|<span data-ttu-id="246dc-141">説明</span><span class="sxs-lookup"><span data-stu-id="246dc-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="246dc-142">id</span><span class="sxs-lookup"><span data-stu-id="246dc-142">id</span></span>|<span data-ttu-id="246dc-143">文字列</span><span class="sxs-lookup"><span data-stu-id="246dc-143">String</span></span>|<span data-ttu-id="246dc-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="246dc-144">Key of the entity.</span></span> <span data-ttu-id="246dc-145">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="246dc-145">This is read-only and automatically generated.</span></span> <span data-ttu-id="246dc-146">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246dc-146">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="246dc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="246dc-147">displayName</span></span>|<span data-ttu-id="246dc-148">String</span><span class="sxs-lookup"><span data-stu-id="246dc-148">String</span></span>|<span data-ttu-id="246dc-149">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="246dc-149">Display Name of the Role definition.</span></span> <span data-ttu-id="246dc-150">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246dc-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="246dc-151">description</span><span class="sxs-lookup"><span data-stu-id="246dc-151">description</span></span>|<span data-ttu-id="246dc-152">String</span><span class="sxs-lookup"><span data-stu-id="246dc-152">String</span></span>|<span data-ttu-id="246dc-153">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="246dc-153">Description of the Role definition.</span></span> <span data-ttu-id="246dc-154">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246dc-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="246dc-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="246dc-155">rolePermissions</span></span>|<span data-ttu-id="246dc-156">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="246dc-156">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="246dc-157">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="246dc-157">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="246dc-158">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="246dc-158">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="246dc-159">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246dc-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="246dc-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="246dc-160">isBuiltIn</span></span>|<span data-ttu-id="246dc-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="246dc-161">Boolean</span></span>|<span data-ttu-id="246dc-162">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="246dc-162">Type of Role.</span></span> <span data-ttu-id="246dc-163">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="246dc-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="246dc-164">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246dc-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="246dc-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="246dc-165">Relationships</span></span>
|<span data-ttu-id="246dc-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="246dc-166">Relationship</span></span>|<span data-ttu-id="246dc-167">型</span><span class="sxs-lookup"><span data-stu-id="246dc-167">Type</span></span>|<span data-ttu-id="246dc-168">説明</span><span class="sxs-lookup"><span data-stu-id="246dc-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="246dc-169">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="246dc-169">roleAssignments</span></span>|<span data-ttu-id="246dc-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="246dc-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="246dc-171">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="246dc-171">List of Role assignments for this role definition.</span></span> <span data-ttu-id="246dc-172">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246dc-172">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="246dc-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="246dc-173">JSON Representation</span></span>
<span data-ttu-id="246dc-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="246dc-174">Here is a JSON representation of the resource.</span></span>
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```



