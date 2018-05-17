# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="6fb15-101">deviceCompliancePolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6fb15-101">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="6fb15-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6fb15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fb15-103">デバイス コンプライアンス ポリシーの割り当てです。</span><span class="sxs-lookup"><span data-stu-id="6fb15-103">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="6fb15-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="6fb15-104">Methods</span></span>
|<span data-ttu-id="6fb15-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6fb15-105">Method</span></span>|<span data-ttu-id="6fb15-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6fb15-106">Return Type</span></span>|<span data-ttu-id="6fb15-107">説明</span><span class="sxs-lookup"><span data-stu-id="6fb15-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fb15-108">deviceCompliancePolicyAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="6fb15-108">List deviceCompliancePolicyAssignments</span></span>](../api/intune_deviceconfig_devicecompliancepolicyassignment_list.md)|<span data-ttu-id="6fb15-109">[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6fb15-109">[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="6fb15-110">[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6fb15-110">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="6fb15-111">deviceCompliancePolicyAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="6fb15-111">Get deviceCompliancePolicyAssignment</span></span>](../api/intune_deviceconfig_devicecompliancepolicyassignment_get.md)|[<span data-ttu-id="6fb15-112">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6fb15-112">deviceCompliancePolicyAssignment</span></span>](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|<span data-ttu-id="6fb15-113">[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6fb15-113">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="6fb15-114">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="6fb15-114">Create deviceCompliancePolicyAssignment</span></span>](../api/intune_deviceconfig_devicecompliancepolicyassignment_create.md)|[<span data-ttu-id="6fb15-115">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6fb15-115">deviceCompliancePolicyAssignment</span></span>](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|<span data-ttu-id="6fb15-116">新しい [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6fb15-116">Create a new [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="6fb15-117">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="6fb15-117">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune_deviceconfig_devicecompliancepolicyassignment_delete.md)|<span data-ttu-id="6fb15-118">なし</span><span class="sxs-lookup"><span data-stu-id="6fb15-118">None</span></span>|<span data-ttu-id="6fb15-119">[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6fb15-119">Deletes a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="6fb15-120">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="6fb15-120">Update deviceCompliancePolicyAssignment</span></span>](../api/intune_deviceconfig_devicecompliancepolicyassignment_update.md)|[<span data-ttu-id="6fb15-121">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6fb15-121">deviceCompliancePolicyAssignment</span></span>](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|<span data-ttu-id="6fb15-122">[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6fb15-122">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6fb15-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fb15-123">Properties</span></span>
|<span data-ttu-id="6fb15-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fb15-124">Property</span></span>|<span data-ttu-id="6fb15-125">型</span><span class="sxs-lookup"><span data-stu-id="6fb15-125">Type</span></span>|<span data-ttu-id="6fb15-126">説明</span><span class="sxs-lookup"><span data-stu-id="6fb15-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb15-127">id</span><span class="sxs-lookup"><span data-stu-id="6fb15-127">id</span></span>|<span data-ttu-id="6fb15-128">String</span><span class="sxs-lookup"><span data-stu-id="6fb15-128">String</span></span>|<span data-ttu-id="6fb15-129">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6fb15-129">Key of the entity.</span></span>|
|<span data-ttu-id="6fb15-130">target</span><span class="sxs-lookup"><span data-stu-id="6fb15-130">target</span></span>|[<span data-ttu-id="6fb15-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6fb15-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6fb15-132">デバイス コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="6fb15-132">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fb15-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6fb15-133">Relationships</span></span>
<span data-ttu-id="6fb15-134">なし</span><span class="sxs-lookup"><span data-stu-id="6fb15-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6fb15-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6fb15-135">JSON Representation</span></span>
<span data-ttu-id="6fb15-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6fb15-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



