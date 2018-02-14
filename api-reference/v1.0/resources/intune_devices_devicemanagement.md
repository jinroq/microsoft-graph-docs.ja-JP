# <a name="devicemanagement-resource-type"></a><span data-ttu-id="f2c74-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2c74-101">deviceManagement resource type</span></span>

> <span data-ttu-id="f2c74-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2c74-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2c74-103">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="f2c74-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="f2c74-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2c74-104">Methods</span></span>
|<span data-ttu-id="f2c74-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2c74-105">Method</span></span>|<span data-ttu-id="f2c74-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f2c74-106">Return Type</span></span>|<span data-ttu-id="f2c74-107">説明</span><span class="sxs-lookup"><span data-stu-id="f2c74-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2c74-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f2c74-108">Get deviceManagement</span></span>](../api/intune_devices_devicemanagement_get.md)|[<span data-ttu-id="f2c74-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f2c74-109">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="f2c74-110">[deviceManagement](../resources/intune_devices_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f2c74-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="f2c74-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f2c74-111">Update deviceManagement</span></span>](../api/intune_devices_devicemanagement_update.md)|[<span data-ttu-id="f2c74-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f2c74-112">deviceManagement</span></span>](../resources/intune_devices_devicemanagement.md)|<span data-ttu-id="f2c74-113">[deviceManagement](../resources/intune_devices_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f2c74-113">Update the properties of a [calendar](../resources/intune_devices_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2c74-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2c74-114">Properties</span></span>
|<span data-ttu-id="f2c74-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2c74-115">Property</span></span>|<span data-ttu-id="f2c74-116">型</span><span class="sxs-lookup"><span data-stu-id="f2c74-116">Type</span></span>|<span data-ttu-id="f2c74-117">説明</span><span class="sxs-lookup"><span data-stu-id="f2c74-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2c74-118">id</span><span class="sxs-lookup"><span data-stu-id="f2c74-118">id</span></span>|<span data-ttu-id="f2c74-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f2c74-119">String</span></span>|<span data-ttu-id="f2c74-120">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="f2c74-120">Unique Identifier for the device</span></span>|
|<span data-ttu-id="f2c74-121">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="f2c74-121">subscriptionState</span></span>|<span data-ttu-id="f2c74-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f2c74-122">String</span></span>|<span data-ttu-id="f2c74-123">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="f2c74-123">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="f2c74-124">可能な値: `pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="f2c74-124">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2c74-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2c74-125">Relationships</span></span>
|<span data-ttu-id="f2c74-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2c74-126">Relationship</span></span>|<span data-ttu-id="f2c74-127">型</span><span class="sxs-lookup"><span data-stu-id="f2c74-127">Type</span></span>|<span data-ttu-id="f2c74-128">説明</span><span class="sxs-lookup"><span data-stu-id="f2c74-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2c74-129">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f2c74-129">applePushNotificationCertificate</span></span>|[<span data-ttu-id="f2c74-130">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f2c74-130">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="f2c74-131">Apple プッシュ通知証明書。</span><span class="sxs-lookup"><span data-stu-id="f2c74-131">Apple push notification certificate.</span></span>|
|<span data-ttu-id="f2c74-132">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f2c74-132">managedDeviceOverview</span></span>|[<span data-ttu-id="f2c74-133">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f2c74-133">managedDeviceOverview</span></span>](../resources/intune_devices_manageddeviceoverview.md)|<span data-ttu-id="f2c74-134">デバイスの概要</span><span class="sxs-lookup"><span data-stu-id="f2c74-134">Device overview</span></span>|
|<span data-ttu-id="f2c74-135">detectedApps</span><span class="sxs-lookup"><span data-stu-id="f2c74-135">detectedApps</span></span>|<span data-ttu-id="f2c74-136">[detectedApp](../resources/intune_devices_detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f2c74-136">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="f2c74-137">デバイスに関連付けられている、検出されたアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="f2c74-137">The list of detected apps associated with a device.</span></span>|
|<span data-ttu-id="f2c74-138">managedDevices</span><span class="sxs-lookup"><span data-stu-id="f2c74-138">managedDevices</span></span>|<span data-ttu-id="f2c74-139">[managedDevice](../resources/intune_devices_manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f2c74-139">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="f2c74-140">管理対象デバイスの一覧。</span><span class="sxs-lookup"><span data-stu-id="f2c74-140">The list of managed devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2c74-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2c74-141">JSON Representation</span></span>
<span data-ttu-id="f2c74-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2c74-142">Here is a JSON representation of the resource.</span></span>
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
  "subscriptionState": "String"
}
```



