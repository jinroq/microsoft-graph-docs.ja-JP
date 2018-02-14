# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="e6453-101">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6453-101">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="e6453-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6453-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6453-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e6453-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="e6453-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6453-104">Methods</span></span>
|<span data-ttu-id="e6453-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6453-105">Method</span></span>|<span data-ttu-id="e6453-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e6453-106">Return Type</span></span>|<span data-ttu-id="e6453-107">説明</span><span class="sxs-lookup"><span data-stu-id="e6453-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6453-108">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e6453-108">Get deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[<span data-ttu-id="e6453-109">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e6453-109">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="e6453-110">[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e6453-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="e6453-111">Update deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e6453-111">Update deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_update.md)|[<span data-ttu-id="e6453-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e6453-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="e6453-113">[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e6453-113">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6453-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6453-114">Properties</span></span>
|<span data-ttu-id="e6453-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6453-115">Property</span></span>|<span data-ttu-id="e6453-116">型</span><span class="sxs-lookup"><span data-stu-id="e6453-116">Type</span></span>|<span data-ttu-id="e6453-117">説明</span><span class="sxs-lookup"><span data-stu-id="e6453-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6453-118">id</span><span class="sxs-lookup"><span data-stu-id="e6453-118">id</span></span>|<span data-ttu-id="e6453-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e6453-119">String</span></span>|<span data-ttu-id="e6453-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e6453-120">Name of the entity.</span></span>|
|<span data-ttu-id="e6453-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e6453-121">pendingCount</span></span>|<span data-ttu-id="e6453-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e6453-122">Int32</span></span>|<span data-ttu-id="e6453-123">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e6453-123">Number of pending devices</span></span>|
|<span data-ttu-id="e6453-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e6453-124">notApplicableCount</span></span>|<span data-ttu-id="e6453-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e6453-125">Int32</span></span>|<span data-ttu-id="e6453-126">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e6453-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="e6453-127">successCount</span><span class="sxs-lookup"><span data-stu-id="e6453-127">successCount</span></span>|<span data-ttu-id="e6453-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e6453-128">Int32</span></span>|<span data-ttu-id="e6453-129">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e6453-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="e6453-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="e6453-130">errorCount</span></span>|<span data-ttu-id="e6453-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e6453-131">Int32</span></span>|<span data-ttu-id="e6453-132">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e6453-132">Number of error devices</span></span>|
|<span data-ttu-id="e6453-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="e6453-133">failedCount</span></span>|<span data-ttu-id="e6453-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e6453-134">Int32</span></span>|<span data-ttu-id="e6453-135">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e6453-135">Number of failed devices</span></span>|
|<span data-ttu-id="e6453-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e6453-136">lastUpdateDateTime</span></span>|<span data-ttu-id="e6453-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6453-137">DateTimeOffset</span></span>|<span data-ttu-id="e6453-138">最終更新日時</span><span class="sxs-lookup"><span data-stu-id="e6453-138">Last update time</span></span>|
|<span data-ttu-id="e6453-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e6453-139">configurationVersion</span></span>|<span data-ttu-id="e6453-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e6453-140">Int32</span></span>|<span data-ttu-id="e6453-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="e6453-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6453-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6453-142">Relationships</span></span>
<span data-ttu-id="e6453-143">なし</span><span class="sxs-lookup"><span data-stu-id="e6453-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6453-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6453-144">JSON Representation</span></span>
<span data-ttu-id="e6453-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6453-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



