# <a name="roledefinition-resource-type"></a><span data-ttu-id="41432-101">roleDefinition リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="41432-101">roleDefinition resource type</span></span>

> <span data-ttu-id="41432-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="41432-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41432-103">ロールの定義リソースです。</span><span class="sxs-lookup"><span data-stu-id="41432-103">The Role Definition resource.</span></span> <span data-ttu-id="41432-104">ロールの定義は、Intune におけるロール ベース アクセスの基礎です。</span><span class="sxs-lookup"><span data-stu-id="41432-104">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="41432-105">ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="41432-105">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="41432-106">ロールには、組み込みとカスタムの 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="41432-106">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="41432-107">組み込みのロールは変更できません。</span><span class="sxs-lookup"><span data-stu-id="41432-107">Built-in roles cannot be modified.</span></span> <span data-ttu-id="41432-108">組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。</span><span class="sxs-lookup"><span data-stu-id="41432-108">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="41432-109">ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。</span><span class="sxs-lookup"><span data-stu-id="41432-109">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="41432-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="41432-110">Methods</span></span>
|<span data-ttu-id="41432-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="41432-111">Method</span></span>|<span data-ttu-id="41432-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="41432-112">Return Type</span></span>|<span data-ttu-id="41432-113">説明</span><span class="sxs-lookup"><span data-stu-id="41432-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="41432-114">List roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41432-114">List roleDefinitions</span></span>](../api/intune_rbac_roledefinition_list.md)|<span data-ttu-id="41432-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41432-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="41432-116">[roleDefinition](../resources/intune_rbac_roledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="41432-116">List properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="41432-117">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41432-117">Get roleDefinition</span></span>](../api/intune_rbac_roledefinition_get.md)|[<span data-ttu-id="41432-118">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41432-118">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="41432-119">[roleDefinition](../resources/intune_rbac_roledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="41432-119">Read properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="41432-120">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41432-120">Create roleDefinition</span></span>](../api/intune_rbac_roledefinition_create.md)|[<span data-ttu-id="41432-121">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41432-121">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="41432-122">新しい [roleDefinition](../resources/intune_rbac_roledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="41432-122">Create a new [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="41432-123">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41432-123">Delete roleDefinition</span></span>](../api/intune_rbac_roledefinition_delete.md)|<span data-ttu-id="41432-124">なし</span><span class="sxs-lookup"><span data-stu-id="41432-124">None</span></span>|<span data-ttu-id="41432-125">[roleDefinition](../resources/intune_rbac_roledefinition.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="41432-125">Deletes a [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>|
|[<span data-ttu-id="41432-126">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41432-126">Update roleDefinition</span></span>](../api/intune_rbac_roledefinition_update.md)|[<span data-ttu-id="41432-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41432-127">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="41432-128">[roleDefinition](../resources/intune_rbac_roledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="41432-128">Update the properties of a [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="41432-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41432-129">Properties</span></span>
|<span data-ttu-id="41432-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41432-130">Property</span></span>|<span data-ttu-id="41432-131">型</span><span class="sxs-lookup"><span data-stu-id="41432-131">Type</span></span>|<span data-ttu-id="41432-132">説明</span><span class="sxs-lookup"><span data-stu-id="41432-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41432-133">id</span><span class="sxs-lookup"><span data-stu-id="41432-133">id</span></span>|<span data-ttu-id="41432-134">String</span><span class="sxs-lookup"><span data-stu-id="41432-134">String</span></span>|<span data-ttu-id="41432-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="41432-135">Key of the entity.</span></span> <span data-ttu-id="41432-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="41432-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="41432-137">displayName</span><span class="sxs-lookup"><span data-stu-id="41432-137">displayName</span></span>|<span data-ttu-id="41432-138">String</span><span class="sxs-lookup"><span data-stu-id="41432-138">String</span></span>|<span data-ttu-id="41432-139">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="41432-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="41432-140">description</span><span class="sxs-lookup"><span data-stu-id="41432-140">description</span></span>|<span data-ttu-id="41432-141">String</span><span class="sxs-lookup"><span data-stu-id="41432-141">String</span></span>|<span data-ttu-id="41432-142">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="41432-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="41432-143">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="41432-143">rolePermissions</span></span>|<span data-ttu-id="41432-144">[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41432-144">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="41432-145">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="41432-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="41432-146">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="41432-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="41432-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="41432-147">isBuiltIn</span></span>|<span data-ttu-id="41432-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="41432-148">Boolean</span></span>|<span data-ttu-id="41432-149">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="41432-149">Type of Role.</span></span> <span data-ttu-id="41432-150">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="41432-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41432-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41432-151">Relationships</span></span>
|<span data-ttu-id="41432-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41432-152">Relationship</span></span>|<span data-ttu-id="41432-153">型</span><span class="sxs-lookup"><span data-stu-id="41432-153">Type</span></span>|<span data-ttu-id="41432-154">説明</span><span class="sxs-lookup"><span data-stu-id="41432-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41432-155">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="41432-155">roleAssignments</span></span>|<span data-ttu-id="41432-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41432-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="41432-157">このロールの定義の、ロールの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="41432-157">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41432-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41432-158">JSON Representation</span></span>
<span data-ttu-id="41432-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41432-159">Here is a JSON representation of the resource.</span></span>
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



