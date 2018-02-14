# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="57c25-101">managedDeviceMobileAppConfigurationDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57c25-101">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="57c25-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="57c25-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57c25-103">MDM モバイル アプリ構成のデバイス状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57c25-103">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="57c25-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="57c25-104">Methods</span></span>
|<span data-ttu-id="57c25-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="57c25-105">Method</span></span>|<span data-ttu-id="57c25-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="57c25-106">Return Type</span></span>|<span data-ttu-id="57c25-107">説明</span><span class="sxs-lookup"><span data-stu-id="57c25-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57c25-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="57c25-108">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_get.md)|[<span data-ttu-id="57c25-109">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="57c25-109">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="57c25-110"> [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="57c25-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="57c25-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="57c25-111">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationdevicesummary_update.md)|[<span data-ttu-id="57c25-112">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="57c25-112">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="57c25-113">[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="57c25-113">Update the properties of a [calendar](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="57c25-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57c25-114">Properties</span></span>
|<span data-ttu-id="57c25-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57c25-115">Property</span></span>|<span data-ttu-id="57c25-116">型</span><span class="sxs-lookup"><span data-stu-id="57c25-116">Type</span></span>|<span data-ttu-id="57c25-117">説明</span><span class="sxs-lookup"><span data-stu-id="57c25-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57c25-118">id</span><span class="sxs-lookup"><span data-stu-id="57c25-118">id</span></span>|<span data-ttu-id="57c25-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="57c25-119">String</span></span>|<span data-ttu-id="57c25-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="57c25-120">Name of the entity.</span></span>|
|<span data-ttu-id="57c25-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="57c25-121">pendingCount</span></span>|<span data-ttu-id="57c25-122">Int32</span><span class="sxs-lookup"><span data-stu-id="57c25-122">Int32</span></span>|<span data-ttu-id="57c25-123">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="57c25-123">Number of pending devices</span></span>|
|<span data-ttu-id="57c25-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="57c25-124">notApplicableCount</span></span>|<span data-ttu-id="57c25-125">Int32</span><span class="sxs-lookup"><span data-stu-id="57c25-125">Int32</span></span>|<span data-ttu-id="57c25-126">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="57c25-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="57c25-127">successCount</span><span class="sxs-lookup"><span data-stu-id="57c25-127">successCount</span></span>|<span data-ttu-id="57c25-128">Int32</span><span class="sxs-lookup"><span data-stu-id="57c25-128">Int32</span></span>|<span data-ttu-id="57c25-129">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="57c25-129">Number of succeeded devices</span></span>|
|<span data-ttu-id="57c25-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="57c25-130">errorCount</span></span>|<span data-ttu-id="57c25-131">Int32</span><span class="sxs-lookup"><span data-stu-id="57c25-131">Int32</span></span>|<span data-ttu-id="57c25-132">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="57c25-132">Number of error devices</span></span>|
|<span data-ttu-id="57c25-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="57c25-133">failedCount</span></span>|<span data-ttu-id="57c25-134">Int32</span><span class="sxs-lookup"><span data-stu-id="57c25-134">Int32</span></span>|<span data-ttu-id="57c25-135">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="57c25-135">Number of failed devices</span></span>|
|<span data-ttu-id="57c25-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="57c25-136">lastUpdateDateTime</span></span>|<span data-ttu-id="57c25-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57c25-137">DateTimeOffset</span></span>|<span data-ttu-id="57c25-138">最終更新日時</span><span class="sxs-lookup"><span data-stu-id="57c25-138">Last update time</span></span>|
|<span data-ttu-id="57c25-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="57c25-139">configurationVersion</span></span>|<span data-ttu-id="57c25-140">Int32</span><span class="sxs-lookup"><span data-stu-id="57c25-140">Int32</span></span>|<span data-ttu-id="57c25-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="57c25-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="57c25-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="57c25-142">Relationships</span></span>
<span data-ttu-id="57c25-143">なし</span><span class="sxs-lookup"><span data-stu-id="57c25-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="57c25-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57c25-144">JSON Representation</span></span>
<span data-ttu-id="57c25-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="57c25-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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



