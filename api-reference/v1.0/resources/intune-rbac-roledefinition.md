---
title: roleDefinition リソース タイプ
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: de9df8872f5c9939082076c5e0d94c2c4fe50ed5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037115"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="da727-109">roleDefinition リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="da727-109">roleDefinition resource type</span></span>

> <span data-ttu-id="da727-110">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da727-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da727-111">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="da727-111">The Role Definition resource.</span></span> <span data-ttu-id="da727-112">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="da727-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="da727-113">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="da727-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="da727-114">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="da727-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="da727-115">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="da727-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="da727-116">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="da727-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="da727-117">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="da727-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="da727-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="da727-118">Methods</span></span>
|<span data-ttu-id="da727-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="da727-119">Method</span></span>|<span data-ttu-id="da727-120">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="da727-120">Return Type</span></span>|<span data-ttu-id="da727-121">説明</span><span class="sxs-lookup"><span data-stu-id="da727-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da727-122">List roleDefinition</span><span class="sxs-lookup"><span data-stu-id="da727-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="da727-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="da727-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="da727-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="da727-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="da727-125">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="da727-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="da727-126">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="da727-126">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="da727-127">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="da727-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="da727-128">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="da727-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="da727-129">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="da727-129">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="da727-130">新しい [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="da727-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="da727-131">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="da727-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="da727-132">なし</span><span class="sxs-lookup"><span data-stu-id="da727-132">None</span></span>|<span data-ttu-id="da727-133">[roleDefinition](../resources/intune-rbac-roledefinition.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="da727-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="da727-134">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="da727-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="da727-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="da727-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="da727-136">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="da727-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da727-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da727-137">Properties</span></span>
|<span data-ttu-id="da727-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da727-138">Property</span></span>|<span data-ttu-id="da727-139">型</span><span class="sxs-lookup"><span data-stu-id="da727-139">Type</span></span>|<span data-ttu-id="da727-140">説明</span><span class="sxs-lookup"><span data-stu-id="da727-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da727-141">id</span><span class="sxs-lookup"><span data-stu-id="da727-141">id</span></span>|<span data-ttu-id="da727-142">文字列</span><span class="sxs-lookup"><span data-stu-id="da727-142">String</span></span>|<span data-ttu-id="da727-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="da727-143">Key of the entity.</span></span> <span data-ttu-id="da727-144">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="da727-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="da727-145">displayName</span><span class="sxs-lookup"><span data-stu-id="da727-145">displayName</span></span>|<span data-ttu-id="da727-146">String</span><span class="sxs-lookup"><span data-stu-id="da727-146">String</span></span>|<span data-ttu-id="da727-147">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="da727-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="da727-148">description</span><span class="sxs-lookup"><span data-stu-id="da727-148">description</span></span>|<span data-ttu-id="da727-149">String</span><span class="sxs-lookup"><span data-stu-id="da727-149">String</span></span>|<span data-ttu-id="da727-150">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="da727-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="da727-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="da727-151">rolePermissions</span></span>|<span data-ttu-id="da727-152">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="da727-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="da727-153">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="da727-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="da727-154">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="da727-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="da727-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="da727-155">isBuiltIn</span></span>|<span data-ttu-id="da727-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="da727-156">Boolean</span></span>|<span data-ttu-id="da727-157">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="da727-157">Type of Role.</span></span> <span data-ttu-id="da727-158">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="da727-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da727-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da727-159">Relationships</span></span>
|<span data-ttu-id="da727-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da727-160">Relationship</span></span>|<span data-ttu-id="da727-161">型</span><span class="sxs-lookup"><span data-stu-id="da727-161">Type</span></span>|<span data-ttu-id="da727-162">説明</span><span class="sxs-lookup"><span data-stu-id="da727-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da727-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="da727-163">roleAssignments</span></span>|<span data-ttu-id="da727-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="da727-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="da727-165">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="da727-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da727-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da727-166">JSON Representation</span></span>
<span data-ttu-id="da727-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="da727-167">Here is a JSON representation of the resource.</span></span>
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



