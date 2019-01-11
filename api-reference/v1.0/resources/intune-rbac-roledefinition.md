---
title: roleDefinition リソース タイプ
description: ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。
localization_priority: Normal
ms.openlocfilehash: d3f5ef8ddd67302b747b2f35b0e4f62f3f6c00d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804817"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="02490-109">roleDefinition リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="02490-109">roleDefinition resource type</span></span>

> <span data-ttu-id="02490-110">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="02490-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02490-111">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="02490-111">The Role Definition resource.</span></span> <span data-ttu-id="02490-112">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="02490-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="02490-113">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="02490-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="02490-114">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="02490-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="02490-115">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="02490-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="02490-116">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="02490-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="02490-117">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="02490-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="02490-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="02490-118">Methods</span></span>
|<span data-ttu-id="02490-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="02490-119">Method</span></span>|<span data-ttu-id="02490-120">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="02490-120">Return Type</span></span>|<span data-ttu-id="02490-121">説明</span><span class="sxs-lookup"><span data-stu-id="02490-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="02490-122">List roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02490-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="02490-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="02490-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="02490-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="02490-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="02490-125">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02490-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="02490-126">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02490-126">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="02490-127">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="02490-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="02490-128">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02490-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="02490-129">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02490-129">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="02490-130">新しい [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="02490-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="02490-131">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02490-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="02490-132">なし</span><span class="sxs-lookup"><span data-stu-id="02490-132">None</span></span>|<span data-ttu-id="02490-133">[roleDefinition](../resources/intune-rbac-roledefinition.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="02490-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="02490-134">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02490-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="02490-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02490-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="02490-136">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="02490-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="02490-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02490-137">Properties</span></span>
|<span data-ttu-id="02490-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02490-138">Property</span></span>|<span data-ttu-id="02490-139">種類</span><span class="sxs-lookup"><span data-stu-id="02490-139">Type</span></span>|<span data-ttu-id="02490-140">説明</span><span class="sxs-lookup"><span data-stu-id="02490-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02490-141">ID</span><span class="sxs-lookup"><span data-stu-id="02490-141">id</span></span>|<span data-ttu-id="02490-142">String</span><span class="sxs-lookup"><span data-stu-id="02490-142">String</span></span>|<span data-ttu-id="02490-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="02490-143">Key of the entity.</span></span> <span data-ttu-id="02490-144">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="02490-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="02490-145">displayName</span><span class="sxs-lookup"><span data-stu-id="02490-145">displayName</span></span>|<span data-ttu-id="02490-146">String</span><span class="sxs-lookup"><span data-stu-id="02490-146">String</span></span>|<span data-ttu-id="02490-147">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="02490-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="02490-148">説明</span><span class="sxs-lookup"><span data-stu-id="02490-148">description</span></span>|<span data-ttu-id="02490-149">String</span><span class="sxs-lookup"><span data-stu-id="02490-149">String</span></span>|<span data-ttu-id="02490-150">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="02490-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="02490-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="02490-151">rolePermissions</span></span>|<span data-ttu-id="02490-152">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="02490-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="02490-153">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="02490-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="02490-154">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="02490-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="02490-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="02490-155">isBuiltIn</span></span>|<span data-ttu-id="02490-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="02490-156">Boolean</span></span>|<span data-ttu-id="02490-157">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="02490-157">Type of Role.</span></span> <span data-ttu-id="02490-158">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="02490-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02490-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02490-159">Relationships</span></span>
|<span data-ttu-id="02490-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02490-160">Relationship</span></span>|<span data-ttu-id="02490-161">型</span><span class="sxs-lookup"><span data-stu-id="02490-161">Type</span></span>|<span data-ttu-id="02490-162">説明</span><span class="sxs-lookup"><span data-stu-id="02490-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02490-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="02490-163">roleAssignments</span></span>|<span data-ttu-id="02490-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="02490-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="02490-165">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="02490-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02490-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02490-166">JSON Representation</span></span>
<span data-ttu-id="02490-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="02490-167">Here is a JSON representation of the resource.</span></span>
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



