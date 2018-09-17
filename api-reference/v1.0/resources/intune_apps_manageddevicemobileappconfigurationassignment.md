# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="1aad7-101">managedDeviceMobileAppConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1aad7-101">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="1aad7-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1aad7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1aad7-103">グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1aad7-103">Contains the properties used to assign an MDM app configuration to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="1aad7-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="1aad7-104">Methods</span></span>
|<span data-ttu-id="1aad7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1aad7-105">Method</span></span>|<span data-ttu-id="1aad7-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1aad7-106">Return Type</span></span>|<span data-ttu-id="1aad7-107">説明</span><span class="sxs-lookup"><span data-stu-id="1aad7-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1aad7-108">managedDeviceMobileAppConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="1aad7-108">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune_apps_manageddevicemobileappconfigurationassignment_list.md)|<span data-ttu-id="1aad7-109">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1aad7-109">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1aad7-110">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1aad7-110">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="1aad7-111">managedDeviceMobileAppConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="1aad7-111">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune_apps_manageddevicemobileappconfigurationassignment_get.md)|[<span data-ttu-id="1aad7-112">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1aad7-112">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="1aad7-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1aad7-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="1aad7-114">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="1aad7-114">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune_apps_manageddevicemobileappconfigurationassignment_create.md)|[<span data-ttu-id="1aad7-115">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1aad7-115">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="1aad7-116">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1aad7-116">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="1aad7-117">managedDeviceMobileAppConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="1aad7-117">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune_apps_manageddevicemobileappconfigurationassignment_delete.md)|<span data-ttu-id="1aad7-118">なし</span><span class="sxs-lookup"><span data-stu-id="1aad7-118">None</span></span>|<span data-ttu-id="1aad7-119">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1aad7-119">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="1aad7-120">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="1aad7-120">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune_apps_manageddevicemobileappconfigurationassignment_update.md)|[<span data-ttu-id="1aad7-121">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1aad7-121">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="1aad7-122">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1aad7-122">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1aad7-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1aad7-123">Properties</span></span>
|<span data-ttu-id="1aad7-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1aad7-124">Property</span></span>|<span data-ttu-id="1aad7-125">タイプ</span><span class="sxs-lookup"><span data-stu-id="1aad7-125">Type</span></span>|<span data-ttu-id="1aad7-126">説明</span><span class="sxs-lookup"><span data-stu-id="1aad7-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aad7-127">ID</span><span class="sxs-lookup"><span data-stu-id="1aad7-127">id</span></span>|<span data-ttu-id="1aad7-128">文字列</span><span class="sxs-lookup"><span data-stu-id="1aad7-128">String</span></span>|<span data-ttu-id="1aad7-129">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1aad7-129">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1aad7-130">ターゲット</span><span class="sxs-lookup"><span data-stu-id="1aad7-130">target</span></span>|[<span data-ttu-id="1aad7-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1aad7-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1aad7-132">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="1aad7-132">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aad7-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1aad7-133">Relationships</span></span>
<span data-ttu-id="1aad7-134">なし</span><span class="sxs-lookup"><span data-stu-id="1aad7-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1aad7-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1aad7-135">JSON Representation</span></span>
<span data-ttu-id="1aad7-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1aad7-136">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








