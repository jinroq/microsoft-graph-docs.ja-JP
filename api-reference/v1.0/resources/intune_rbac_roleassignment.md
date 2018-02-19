# <a name="roleassignment-resource-type"></a><span data-ttu-id="fbfd8-101">roleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbfd8-101">roleAssignment resource type</span></span>

> <span data-ttu-id="fbfd8-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbfd8-103">役割の割り当てリソースです。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-103">The Role Assignment resource.</span></span> <span data-ttu-id="fbfd8-104">役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-104">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="fbfd8-105">役割ごとに 1 つまたは複数の役割の割り当てが可能です。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-105">There can be one or more role assignments per role.</span></span> <span data-ttu-id="fbfd8-106">カスタムおよび組み込みの役割に適用されます。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-106">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="fbfd8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fbfd8-107">Methods</span></span>
|<span data-ttu-id="fbfd8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fbfd8-108">Method</span></span>|<span data-ttu-id="fbfd8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fbfd8-109">Return Type</span></span>|<span data-ttu-id="fbfd8-110">説明</span><span class="sxs-lookup"><span data-stu-id="fbfd8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fbfd8-111">roleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="fbfd8-111">List roleAssignments</span></span>](../api/intune_rbac_roleassignment_list.md)|<span data-ttu-id="fbfd8-112">[roleAssignment](../resources/intune_rbac_roleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbfd8-112">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="fbfd8-113">[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-113">List properties and relationships of the [roleAssignment](../resources/intune_rbac_roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="fbfd8-114">roleAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="fbfd8-114">Get roleAssignment</span></span>](../api/intune_rbac_roleassignment_get.md)|[<span data-ttu-id="fbfd8-115">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fbfd8-115">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="fbfd8-116">[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-116">Read properties and relationships of [plannerTaskDetails](../resources/intune_rbac_roleassignment.md) object.</span></span>|
|[<span data-ttu-id="fbfd8-117">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="fbfd8-117">Create roleAssignment</span></span>](../api/intune_rbac_roleassignment_create.md)|[<span data-ttu-id="fbfd8-118">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fbfd8-118">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="fbfd8-119">新しい [roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-119">Create a new [plannerBucket](../resources/intune_rbac_roleassignment.md) object.</span></span>|
|[<span data-ttu-id="fbfd8-120">roleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="fbfd8-120">Delete roleAssignment</span></span>](../api/intune_rbac_roleassignment_delete.md)|<span data-ttu-id="fbfd8-121">なし</span><span class="sxs-lookup"><span data-stu-id="fbfd8-121">None</span></span>|<span data-ttu-id="fbfd8-122">[roleAssignment](../resources/intune_rbac_roleassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-122">Deletes a [roleAssignment](../resources/intune_rbac_roleassignment.md).</span></span>|
|[<span data-ttu-id="fbfd8-123">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="fbfd8-123">Update roleAssignment</span></span>](../api/intune_rbac_roleassignment_update.md)|[<span data-ttu-id="fbfd8-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="fbfd8-124">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="fbfd8-125">[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-125">Update the properties of a [calendar](../resources/intune_rbac_roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fbfd8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbfd8-126">Properties</span></span>
|<span data-ttu-id="fbfd8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbfd8-127">Property</span></span>|<span data-ttu-id="fbfd8-128">型</span><span class="sxs-lookup"><span data-stu-id="fbfd8-128">Type</span></span>|<span data-ttu-id="fbfd8-129">説明</span><span class="sxs-lookup"><span data-stu-id="fbfd8-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbfd8-130">id</span><span class="sxs-lookup"><span data-stu-id="fbfd8-130">id</span></span>|<span data-ttu-id="fbfd8-131">String</span><span class="sxs-lookup"><span data-stu-id="fbfd8-131">String</span></span>|<span data-ttu-id="fbfd8-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-132">Name of the entity.</span></span> <span data-ttu-id="fbfd8-133">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-133">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="fbfd8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fbfd8-134">displayName</span></span>|<span data-ttu-id="fbfd8-135">String</span><span class="sxs-lookup"><span data-stu-id="fbfd8-135">String</span></span>|<span data-ttu-id="fbfd8-136">役割の割り当ての表示名またはフレンドリ名です。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-136">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="fbfd8-137">description</span><span class="sxs-lookup"><span data-stu-id="fbfd8-137">description</span></span>|<span data-ttu-id="fbfd8-138">String</span><span class="sxs-lookup"><span data-stu-id="fbfd8-138">String</span></span>|<span data-ttu-id="fbfd8-139">役割の割り当ての説明です。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-139">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="fbfd8-140">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fbfd8-140">resourceScopes</span></span>|<span data-ttu-id="fbfd8-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fbfd8-141">String collection</span></span>|<span data-ttu-id="fbfd8-142">役割のスコープ メンバーのセキュリティ グループの ID リストです。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-142">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fbfd8-143">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-143">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbfd8-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbfd8-144">Relationships</span></span>
|<span data-ttu-id="fbfd8-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbfd8-145">Relationship</span></span>|<span data-ttu-id="fbfd8-146">型</span><span class="sxs-lookup"><span data-stu-id="fbfd8-146">Type</span></span>|<span data-ttu-id="fbfd8-147">説明</span><span class="sxs-lookup"><span data-stu-id="fbfd8-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbfd8-148">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fbfd8-148">roleDefinition</span></span>|[<span data-ttu-id="fbfd8-149">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fbfd8-149">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="fbfd8-150">この割り当てが含まれる役割の定義。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-150">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbfd8-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbfd8-151">JSON Representation</span></span>
<span data-ttu-id="fbfd8-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fbfd8-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
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



