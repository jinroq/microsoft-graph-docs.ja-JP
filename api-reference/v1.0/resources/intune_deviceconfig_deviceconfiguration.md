# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="ace24-101">deviceConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ace24-101">deviceConfiguration resource type</span></span>

> <span data-ttu-id="ace24-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ace24-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ace24-103">デバイス構成です。</span><span class="sxs-lookup"><span data-stu-id="ace24-103">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="ace24-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="ace24-104">Methods</span></span>
|<span data-ttu-id="ace24-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ace24-105">Method</span></span>|<span data-ttu-id="ace24-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ace24-106">Return Type</span></span>|<span data-ttu-id="ace24-107">説明</span><span class="sxs-lookup"><span data-stu-id="ace24-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ace24-108">deviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="ace24-108">List deviceConfigurations</span></span>](../api/intune_deviceconfig_deviceconfiguration_list.md)|<span data-ttu-id="ace24-109">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ace24-109">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) collection</span></span>|<span data-ttu-id="ace24-110">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ace24-110">List properties and relationships of the [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ace24-111">deviceConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="ace24-111">Get deviceConfiguration</span></span>](../api/intune_deviceconfig_deviceconfiguration_get.md)|[<span data-ttu-id="ace24-112">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ace24-112">deviceConfiguration</span></span>](../resources/intune_deviceconfig_deviceconfiguration.md)|<span data-ttu-id="ace24-113">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ace24-113">Read properties and relationships of the [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ace24-114">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="ace24-114">assign action</span></span>](../api/intune_deviceconfig_deviceconfiguration_assign.md)|<span data-ttu-id="ace24-115">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ace24-115">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ace24-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ace24-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ace24-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ace24-117">Properties</span></span>
|<span data-ttu-id="ace24-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ace24-118">Property</span></span>|<span data-ttu-id="ace24-119">タイプ</span><span class="sxs-lookup"><span data-stu-id="ace24-119">Type</span></span>|<span data-ttu-id="ace24-120">説明</span><span class="sxs-lookup"><span data-stu-id="ace24-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ace24-121">ID</span><span class="sxs-lookup"><span data-stu-id="ace24-121">id</span></span>|<span data-ttu-id="ace24-122">文字列</span><span class="sxs-lookup"><span data-stu-id="ace24-122">String</span></span>|<span data-ttu-id="ace24-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ace24-123">Key of the entity.</span></span>|
|<span data-ttu-id="ace24-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ace24-124">lastModifiedDateTime</span></span>|<span data-ttu-id="ace24-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ace24-125">DateTimeOffset</span></span>|<span data-ttu-id="ace24-126">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ace24-126">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ace24-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ace24-127">createdDateTime</span></span>|<span data-ttu-id="ace24-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ace24-128">DateTimeOffset</span></span>|<span data-ttu-id="ace24-129">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ace24-129">DateTime the object was created.</span></span>|
|<span data-ttu-id="ace24-130">説明</span><span class="sxs-lookup"><span data-stu-id="ace24-130">description</span></span>|<span data-ttu-id="ace24-131">文字列</span><span class="sxs-lookup"><span data-stu-id="ace24-131">String</span></span>|<span data-ttu-id="ace24-132">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="ace24-132">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="ace24-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ace24-133">displayName</span></span>|<span data-ttu-id="ace24-134">文字列</span><span class="sxs-lookup"><span data-stu-id="ace24-134">String</span></span>|<span data-ttu-id="ace24-135">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="ace24-135">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ace24-136">バージョン</span><span class="sxs-lookup"><span data-stu-id="ace24-136">version</span></span>|<span data-ttu-id="ace24-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ace24-137">Int32</span></span>|<span data-ttu-id="ace24-138">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ace24-138">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ace24-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ace24-139">Relationships</span></span>
|<span data-ttu-id="ace24-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ace24-140">Relationship</span></span>|<span data-ttu-id="ace24-141">型</span><span class="sxs-lookup"><span data-stu-id="ace24-141">Type</span></span>|<span data-ttu-id="ace24-142">説明</span><span class="sxs-lookup"><span data-stu-id="ace24-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ace24-143">割り当て</span><span class="sxs-lookup"><span data-stu-id="ace24-143">assignments</span></span>|<span data-ttu-id="ace24-144">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ace24-144">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ace24-145">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="ace24-145">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="ace24-146">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ace24-146">deviceStatuses</span></span>|<span data-ttu-id="ace24-147">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ace24-147">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="ace24-148">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="ace24-148">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="ace24-149">userStatuses</span><span class="sxs-lookup"><span data-stu-id="ace24-149">userStatuses</span></span>|<span data-ttu-id="ace24-150">[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ace24-150">[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="ace24-151">ユーザーごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="ace24-151">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="ace24-152">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ace24-152">deviceStatusOverview</span></span>|[<span data-ttu-id="ace24-153">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ace24-153">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="ace24-154">デバイス構成のデバイス状態の概要</span><span class="sxs-lookup"><span data-stu-id="ace24-154">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="ace24-155">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ace24-155">userStatusOverview</span></span>|[<span data-ttu-id="ace24-156">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="ace24-156">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="ace24-157">デバイス構成のユーザー状態の概要</span><span class="sxs-lookup"><span data-stu-id="ace24-157">Device Configuration users status overview</span></span>|
|<span data-ttu-id="ace24-158">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="ace24-158">deviceSettingStateSummaries</span></span>|<span data-ttu-id="ace24-159">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ace24-159">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="ace24-160">デバイス構成設定状態のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="ace24-160">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ace24-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ace24-161">JSON Representation</span></span>
<span data-ttu-id="ace24-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ace24-162">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```








