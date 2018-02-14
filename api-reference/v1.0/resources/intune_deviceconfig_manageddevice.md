# <a name="manageddevice-resource-type"></a><span data-ttu-id="ea5c2-101">managedDevice リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ea5c2-101">managedDevice resource type</span></span>

> <span data-ttu-id="ea5c2-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ea5c2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea5c2-103">Intune 経由で管理または事前登録されるデバイス</span><span class="sxs-lookup"><span data-stu-id="ea5c2-103">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="ea5c2-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="ea5c2-104">Methods</span></span>
|<span data-ttu-id="ea5c2-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ea5c2-105">Method</span></span>|<span data-ttu-id="ea5c2-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ea5c2-106">Return Type</span></span>|<span data-ttu-id="ea5c2-107">説明</span><span class="sxs-lookup"><span data-stu-id="ea5c2-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea5c2-108">List managedDevices</span><span class="sxs-lookup"><span data-stu-id="ea5c2-108">List managedDevices</span></span>](../api/intune_deviceconfig_manageddevice_list.md)|<span data-ttu-id="ea5c2-109">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ea5c2-109">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) collection</span></span>|<span data-ttu-id="ea5c2-110">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ea5c2-110">List properties and relationships of the [managedDevice](../resources/intune_deviceconfig_manageddevice.md) objects.</span></span>|
|[<span data-ttu-id="ea5c2-111">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="ea5c2-111">Get managedDevice</span></span>](../api/intune_deviceconfig_manageddevice_get.md)|[<span data-ttu-id="ea5c2-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="ea5c2-112">managedDevice</span></span>](../resources/intune_deviceconfig_manageddevice.md)|<span data-ttu-id="ea5c2-113">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ea5c2-113">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_manageddevice.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea5c2-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea5c2-114">Properties</span></span>
|<span data-ttu-id="ea5c2-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea5c2-115">Property</span></span>|<span data-ttu-id="ea5c2-116">型</span><span class="sxs-lookup"><span data-stu-id="ea5c2-116">Type</span></span>|<span data-ttu-id="ea5c2-117">説明</span><span class="sxs-lookup"><span data-stu-id="ea5c2-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea5c2-118">id</span><span class="sxs-lookup"><span data-stu-id="ea5c2-118">id</span></span>|<span data-ttu-id="ea5c2-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ea5c2-119">String</span></span>|<span data-ttu-id="ea5c2-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ea5c2-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea5c2-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ea5c2-121">Relationships</span></span>
|<span data-ttu-id="ea5c2-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ea5c2-122">Relationship</span></span>|<span data-ttu-id="ea5c2-123">型</span><span class="sxs-lookup"><span data-stu-id="ea5c2-123">Type</span></span>|<span data-ttu-id="ea5c2-124">説明</span><span class="sxs-lookup"><span data-stu-id="ea5c2-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea5c2-125">deviceConfigurationStates</span><span class="sxs-lookup"><span data-stu-id="ea5c2-125">deviceConfigurationStates</span></span>|<span data-ttu-id="ea5c2-126">[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ea5c2-126">[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) collection</span></span>|<span data-ttu-id="ea5c2-127">対象デバイスのデバイス構成の状態。</span><span class="sxs-lookup"><span data-stu-id="ea5c2-127">Device configuration states for this device.</span></span>|
|<span data-ttu-id="ea5c2-128">deviceCompliancePolicyStates</span><span class="sxs-lookup"><span data-stu-id="ea5c2-128">deviceCompliancePolicyStates</span></span>|<span data-ttu-id="ea5c2-129">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ea5c2-129">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) collection</span></span>|<span data-ttu-id="ea5c2-130">対象デバイスのデバイス コンプライアンス ポリシーの状態。</span><span class="sxs-lookup"><span data-stu-id="ea5c2-130">Device compliance policy states for this device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea5c2-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ea5c2-131">JSON Representation</span></span>
<span data-ttu-id="ea5c2-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ea5c2-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



