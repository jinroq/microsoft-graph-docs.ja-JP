# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="e5575-101">deviceConfigurationDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5575-101">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="e5575-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5575-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5575-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e5575-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="e5575-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5575-104">Methods</span></span>
|<span data-ttu-id="e5575-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5575-105">Method</span></span>|<span data-ttu-id="e5575-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e5575-106">Return Type</span></span>|<span data-ttu-id="e5575-107">説明</span><span class="sxs-lookup"><span data-stu-id="e5575-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5575-108">deviceConfigurationDeviceStateSummaryを取得する</span><span class="sxs-lookup"><span data-stu-id="e5575-108">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_get.md)|[<span data-ttu-id="e5575-109">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e5575-109">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="e5575-110">[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e5575-110">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="e5575-111">deviceConfigurationDeviceStateSummaryを更新する</span><span class="sxs-lookup"><span data-stu-id="e5575-111">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune_deviceconfig_deviceconfigurationdevicestatesummary_update.md)|[<span data-ttu-id="e5575-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e5575-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="e5575-113">[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5575-113">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5575-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5575-114">Properties</span></span>
|<span data-ttu-id="e5575-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5575-115">Property</span></span>|<span data-ttu-id="e5575-116">型</span><span class="sxs-lookup"><span data-stu-id="e5575-116">Type</span></span>|<span data-ttu-id="e5575-117">説明</span><span class="sxs-lookup"><span data-stu-id="e5575-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5575-118">ID</span><span class="sxs-lookup"><span data-stu-id="e5575-118">id</span></span>|<span data-ttu-id="e5575-119">文字列</span><span class="sxs-lookup"><span data-stu-id="e5575-119">String</span></span>|<span data-ttu-id="e5575-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e5575-120">Key of the entity.</span></span>|
|<span data-ttu-id="e5575-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5575-121">unknownDeviceCount</span></span>|<span data-ttu-id="e5575-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e5575-122">Int32</span></span>|<span data-ttu-id="e5575-123">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e5575-123">Number of unknown devices</span></span>|
|<span data-ttu-id="e5575-124">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5575-124">notApplicableDeviceCount</span></span>|<span data-ttu-id="e5575-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e5575-125">Int32</span></span>|<span data-ttu-id="e5575-126">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e5575-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="e5575-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5575-127">compliantDeviceCount</span></span>|<span data-ttu-id="e5575-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e5575-128">Int32</span></span>|<span data-ttu-id="e5575-129">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e5575-129">Number of compliant devices</span></span>|
|<span data-ttu-id="e5575-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5575-130">remediatedDeviceCount</span></span>|<span data-ttu-id="e5575-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e5575-131">Int32</span></span>|<span data-ttu-id="e5575-132">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e5575-132">Number of remediated devices</span></span>|
|<span data-ttu-id="e5575-133">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5575-133">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e5575-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e5575-134">Int32</span></span>|<span data-ttu-id="e5575-135">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e5575-135">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e5575-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5575-136">errorDeviceCount</span></span>|<span data-ttu-id="e5575-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e5575-137">Int32</span></span>|<span data-ttu-id="e5575-138">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e5575-138">Number of error devices</span></span>|
|<span data-ttu-id="e5575-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e5575-139">conflictDeviceCount</span></span>|<span data-ttu-id="e5575-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e5575-140">Int32</span></span>|<span data-ttu-id="e5575-141">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e5575-141">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5575-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5575-142">Relationships</span></span>
<span data-ttu-id="e5575-143">なし</span><span class="sxs-lookup"><span data-stu-id="e5575-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e5575-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5575-144">JSON Representation</span></span>
<span data-ttu-id="e5575-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5575-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}-->
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








