# <a name="roleassignment-resource-type"></a><span data-ttu-id="7efe6-101">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7efe6-101">roleAssignment resource type</span></span>

> <span data-ttu-id="7efe6-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7efe6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7efe6-103">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="7efe6-103">The Role Assignment resource.</span></span> <span data-ttu-id="7efe6-104">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="7efe6-104">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="7efe6-105">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="7efe6-105">There can be one or more role assignments per role.</span></span> <span data-ttu-id="7efe6-106">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7efe6-106">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="7efe6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7efe6-107">Methods</span></span>
|<span data-ttu-id="7efe6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7efe6-108">Method</span></span>|<span data-ttu-id="7efe6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7efe6-109">Return Type</span></span>|<span data-ttu-id="7efe6-110">説明</span><span class="sxs-lookup"><span data-stu-id="7efe6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7efe6-111">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="7efe6-111">List roleAssignments</span></span>](../api/intune_rbac_roleassignment_list.md)|<span data-ttu-id="7efe6-112">[roleAssignment](../resources/intune_rbac_roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7efe6-112">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="7efe6-113">[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7efe6-113">List properties and relationships of the [roleAssignment](../resources/intune_rbac_roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="7efe6-114">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="7efe6-114">Get roleAssignment</span></span>](../api/intune_rbac_roleassignment_get.md)|[<span data-ttu-id="7efe6-115">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="7efe6-115">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="7efe6-116">[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7efe6-116">Read properties and relationships of the [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|
|[<span data-ttu-id="7efe6-117">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="7efe6-117">Create roleAssignment</span></span>](../api/intune_rbac_roleassignment_create.md)|[<span data-ttu-id="7efe6-118">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="7efe6-118">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="7efe6-119">新しい [roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7efe6-119">Create a new [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|
|[<span data-ttu-id="7efe6-120">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="7efe6-120">Delete roleAssignment</span></span>](../api/intune_rbac_roleassignment_delete.md)|<span data-ttu-id="7efe6-121">なし</span><span class="sxs-lookup"><span data-stu-id="7efe6-121">None</span></span>|<span data-ttu-id="7efe6-122">[roleAssignment](../resources/intune_rbac_roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7efe6-122">Deletes a [roleAssignment](../resources/intune_rbac_roleassignment.md).</span></span>|
|[<span data-ttu-id="7efe6-123">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="7efe6-123">Update roleAssignment</span></span>](../api/intune_rbac_roleassignment_update.md)|[<span data-ttu-id="7efe6-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="7efe6-124">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="7efe6-125">[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7efe6-125">Update the properties of a [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7efe6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7efe6-126">Properties</span></span>
|<span data-ttu-id="7efe6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7efe6-127">Property</span></span>|<span data-ttu-id="7efe6-128">タイプ</span><span class="sxs-lookup"><span data-stu-id="7efe6-128">Type</span></span>|<span data-ttu-id="7efe6-129">説明</span><span class="sxs-lookup"><span data-stu-id="7efe6-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7efe6-130">id</span><span class="sxs-lookup"><span data-stu-id="7efe6-130">id</span></span>|<span data-ttu-id="7efe6-131">文字列</span><span class="sxs-lookup"><span data-stu-id="7efe6-131">String</span></span>|<span data-ttu-id="7efe6-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7efe6-132">Key of the entity.</span></span> <span data-ttu-id="7efe6-133">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="7efe6-133">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="7efe6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7efe6-134">displayName</span></span>|<span data-ttu-id="7efe6-135">文字列</span><span class="sxs-lookup"><span data-stu-id="7efe6-135">String</span></span>|<span data-ttu-id="7efe6-136">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="7efe6-136">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="7efe6-137">説明</span><span class="sxs-lookup"><span data-stu-id="7efe6-137">description</span></span>|<span data-ttu-id="7efe6-138">文字列</span><span class="sxs-lookup"><span data-stu-id="7efe6-138">String</span></span>|<span data-ttu-id="7efe6-139">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="7efe6-139">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="7efe6-140">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="7efe6-140">resourceScopes</span></span>|<span data-ttu-id="7efe6-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7efe6-141">String collection</span></span>|<span data-ttu-id="7efe6-142">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="7efe6-142">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7efe6-143">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="7efe6-143">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7efe6-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7efe6-144">Relationships</span></span>
|<span data-ttu-id="7efe6-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7efe6-145">Relationship</span></span>|<span data-ttu-id="7efe6-146">型</span><span class="sxs-lookup"><span data-stu-id="7efe6-146">Type</span></span>|<span data-ttu-id="7efe6-147">説明</span><span class="sxs-lookup"><span data-stu-id="7efe6-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7efe6-148">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7efe6-148">roleDefinition</span></span>|[<span data-ttu-id="7efe6-149">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7efe6-149">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="7efe6-150">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="7efe6-150">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7efe6-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7efe6-151">JSON Representation</span></span>
<span data-ttu-id="7efe6-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7efe6-152">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.roleAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



