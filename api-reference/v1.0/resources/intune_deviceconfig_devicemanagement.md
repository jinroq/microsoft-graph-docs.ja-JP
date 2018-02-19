# <a name="devicemanagement-resource-type"></a><span data-ttu-id="b861e-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b861e-101">deviceManagement resource type</span></span>

> <span data-ttu-id="b861e-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b861e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b861e-103">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="b861e-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="b861e-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="b861e-104">Methods</span></span>
|<span data-ttu-id="b861e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b861e-105">Method</span></span>|<span data-ttu-id="b861e-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b861e-106">Return Type</span></span>|<span data-ttu-id="b861e-107">説明</span><span class="sxs-lookup"><span data-stu-id="b861e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b861e-108">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="b861e-108">Get deviceManagement</span></span>](../api/intune_deviceconfig_devicemanagement_get.md)|[<span data-ttu-id="b861e-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="b861e-109">deviceManagement</span></span>](../resources/intune_deviceconfig_devicemanagement.md)|<span data-ttu-id="b861e-110">[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b861e-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="b861e-111">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="b861e-111">Update deviceManagement</span></span>](../api/intune_deviceconfig_devicemanagement_update.md)|[<span data-ttu-id="b861e-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="b861e-112">deviceManagement</span></span>](../resources/intune_deviceconfig_devicemanagement.md)|<span data-ttu-id="b861e-113">[deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b861e-113">Update the properties of a [calendar](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b861e-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b861e-114">Properties</span></span>
|<span data-ttu-id="b861e-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b861e-115">Property</span></span>|<span data-ttu-id="b861e-116">型</span><span class="sxs-lookup"><span data-stu-id="b861e-116">Type</span></span>|<span data-ttu-id="b861e-117">説明</span><span class="sxs-lookup"><span data-stu-id="b861e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b861e-118">id</span><span class="sxs-lookup"><span data-stu-id="b861e-118">id</span></span>|<span data-ttu-id="b861e-119">String</span><span class="sxs-lookup"><span data-stu-id="b861e-119">String</span></span>|<span data-ttu-id="b861e-120">一意識別子</span><span class="sxs-lookup"><span data-stu-id="b861e-120">Unique Identifier</span></span>|
|<span data-ttu-id="b861e-121">settings</span><span class="sxs-lookup"><span data-stu-id="b861e-121">settings</span></span>|[<span data-ttu-id="b861e-122">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="b861e-122">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="b861e-123">アカウント レベルの設定です。</span><span class="sxs-lookup"><span data-stu-id="b861e-123">Account level settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b861e-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b861e-124">Relationships</span></span>
|<span data-ttu-id="b861e-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b861e-125">Relationship</span></span>|<span data-ttu-id="b861e-126">型</span><span class="sxs-lookup"><span data-stu-id="b861e-126">Type</span></span>|<span data-ttu-id="b861e-127">説明</span><span class="sxs-lookup"><span data-stu-id="b861e-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b861e-128">deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="b861e-128">deviceConfigurations</span></span>|<span data-ttu-id="b861e-129">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b861e-129">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) collection</span></span>|<span data-ttu-id="b861e-130">デバイス構成です。</span><span class="sxs-lookup"><span data-stu-id="b861e-130">The device configurations.</span></span>|
|<span data-ttu-id="b861e-131">deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="b861e-131">deviceCompliancePolicies</span></span>|<span data-ttu-id="b861e-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b861e-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="b861e-133">デバイス コンプライアンス ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="b861e-133">The device compliance policies.</span></span>|
|<span data-ttu-id="b861e-134">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b861e-134">softwareUpdateStatusSummary</span></span>|[<span data-ttu-id="b861e-135">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b861e-135">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="b861e-136">ソフトウェア更新状態の概要です。</span><span class="sxs-lookup"><span data-stu-id="b861e-136">The software update status summary.</span></span>|
|<span data-ttu-id="b861e-137">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b861e-137">deviceCompliancePolicyDeviceStateSummary</span></span>|[<span data-ttu-id="b861e-138">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b861e-138">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="b861e-139">このアカウントのデバイス コンプライアンスの状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="b861e-139">The device compliance state summary for this account.</span></span>|
|<span data-ttu-id="b861e-140">deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="b861e-140">deviceCompliancePolicySettingStateSummaries</span></span>|<span data-ttu-id="b861e-141">[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b861e-141">[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="b861e-142">このアカウントにおける、コンプライアンス ポリシーの設定の状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="b861e-142">The summary states of compliance policy settings for this account.</span></span>|
|<span data-ttu-id="b861e-143">deviceConfigurationDeviceStateSummaries</span><span class="sxs-lookup"><span data-stu-id="b861e-143">deviceConfigurationDeviceStateSummaries</span></span>|[<span data-ttu-id="b861e-144">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b861e-144">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="b861e-145">このアカウントにおける、デバイス構成のデバイス状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="b861e-145">The device configuration device state summary for this account.</span></span>|
|<span data-ttu-id="b861e-146">iosUpdateStatuses</span><span class="sxs-lookup"><span data-stu-id="b861e-146">iosUpdateStatuses</span></span>|<span data-ttu-id="b861e-147">[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b861e-147">[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) collection</span></span>|<span data-ttu-id="b861e-148">このアカウントにおける、iOS ソフトウェアの更新のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="b861e-148">The IOS software update installation statuses for this account.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b861e-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b861e-149">JSON Representation</span></span>
<span data-ttu-id="b861e-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b861e-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```



