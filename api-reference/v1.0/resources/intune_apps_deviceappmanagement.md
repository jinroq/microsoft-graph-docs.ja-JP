# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="7be67-101">deviceAppManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7be67-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="7be67-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7be67-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7be67-103">すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="7be67-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="7be67-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="7be67-104">Methods</span></span>
|<span data-ttu-id="7be67-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7be67-105">Method</span></span>|<span data-ttu-id="7be67-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7be67-106">Return Type</span></span>|<span data-ttu-id="7be67-107">説明</span><span class="sxs-lookup"><span data-stu-id="7be67-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7be67-108">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7be67-108">Get deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_get.md)|[<span data-ttu-id="7be67-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7be67-109">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="7be67-110">[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7be67-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="7be67-111">Update deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7be67-111">Update deviceAppManagement</span></span>](../api/intune_apps_deviceappmanagement_update.md)|[<span data-ttu-id="7be67-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7be67-112">deviceAppManagement</span></span>](../resources/intune_apps_deviceappmanagement.md)|<span data-ttu-id="7be67-113">[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7be67-113">Update the properties of a [calendar](../resources/intune_apps_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7be67-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7be67-114">Properties</span></span>
|<span data-ttu-id="7be67-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7be67-115">Property</span></span>|<span data-ttu-id="7be67-116">型</span><span class="sxs-lookup"><span data-stu-id="7be67-116">Type</span></span>|<span data-ttu-id="7be67-117">説明</span><span class="sxs-lookup"><span data-stu-id="7be67-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7be67-118">id</span><span class="sxs-lookup"><span data-stu-id="7be67-118">id</span></span>|<span data-ttu-id="7be67-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7be67-119">String</span></span>|<span data-ttu-id="7be67-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7be67-120">Name of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7be67-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7be67-121">Relationships</span></span>
|<span data-ttu-id="7be67-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7be67-122">Relationship</span></span>|<span data-ttu-id="7be67-123">型</span><span class="sxs-lookup"><span data-stu-id="7be67-123">Type</span></span>|<span data-ttu-id="7be67-124">説明</span><span class="sxs-lookup"><span data-stu-id="7be67-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7be67-125">mobileApps</span><span class="sxs-lookup"><span data-stu-id="7be67-125">mobileApps</span></span>|<span data-ttu-id="7be67-126">[mobileApp](../resources/intune_apps_mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7be67-126">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="7be67-127">モバイル アプリ。</span><span class="sxs-lookup"><span data-stu-id="7be67-127">The mobile apps.</span></span>|
|<span data-ttu-id="7be67-128">mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="7be67-128">mobileAppCategories</span></span>|<span data-ttu-id="7be67-129">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7be67-129">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="7be67-130">モバイル アプリ カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="7be67-130">The mobile app categories.</span></span>|
|<span data-ttu-id="7be67-131">mobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7be67-131">mobileAppConfigurations</span></span>|<span data-ttu-id="7be67-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7be67-132">[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="7be67-133">管理対象デバイスのモバイル アプリケーション構成。</span><span class="sxs-lookup"><span data-stu-id="7be67-133">The Managed Device Mobile Application Configurations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7be67-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7be67-134">JSON Representation</span></span>
<span data-ttu-id="7be67-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7be67-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



