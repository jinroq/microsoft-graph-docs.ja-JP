# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="b162b-101">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b162b-101">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="b162b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b162b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b162b-103">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="b162b-103">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="b162b-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="b162b-104">Methods</span></span>
|<span data-ttu-id="b162b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b162b-105">Method</span></span>|<span data-ttu-id="b162b-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b162b-106">Return Type</span></span>|<span data-ttu-id="b162b-107">説明</span><span class="sxs-lookup"><span data-stu-id="b162b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b162b-108">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="b162b-108">List deviceConfigurationAssignments</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|<span data-ttu-id="b162b-109">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b162b-109">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b162b-110">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b162b-110">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="b162b-111">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="b162b-111">Get deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[<span data-ttu-id="b162b-112">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b162b-112">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="b162b-113">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b162b-113">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b162b-114">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="b162b-114">Create deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[<span data-ttu-id="b162b-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b162b-115">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="b162b-116">新しい [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b162b-116">Create a new [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b162b-117">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="b162b-117">Delete deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|<span data-ttu-id="b162b-118">なし</span><span class="sxs-lookup"><span data-stu-id="b162b-118">None</span></span>|<span data-ttu-id="b162b-119">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b162b-119">Deletes a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="b162b-120">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="b162b-120">Update deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[<span data-ttu-id="b162b-121">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b162b-121">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="b162b-122">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b162b-122">Update the properties of a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b162b-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b162b-123">Properties</span></span>
|<span data-ttu-id="b162b-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b162b-124">Property</span></span>|<span data-ttu-id="b162b-125">型</span><span class="sxs-lookup"><span data-stu-id="b162b-125">Type</span></span>|<span data-ttu-id="b162b-126">説明</span><span class="sxs-lookup"><span data-stu-id="b162b-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b162b-127">id</span><span class="sxs-lookup"><span data-stu-id="b162b-127">id</span></span>|<span data-ttu-id="b162b-128">String</span><span class="sxs-lookup"><span data-stu-id="b162b-128">String</span></span>|<span data-ttu-id="b162b-129">割り当てのキーです。</span><span class="sxs-lookup"><span data-stu-id="b162b-129">The key of the assignment.</span></span>|
|<span data-ttu-id="b162b-130">target</span><span class="sxs-lookup"><span data-stu-id="b162b-130">target</span></span>|[<span data-ttu-id="b162b-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b162b-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b162b-132">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="b162b-132">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b162b-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b162b-133">Relationships</span></span>
<span data-ttu-id="b162b-134">なし</span><span class="sxs-lookup"><span data-stu-id="b162b-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b162b-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b162b-135">JSON Representation</span></span>
<span data-ttu-id="b162b-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b162b-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



