# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="96ee9-101">deviceCompliancePolicyDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96ee9-101">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="96ee9-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="96ee9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96ee9-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="96ee9-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="96ee9-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="96ee9-104">Methods</span></span>
|<span data-ttu-id="96ee9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="96ee9-105">Method</span></span>|<span data-ttu-id="96ee9-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="96ee9-106">Return Type</span></span>|<span data-ttu-id="96ee9-107">説明</span><span class="sxs-lookup"><span data-stu-id="96ee9-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96ee9-108">deviceCompliancePolicyDeviceStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="96ee9-108">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_get.md)|[<span data-ttu-id="96ee9-109">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="96ee9-109">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="96ee9-110">[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="96ee9-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="96ee9-111">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="96ee9-111">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_update.md)|[<span data-ttu-id="96ee9-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="96ee9-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="96ee9-113">[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="96ee9-113">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96ee9-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96ee9-114">Properties</span></span>
|<span data-ttu-id="96ee9-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96ee9-115">Property</span></span>|<span data-ttu-id="96ee9-116">型</span><span class="sxs-lookup"><span data-stu-id="96ee9-116">Type</span></span>|<span data-ttu-id="96ee9-117">説明</span><span class="sxs-lookup"><span data-stu-id="96ee9-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96ee9-118">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-118">inGracePeriodCount</span></span>|<span data-ttu-id="96ee9-119">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-119">Int32</span></span>|<span data-ttu-id="96ee9-120">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-120">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="96ee9-121">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-121">configManagerCount</span></span>|<span data-ttu-id="96ee9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-122">Int32</span></span>|<span data-ttu-id="96ee9-123">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-123">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="96ee9-124">id</span><span class="sxs-lookup"><span data-stu-id="96ee9-124">id</span></span>|<span data-ttu-id="96ee9-125">String</span><span class="sxs-lookup"><span data-stu-id="96ee9-125">String</span></span>|<span data-ttu-id="96ee9-126">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="96ee9-126">Name of the entity.</span></span>|
|<span data-ttu-id="96ee9-127">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-127">unknownDeviceCount</span></span>|<span data-ttu-id="96ee9-128">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-128">Int32</span></span>|<span data-ttu-id="96ee9-129">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-129">Number of unknown devices</span></span>|
|<span data-ttu-id="96ee9-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="96ee9-131">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-131">Int32</span></span>|<span data-ttu-id="96ee9-132">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-132">Number of not applicable devices</span></span>|
|<span data-ttu-id="96ee9-133">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-133">compliantDeviceCount</span></span>|<span data-ttu-id="96ee9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-134">Int32</span></span>|<span data-ttu-id="96ee9-135">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-135">Number of compliant devices</span></span>|
|<span data-ttu-id="96ee9-136">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-136">remediatedDeviceCount</span></span>|<span data-ttu-id="96ee9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-137">Int32</span></span>|<span data-ttu-id="96ee9-138">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-138">Number of remediated devices</span></span>|
|<span data-ttu-id="96ee9-139">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-139">nonCompliantDeviceCount</span></span>|<span data-ttu-id="96ee9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-140">Int32</span></span>|<span data-ttu-id="96ee9-141">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-141">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="96ee9-142">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-142">errorDeviceCount</span></span>|<span data-ttu-id="96ee9-143">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-143">Int32</span></span>|<span data-ttu-id="96ee9-144">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-144">Number of error devices</span></span>|
|<span data-ttu-id="96ee9-145">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ee9-145">conflictDeviceCount</span></span>|<span data-ttu-id="96ee9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="96ee9-146">Int32</span></span>|<span data-ttu-id="96ee9-147">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="96ee9-147">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="96ee9-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96ee9-148">Relationships</span></span>
<span data-ttu-id="96ee9-149">なし</span><span class="sxs-lookup"><span data-stu-id="96ee9-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96ee9-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96ee9-150">JSON Representation</span></span>
<span data-ttu-id="96ee9-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96ee9-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



