# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="a452c-101">managedDeviceMobileAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a452c-101">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="a452c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a452c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a452c-103">登録済みデバイスのモバイル アプリ構成用の抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="a452c-103">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="a452c-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="a452c-104">Methods</span></span>
|<span data-ttu-id="a452c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a452c-105">Method</span></span>|<span data-ttu-id="a452c-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a452c-106">Return Type</span></span>|<span data-ttu-id="a452c-107">説明</span><span class="sxs-lookup"><span data-stu-id="a452c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a452c-108">managedDeviceMobileAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="a452c-108">List managedDeviceMobileAppConfigurations</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|<span data-ttu-id="a452c-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a452c-109">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="a452c-110">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a452c-110">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a452c-111">managedDeviceMobileAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="a452c-111">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[<span data-ttu-id="a452c-112">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a452c-112">managedDeviceMobileAppConfiguration</span></span>](../resources/intune_apps_manageddevicemobileappconfiguration.md)|<span data-ttu-id="a452c-113">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a452c-113">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a452c-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a452c-114">Properties</span></span>
|<span data-ttu-id="a452c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a452c-115">Property</span></span>|<span data-ttu-id="a452c-116">型</span><span class="sxs-lookup"><span data-stu-id="a452c-116">Type</span></span>|<span data-ttu-id="a452c-117">説明</span><span class="sxs-lookup"><span data-stu-id="a452c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a452c-118">ID</span><span class="sxs-lookup"><span data-stu-id="a452c-118">id</span></span>|<span data-ttu-id="a452c-119">文字列</span><span class="sxs-lookup"><span data-stu-id="a452c-119">String</span></span>|<span data-ttu-id="a452c-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a452c-120">Key of the entity.</span></span>|
|<span data-ttu-id="a452c-121">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="a452c-121">targetedMobileApps</span></span>|<span data-ttu-id="a452c-122">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a452c-122">String collection</span></span>|<span data-ttu-id="a452c-123">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="a452c-123">the associated app.</span></span>|
|<span data-ttu-id="a452c-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a452c-124">createdDateTime</span></span>|<span data-ttu-id="a452c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a452c-125">DateTimeOffset</span></span>|<span data-ttu-id="a452c-126">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a452c-126">DateTime the object was created.</span></span>|
|<span data-ttu-id="a452c-127">説明</span><span class="sxs-lookup"><span data-stu-id="a452c-127">description</span></span>|<span data-ttu-id="a452c-128">文字列</span><span class="sxs-lookup"><span data-stu-id="a452c-128">String</span></span>|<span data-ttu-id="a452c-129">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="a452c-129">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="a452c-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a452c-130">lastModifiedDateTime</span></span>|<span data-ttu-id="a452c-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a452c-131">DateTimeOffset</span></span>|<span data-ttu-id="a452c-132">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a452c-132">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a452c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a452c-133">displayName</span></span>|<span data-ttu-id="a452c-134">文字列</span><span class="sxs-lookup"><span data-stu-id="a452c-134">String</span></span>|<span data-ttu-id="a452c-135">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="a452c-135">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="a452c-136">バージョン</span><span class="sxs-lookup"><span data-stu-id="a452c-136">version</span></span>|<span data-ttu-id="a452c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a452c-137">Int32</span></span>|<span data-ttu-id="a452c-138">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a452c-138">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a452c-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a452c-139">Relationships</span></span>
|<span data-ttu-id="a452c-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a452c-140">Relationship</span></span>|<span data-ttu-id="a452c-141">型</span><span class="sxs-lookup"><span data-stu-id="a452c-141">Type</span></span>|<span data-ttu-id="a452c-142">説明</span><span class="sxs-lookup"><span data-stu-id="a452c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a452c-143">割り当て</span><span class="sxs-lookup"><span data-stu-id="a452c-143">assignments</span></span>|<span data-ttu-id="a452c-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a452c-144">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a452c-145">アプリ構成のグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="a452c-145">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="a452c-146">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a452c-146">deviceStatuses</span></span>|<span data-ttu-id="a452c-147">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a452c-147">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a452c-148">ManagedDeviceMobileAppConfigurationDeviceStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="a452c-148">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="a452c-149">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a452c-149">userStatuses</span></span>|<span data-ttu-id="a452c-150">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a452c-150">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a452c-151">ManagedDeviceMobileAppConfigurationUserStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="a452c-151">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="a452c-152">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a452c-152">deviceStatusSummary</span></span>|[<span data-ttu-id="a452c-153">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a452c-153">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="a452c-154">アプリ構成のデバイス状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="a452c-154">App configuration device status summary.</span></span>|
|<span data-ttu-id="a452c-155">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a452c-155">userStatusSummary</span></span>|[<span data-ttu-id="a452c-156">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="a452c-156">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="a452c-157">アプリ構成のユーザー状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="a452c-157">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a452c-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a452c-158">JSON Representation</span></span>
<span data-ttu-id="a452c-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a452c-159">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```








