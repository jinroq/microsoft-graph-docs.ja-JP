# <a name="devicemanagement-resource-type"></a><span data-ttu-id="e394a-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e394a-101">deviceManagement resource type</span></span>

> <span data-ttu-id="e394a-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e394a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e394a-103">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="e394a-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="e394a-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="e394a-104">Methods</span></span>
|<span data-ttu-id="e394a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e394a-105">Method</span></span>|<span data-ttu-id="e394a-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e394a-106">Return Type</span></span>|<span data-ttu-id="e394a-107">説明</span><span class="sxs-lookup"><span data-stu-id="e394a-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e394a-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e394a-108">Get deviceManagement</span></span>](../api/intune_rbac_devicemanagement_get.md)|[<span data-ttu-id="e394a-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e394a-109">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="e394a-110">[deviceManagement](../resources/intune_rbac_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e394a-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="e394a-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e394a-111">Update deviceManagement</span></span>](../api/intune_rbac_devicemanagement_update.md)|[<span data-ttu-id="e394a-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e394a-112">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="e394a-113">[deviceManagement](../resources/intune_rbac_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e394a-113">Update the properties of a [calendar](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="e394a-114">getEffectivePermissions 関数</span><span class="sxs-lookup"><span data-stu-id="e394a-114">getEffectivePermissions function</span></span>](../api/intune_rbac_devicemanagement_geteffectivepermissions.md)|<span data-ttu-id="e394a-115">[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e394a-115">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="e394a-116">現在の認証ユーザーの有効なアクセス許可を取得します</span><span class="sxs-lookup"><span data-stu-id="e394a-116">Retrieves the effective permissions of the currently authenticated user</span></span>|

## <a name="properties"></a><span data-ttu-id="e394a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e394a-117">Properties</span></span>
|<span data-ttu-id="e394a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e394a-118">Property</span></span>|<span data-ttu-id="e394a-119">型</span><span class="sxs-lookup"><span data-stu-id="e394a-119">Type</span></span>|<span data-ttu-id="e394a-120">説明</span><span class="sxs-lookup"><span data-stu-id="e394a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e394a-121">id</span><span class="sxs-lookup"><span data-stu-id="e394a-121">id</span></span>|<span data-ttu-id="e394a-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e394a-122">String</span></span>|<span data-ttu-id="e394a-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e394a-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="e394a-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e394a-124">Relationships</span></span>
|<span data-ttu-id="e394a-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e394a-125">Relationship</span></span>|<span data-ttu-id="e394a-126">型</span><span class="sxs-lookup"><span data-stu-id="e394a-126">Type</span></span>|<span data-ttu-id="e394a-127">説明</span><span class="sxs-lookup"><span data-stu-id="e394a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e394a-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="e394a-128">roleDefinitions</span></span>|<span data-ttu-id="e394a-129">[roleDefinition](../resources/intune_rbac_roledefinition.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e394a-129">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="e394a-130">ロールの定義。</span><span class="sxs-lookup"><span data-stu-id="e394a-130">The Role Definitions.</span></span>|
|<span data-ttu-id="e394a-131">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="e394a-131">roleAssignments</span></span>|<span data-ttu-id="e394a-132">[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e394a-132">[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="e394a-133">ロールの割り当て。</span><span class="sxs-lookup"><span data-stu-id="e394a-133">The Role Assignments.</span></span>|
|<span data-ttu-id="e394a-134">resourceOperations</span><span class="sxs-lookup"><span data-stu-id="e394a-134">resourceOperations</span></span>|<span data-ttu-id="e394a-135">[resourceOperation](../resources/intune_rbac_resourceoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e394a-135">[resourceOperation](../resources/intune_rbac_resourceoperation.md) collection</span></span>|<span data-ttu-id="e394a-136">リソースの操作。</span><span class="sxs-lookup"><span data-stu-id="e394a-136">The Resource Operations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e394a-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e394a-137">JSON Representation</span></span>
<span data-ttu-id="e394a-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e394a-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



