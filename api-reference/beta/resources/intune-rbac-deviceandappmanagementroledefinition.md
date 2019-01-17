---
title: deviceAndAppManagementRoleDefinition リソースの種類
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: abe28e4b36c62df049e5f85b910e27f787bce2bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922894"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="e3a10-109">deviceAndAppManagementRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e3a10-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="e3a10-110">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e3a10-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3a10-111">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3a10-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3a10-112">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3a10-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3a10-113">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="e3a10-113">The Role Definition resource.</span></span> <span data-ttu-id="e3a10-114">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="e3a10-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="e3a10-115">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="e3a10-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="e3a10-116">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="e3a10-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="e3a10-117">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="e3a10-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="e3a10-118">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3a10-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="e3a10-119">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="e3a10-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="e3a10-120">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e3a10-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3a10-121">Methods</span></span>
|<span data-ttu-id="e3a10-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3a10-122">Method</span></span>|<span data-ttu-id="e3a10-123">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e3a10-123">Return Type</span></span>|<span data-ttu-id="e3a10-124">説明</span><span class="sxs-lookup"><span data-stu-id="e3a10-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3a10-125">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="e3a10-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="e3a10-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3a10-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="e3a10-127">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e3a10-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="e3a10-128">deviceAndAppManagementRoleDefinition の取得</span><span class="sxs-lookup"><span data-stu-id="e3a10-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="e3a10-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e3a10-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="e3a10-130">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e3a10-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="e3a10-131">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="e3a10-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="e3a10-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e3a10-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="e3a10-133">新しい [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e3a10-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="e3a10-134">deviceAndAppManagementRoleDefinition の削除</span><span class="sxs-lookup"><span data-stu-id="e3a10-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="e3a10-135">なし</span><span class="sxs-lookup"><span data-stu-id="e3a10-135">None</span></span>|<span data-ttu-id="e3a10-136">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の削除</span><span class="sxs-lookup"><span data-stu-id="e3a10-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="e3a10-137">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="e3a10-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="e3a10-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e3a10-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="e3a10-139">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3a10-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3a10-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3a10-140">Properties</span></span>
|<span data-ttu-id="e3a10-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3a10-141">Property</span></span>|<span data-ttu-id="e3a10-142">型</span><span class="sxs-lookup"><span data-stu-id="e3a10-142">Type</span></span>|<span data-ttu-id="e3a10-143">説明</span><span class="sxs-lookup"><span data-stu-id="e3a10-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3a10-144">id</span><span class="sxs-lookup"><span data-stu-id="e3a10-144">id</span></span>|<span data-ttu-id="e3a10-145">String</span><span class="sxs-lookup"><span data-stu-id="e3a10-145">String</span></span>|<span data-ttu-id="e3a10-146">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e3a10-146">Key of the entity.</span></span> <span data-ttu-id="e3a10-147">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="e3a10-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="e3a10-148">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="e3a10-149">displayName</span><span class="sxs-lookup"><span data-stu-id="e3a10-149">displayName</span></span>|<span data-ttu-id="e3a10-150">String</span><span class="sxs-lookup"><span data-stu-id="e3a10-150">String</span></span>|<span data-ttu-id="e3a10-151">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="e3a10-151">Display Name of the Role definition.</span></span> <span data-ttu-id="e3a10-152">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="e3a10-153">説明</span><span class="sxs-lookup"><span data-stu-id="e3a10-153">description</span></span>|<span data-ttu-id="e3a10-154">String</span><span class="sxs-lookup"><span data-stu-id="e3a10-154">String</span></span>|<span data-ttu-id="e3a10-155">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="e3a10-155">Description of the Role definition.</span></span> <span data-ttu-id="e3a10-156">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="e3a10-157">permissions</span><span class="sxs-lookup"><span data-stu-id="e3a10-157">permissions</span></span>|<span data-ttu-id="e3a10-158">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3a10-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e3a10-159">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="e3a10-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e3a10-160">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3a10-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="e3a10-161">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="e3a10-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e3a10-162">rolePermissions</span></span>|<span data-ttu-id="e3a10-163">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3a10-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e3a10-164">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="e3a10-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e3a10-165">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3a10-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="e3a10-166">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="e3a10-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e3a10-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="e3a10-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3a10-168">Boolean</span></span>|<span data-ttu-id="e3a10-169">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="e3a10-169">Type of Role.</span></span> <span data-ttu-id="e3a10-170">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="e3a10-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="e3a10-171">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="e3a10-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e3a10-172">isBuiltIn</span></span>|<span data-ttu-id="e3a10-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3a10-173">Boolean</span></span>|<span data-ttu-id="e3a10-174">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="e3a10-174">Type of Role.</span></span> <span data-ttu-id="e3a10-175">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="e3a10-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="e3a10-176">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3a10-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3a10-177">Relationships</span></span>
|<span data-ttu-id="e3a10-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3a10-178">Relationship</span></span>|<span data-ttu-id="e3a10-179">型</span><span class="sxs-lookup"><span data-stu-id="e3a10-179">Type</span></span>|<span data-ttu-id="e3a10-180">説明</span><span class="sxs-lookup"><span data-stu-id="e3a10-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3a10-181">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="e3a10-181">roleAssignments</span></span>|<span data-ttu-id="e3a10-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3a10-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="e3a10-183">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="e3a10-183">List of Role assignments for this role definition.</span></span> <span data-ttu-id="e3a10-184">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3a10-184">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3a10-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e3a10-185">JSON Representation</span></span>
<span data-ttu-id="e3a10-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e3a10-186">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true
}
```





