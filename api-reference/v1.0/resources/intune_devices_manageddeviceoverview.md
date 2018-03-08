# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="537c8-101">managedDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="537c8-101">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="537c8-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="537c8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="537c8-103">管理対象デバイスの概要データ</span><span class="sxs-lookup"><span data-stu-id="537c8-103">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="537c8-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="537c8-104">Methods</span></span>
|<span data-ttu-id="537c8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="537c8-105">Method</span></span>|<span data-ttu-id="537c8-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="537c8-106">Return Type</span></span>|<span data-ttu-id="537c8-107">説明</span><span class="sxs-lookup"><span data-stu-id="537c8-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="537c8-108">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="537c8-108">Get managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_get.md)|[<span data-ttu-id="537c8-109">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="537c8-109">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="537c8-110">[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="537c8-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="537c8-111">Update managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="537c8-111">Update managedDeviceOverview</span></span>](../api/intune_devices_manageddeviceoverview_update.md)|[<span data-ttu-id="537c8-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="537c8-112">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="537c8-113">[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="537c8-113">Update the properties of a [calendar](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="537c8-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="537c8-114">Properties</span></span>
|<span data-ttu-id="537c8-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="537c8-115">Property</span></span>|<span data-ttu-id="537c8-116">型</span><span class="sxs-lookup"><span data-stu-id="537c8-116">Type</span></span>|<span data-ttu-id="537c8-117">説明</span><span class="sxs-lookup"><span data-stu-id="537c8-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="537c8-118">id</span><span class="sxs-lookup"><span data-stu-id="537c8-118">id</span></span>|<span data-ttu-id="537c8-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="537c8-119">String</span></span>|<span data-ttu-id="537c8-120">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="537c8-120">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="537c8-121">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="537c8-121">enrolledDeviceCount</span></span>|<span data-ttu-id="537c8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="537c8-122">Int32</span></span>|<span data-ttu-id="537c8-123">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="537c8-123">Total enrolled device count.</span></span> <span data-ttu-id="537c8-124">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="537c8-124">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="537c8-125">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="537c8-125">mdmEnrolledCount</span></span>|<span data-ttu-id="537c8-126">Int32</span><span class="sxs-lookup"><span data-stu-id="537c8-126">Int32</span></span>|<span data-ttu-id="537c8-127">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="537c8-127">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="537c8-128">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="537c8-128">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="537c8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="537c8-129">Int32</span></span>|<span data-ttu-id="537c8-130">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="537c8-130">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="537c8-131">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="537c8-131">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="537c8-132">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="537c8-132">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="537c8-133">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="537c8-133">Device operating system summary.</span></span>|
|<span data-ttu-id="537c8-134">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="537c8-134">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="537c8-135">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="537c8-135">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="537c8-136">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="537c8-136">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="537c8-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="537c8-137">Relationships</span></span>
<span data-ttu-id="537c8-138">なし</span><span class="sxs-lookup"><span data-stu-id="537c8-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="537c8-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="537c8-139">JSON Representation</span></span>
<span data-ttu-id="537c8-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="537c8-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```


