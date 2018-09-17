# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="1aae8-101">deviceAndAppManagementRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1aae8-101">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="1aae8-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1aae8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1aae8-103">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="1aae8-103">The Role Definition resource.</span></span> <span data-ttu-id="1aae8-104">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="1aae8-104">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="1aae8-105">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="1aae8-105">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="1aae8-106">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="1aae8-106">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="1aae8-107">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="1aae8-107">Built-in roles cannot be modified.</span></span> <span data-ttu-id="1aae8-108">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1aae8-108">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="1aae8-109">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="1aae8-109">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="1aae8-110">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1aae8-110">Inherits from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1aae8-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="1aae8-111">Methods</span></span>
|<span data-ttu-id="1aae8-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="1aae8-112">Method</span></span>|<span data-ttu-id="1aae8-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1aae8-113">Return Type</span></span>|<span data-ttu-id="1aae8-114">説明</span><span class="sxs-lookup"><span data-stu-id="1aae8-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1aae8-115">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="1aae8-115">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune_rbac_deviceandappmanagementroledefinition_list.md)|<span data-ttu-id="1aae8-116">[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1aae8-116">[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="1aae8-117">[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1aae8-117">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="1aae8-118">deviceAndAppManagementRoleDefinition の取得</span><span class="sxs-lookup"><span data-stu-id="1aae8-118">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune_rbac_deviceandappmanagementroledefinition_get.md)|[<span data-ttu-id="1aae8-119">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1aae8-119">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|<span data-ttu-id="1aae8-120">[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1aae8-120">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="1aae8-121">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="1aae8-121">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune_rbac_deviceandappmanagementroledefinition_create.md)|[<span data-ttu-id="1aae8-122">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1aae8-122">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|<span data-ttu-id="1aae8-123">新しい [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1aae8-123">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="1aae8-124">deviceAndAppManagementRoleDefinition の削除</span><span class="sxs-lookup"><span data-stu-id="1aae8-124">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune_rbac_deviceandappmanagementroledefinition_delete.md)|<span data-ttu-id="1aae8-125">なし</span><span class="sxs-lookup"><span data-stu-id="1aae8-125">None</span></span>|<span data-ttu-id="1aae8-126">[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) の削除</span><span class="sxs-lookup"><span data-stu-id="1aae8-126">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="1aae8-127">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="1aae8-127">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune_rbac_deviceandappmanagementroledefinition_update.md)|[<span data-ttu-id="1aae8-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1aae8-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|<span data-ttu-id="1aae8-129">[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1aae8-129">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1aae8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1aae8-130">Properties</span></span>
|<span data-ttu-id="1aae8-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1aae8-131">Property</span></span>|<span data-ttu-id="1aae8-132">タイプ</span><span class="sxs-lookup"><span data-stu-id="1aae8-132">Type</span></span>|<span data-ttu-id="1aae8-133">説明</span><span class="sxs-lookup"><span data-stu-id="1aae8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aae8-134">ID</span><span class="sxs-lookup"><span data-stu-id="1aae8-134">id</span></span>|<span data-ttu-id="1aae8-135">文字列</span><span class="sxs-lookup"><span data-stu-id="1aae8-135">String</span></span>|<span data-ttu-id="1aae8-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1aae8-136">Key of the entity.</span></span> <span data-ttu-id="1aae8-137">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="1aae8-137">This is read-only and automatically generated.</span></span> <span data-ttu-id="1aae8-138">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1aae8-138">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="1aae8-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1aae8-139">displayName</span></span>|<span data-ttu-id="1aae8-140">文字列</span><span class="sxs-lookup"><span data-stu-id="1aae8-140">String</span></span>|<span data-ttu-id="1aae8-141">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="1aae8-141">Display Name of the Role definition.</span></span> <span data-ttu-id="1aae8-142">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1aae8-142">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="1aae8-143">説明</span><span class="sxs-lookup"><span data-stu-id="1aae8-143">description</span></span>|<span data-ttu-id="1aae8-144">文字列</span><span class="sxs-lookup"><span data-stu-id="1aae8-144">String</span></span>|<span data-ttu-id="1aae8-145">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="1aae8-145">Description of the Role definition.</span></span> <span data-ttu-id="1aae8-146">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1aae8-146">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="1aae8-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="1aae8-147">rolePermissions</span></span>|<span data-ttu-id="1aae8-148">[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1aae8-148">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="1aae8-149">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="1aae8-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="1aae8-150">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1aae8-150">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="1aae8-151">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1aae8-151">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="1aae8-152">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="1aae8-152">isBuiltIn</span></span>|<span data-ttu-id="1aae8-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="1aae8-153">Boolean</span></span>|<span data-ttu-id="1aae8-154">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="1aae8-154">Type of Role.</span></span> <span data-ttu-id="1aae8-155">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="1aae8-155">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="1aae8-156">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1aae8-156">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aae8-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1aae8-157">Relationships</span></span>
|<span data-ttu-id="1aae8-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1aae8-158">Relationship</span></span>|<span data-ttu-id="1aae8-159">型</span><span class="sxs-lookup"><span data-stu-id="1aae8-159">Type</span></span>|<span data-ttu-id="1aae8-160">説明</span><span class="sxs-lookup"><span data-stu-id="1aae8-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aae8-161">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="1aae8-161">roleAssignments</span></span>|<span data-ttu-id="1aae8-162">[roleAssignment](../resources/intune_rbac_roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1aae8-162">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="1aae8-163">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="1aae8-163">List of Role assignments for this role definition.</span></span> <span data-ttu-id="1aae8-164">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1aae8-164">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1aae8-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1aae8-165">JSON Representation</span></span>
<span data-ttu-id="1aae8-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1aae8-166">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.roleDefinition",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}-->
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








