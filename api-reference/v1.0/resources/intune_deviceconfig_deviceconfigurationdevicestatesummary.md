# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="5c79b-101">deviceConfigurationDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c79b-101">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="5c79b-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c79b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c79b-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5c79b-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="5c79b-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="5c79b-104">Methods</span></span>
|<span data-ttu-id="5c79b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5c79b-105">Method</span></span>|<span data-ttu-id="5c79b-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5c79b-106">Return Type</span></span>|<span data-ttu-id="5c79b-107">説明</span><span class="sxs-lookup"><span data-stu-id="5c79b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c79b-108">Get deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="5c79b-108">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_get.md)|[<span data-ttu-id="5c79b-109">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="5c79b-109">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="5c79b-110">[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5c79b-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="5c79b-111">Update deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="5c79b-111">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_update.md)|[<span data-ttu-id="5c79b-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="5c79b-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="5c79b-113">[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5c79b-113">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c79b-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c79b-114">Properties</span></span>
|<span data-ttu-id="5c79b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c79b-115">Property</span></span>|<span data-ttu-id="5c79b-116">型</span><span class="sxs-lookup"><span data-stu-id="5c79b-116">Type</span></span>|<span data-ttu-id="5c79b-117">説明</span><span class="sxs-lookup"><span data-stu-id="5c79b-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c79b-118">id</span><span class="sxs-lookup"><span data-stu-id="5c79b-118">id</span></span>|<span data-ttu-id="5c79b-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5c79b-119">String</span></span>|<span data-ttu-id="5c79b-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5c79b-120">Name of the entity.</span></span>|
|<span data-ttu-id="5c79b-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c79b-121">unknownDeviceCount</span></span>|<span data-ttu-id="5c79b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="5c79b-122">Int32</span></span>|<span data-ttu-id="5c79b-123">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5c79b-123">Number of unknown devices</span></span>|
|<span data-ttu-id="5c79b-124">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c79b-124">notApplicableDeviceCount</span></span>|<span data-ttu-id="5c79b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="5c79b-125">Int32</span></span>|<span data-ttu-id="5c79b-126">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5c79b-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="5c79b-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c79b-127">compliantDeviceCount</span></span>|<span data-ttu-id="5c79b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5c79b-128">Int32</span></span>|<span data-ttu-id="5c79b-129">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5c79b-129">Number of compliant devices</span></span>|
|<span data-ttu-id="5c79b-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c79b-130">remediatedDeviceCount</span></span>|<span data-ttu-id="5c79b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5c79b-131">Int32</span></span>|<span data-ttu-id="5c79b-132">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5c79b-132">Number of remediated devices</span></span>|
|<span data-ttu-id="5c79b-133">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c79b-133">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5c79b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="5c79b-134">Int32</span></span>|<span data-ttu-id="5c79b-135">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5c79b-135">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="5c79b-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c79b-136">errorDeviceCount</span></span>|<span data-ttu-id="5c79b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5c79b-137">Int32</span></span>|<span data-ttu-id="5c79b-138">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5c79b-138">Number of error devices</span></span>|
|<span data-ttu-id="5c79b-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c79b-139">conflictDeviceCount</span></span>|<span data-ttu-id="5c79b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5c79b-140">Int32</span></span>|<span data-ttu-id="5c79b-141">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5c79b-141">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c79b-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5c79b-142">Relationships</span></span>
<span data-ttu-id="5c79b-143">なし</span><span class="sxs-lookup"><span data-stu-id="5c79b-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5c79b-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c79b-144">JSON Representation</span></span>
<span data-ttu-id="5c79b-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c79b-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
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



