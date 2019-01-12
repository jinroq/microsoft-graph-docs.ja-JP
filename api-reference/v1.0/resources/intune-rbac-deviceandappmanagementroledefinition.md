---
title: deviceAndAppManagementRoleDefinition リソースの種類
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b3a5204b766352436e1af3964b2f3f4baedc4efa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965188"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="901e6-109">deviceAndAppManagementRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="901e6-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="901e6-110">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="901e6-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="901e6-111">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="901e6-111">The Role Definition resource.</span></span> <span data-ttu-id="901e6-112">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="901e6-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="901e6-113">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="901e6-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="901e6-114">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="901e6-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="901e6-115">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="901e6-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="901e6-116">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="901e6-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="901e6-117">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="901e6-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="901e6-118">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="901e6-118">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="901e6-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="901e6-119">Methods</span></span>
|<span data-ttu-id="901e6-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="901e6-120">Method</span></span>|<span data-ttu-id="901e6-121">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="901e6-121">Return Type</span></span>|<span data-ttu-id="901e6-122">説明</span><span class="sxs-lookup"><span data-stu-id="901e6-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="901e6-123">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="901e6-123">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="901e6-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="901e6-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="901e6-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="901e6-125">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="901e6-126">deviceAndAppManagementRoleDefinition の取得</span><span class="sxs-lookup"><span data-stu-id="901e6-126">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="901e6-127">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="901e6-127">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="901e6-128">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="901e6-128">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="901e6-129">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="901e6-129">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="901e6-130">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="901e6-130">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="901e6-131">新しい [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="901e6-131">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="901e6-132">deviceAndAppManagementRoleDefinition の削除</span><span class="sxs-lookup"><span data-stu-id="901e6-132">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="901e6-133">なし</span><span class="sxs-lookup"><span data-stu-id="901e6-133">None</span></span>|<span data-ttu-id="901e6-134">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の削除</span><span class="sxs-lookup"><span data-stu-id="901e6-134">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="901e6-135">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="901e6-135">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="901e6-136">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="901e6-136">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="901e6-137">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="901e6-137">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="901e6-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="901e6-138">Properties</span></span>
|<span data-ttu-id="901e6-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="901e6-139">Property</span></span>|<span data-ttu-id="901e6-140">種類</span><span class="sxs-lookup"><span data-stu-id="901e6-140">Type</span></span>|<span data-ttu-id="901e6-141">説明</span><span class="sxs-lookup"><span data-stu-id="901e6-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="901e6-142">ID</span><span class="sxs-lookup"><span data-stu-id="901e6-142">id</span></span>|<span data-ttu-id="901e6-143">String</span><span class="sxs-lookup"><span data-stu-id="901e6-143">String</span></span>|<span data-ttu-id="901e6-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="901e6-144">Key of the entity.</span></span> <span data-ttu-id="901e6-145">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="901e6-145">This is read-only and automatically generated.</span></span> <span data-ttu-id="901e6-146">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="901e6-146">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="901e6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="901e6-147">displayName</span></span>|<span data-ttu-id="901e6-148">String</span><span class="sxs-lookup"><span data-stu-id="901e6-148">String</span></span>|<span data-ttu-id="901e6-149">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="901e6-149">Display Name of the Role definition.</span></span> <span data-ttu-id="901e6-150">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="901e6-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="901e6-151">説明</span><span class="sxs-lookup"><span data-stu-id="901e6-151">description</span></span>|<span data-ttu-id="901e6-152">String</span><span class="sxs-lookup"><span data-stu-id="901e6-152">String</span></span>|<span data-ttu-id="901e6-153">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="901e6-153">Description of the Role definition.</span></span> <span data-ttu-id="901e6-154">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="901e6-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="901e6-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="901e6-155">rolePermissions</span></span>|<span data-ttu-id="901e6-156">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="901e6-156">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="901e6-157">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="901e6-157">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="901e6-158">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="901e6-158">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="901e6-159">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="901e6-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="901e6-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="901e6-160">isBuiltIn</span></span>|<span data-ttu-id="901e6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="901e6-161">Boolean</span></span>|<span data-ttu-id="901e6-162">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="901e6-162">Type of Role.</span></span> <span data-ttu-id="901e6-163">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="901e6-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="901e6-164">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="901e6-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="901e6-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="901e6-165">Relationships</span></span>
|<span data-ttu-id="901e6-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="901e6-166">Relationship</span></span>|<span data-ttu-id="901e6-167">型</span><span class="sxs-lookup"><span data-stu-id="901e6-167">Type</span></span>|<span data-ttu-id="901e6-168">説明</span><span class="sxs-lookup"><span data-stu-id="901e6-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="901e6-169">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="901e6-169">roleAssignments</span></span>|<span data-ttu-id="901e6-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="901e6-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="901e6-171">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="901e6-171">List of Role assignments for this role definition.</span></span> <span data-ttu-id="901e6-172">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="901e6-172">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="901e6-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="901e6-173">JSON Representation</span></span>
<span data-ttu-id="901e6-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="901e6-174">Here is a JSON representation of the resource.</span></span>
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



