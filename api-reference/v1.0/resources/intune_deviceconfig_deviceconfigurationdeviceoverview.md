# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="be599-101">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be599-101">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="be599-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="be599-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be599-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="be599-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="be599-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="be599-104">Methods</span></span>
|<span data-ttu-id="be599-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="be599-105">Method</span></span>|<span data-ttu-id="be599-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be599-106">Return Type</span></span>|<span data-ttu-id="be599-107">説明</span><span class="sxs-lookup"><span data-stu-id="be599-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be599-108">deviceConfigurationDeviceOverview の取得</span><span class="sxs-lookup"><span data-stu-id="be599-108">Get deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[<span data-ttu-id="be599-109">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="be599-109">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="be599-110">[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="be599-110">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="be599-111">deviceConfigurationDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="be599-111">Update deviceConfigurationDeviceOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_update.md)|[<span data-ttu-id="be599-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="be599-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="be599-113">[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="be599-113">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="be599-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be599-114">Properties</span></span>
|<span data-ttu-id="be599-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be599-115">Property</span></span>|<span data-ttu-id="be599-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="be599-116">Type</span></span>|<span data-ttu-id="be599-117">説明</span><span class="sxs-lookup"><span data-stu-id="be599-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be599-118">ID</span><span class="sxs-lookup"><span data-stu-id="be599-118">id</span></span>|<span data-ttu-id="be599-119">文字列</span><span class="sxs-lookup"><span data-stu-id="be599-119">String</span></span>|<span data-ttu-id="be599-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="be599-120">Key of the entity.</span></span>|
|<span data-ttu-id="be599-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="be599-121">pendingCount</span></span>|<span data-ttu-id="be599-122">Int32</span><span class="sxs-lookup"><span data-stu-id="be599-122">Int32</span></span>|<span data-ttu-id="be599-123">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="be599-123">Number of pending devices</span></span>|
|<span data-ttu-id="be599-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="be599-124">notApplicableCount</span></span>|<span data-ttu-id="be599-125">Int32</span><span class="sxs-lookup"><span data-stu-id="be599-125">Int32</span></span>|<span data-ttu-id="be599-126">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="be599-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="be599-127">successCount</span><span class="sxs-lookup"><span data-stu-id="be599-127">successCount</span></span>|<span data-ttu-id="be599-128">Int32</span><span class="sxs-lookup"><span data-stu-id="be599-128">Int32</span></span>|<span data-ttu-id="be599-129">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="be599-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="be599-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="be599-130">errorCount</span></span>|<span data-ttu-id="be599-131">Int32</span><span class="sxs-lookup"><span data-stu-id="be599-131">Int32</span></span>|<span data-ttu-id="be599-132">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="be599-132">Number of error devices</span></span>|
|<span data-ttu-id="be599-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="be599-133">failedCount</span></span>|<span data-ttu-id="be599-134">Int32</span><span class="sxs-lookup"><span data-stu-id="be599-134">Int32</span></span>|<span data-ttu-id="be599-135">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="be599-135">Number of failed devices</span></span>|
|<span data-ttu-id="be599-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="be599-136">lastUpdateDateTime</span></span>|<span data-ttu-id="be599-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be599-137">DateTimeOffset</span></span>|<span data-ttu-id="be599-138">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="be599-138">Last update time</span></span>|
|<span data-ttu-id="be599-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="be599-139">configurationVersion</span></span>|<span data-ttu-id="be599-140">Int32</span><span class="sxs-lookup"><span data-stu-id="be599-140">Int32</span></span>|<span data-ttu-id="be599-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="be599-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="be599-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be599-142">Relationships</span></span>
<span data-ttu-id="be599-143">なし</span><span class="sxs-lookup"><span data-stu-id="be599-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be599-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be599-144">JSON Representation</span></span>
<span data-ttu-id="be599-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be599-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}-->
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








