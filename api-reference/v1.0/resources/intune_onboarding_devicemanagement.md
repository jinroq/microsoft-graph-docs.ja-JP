# <a name="devicemanagement-resource-type"></a><span data-ttu-id="8cc50-101">deviceManagement リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="8cc50-101">deviceManagement resource type</span></span>

> <span data-ttu-id="8cc50-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8cc50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cc50-103">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="8cc50-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="8cc50-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="8cc50-104">Methods</span></span>
|<span data-ttu-id="8cc50-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8cc50-105">Method</span></span>|<span data-ttu-id="8cc50-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8cc50-106">Return Type</span></span>|<span data-ttu-id="8cc50-107">説明</span><span class="sxs-lookup"><span data-stu-id="8cc50-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8cc50-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8cc50-108">Get deviceManagement</span></span>](../api/intune_onboarding_devicemanagement_get.md)|[<span data-ttu-id="8cc50-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8cc50-109">deviceManagement</span></span>](../resources/intune_onboarding_devicemanagement.md)|<span data-ttu-id="8cc50-110">[deviceManagement](../resources/intune_onboarding_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8cc50-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_onboarding_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="8cc50-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8cc50-111">Update deviceManagement</span></span>](../api/intune_onboarding_devicemanagement_update.md)|[<span data-ttu-id="8cc50-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8cc50-112">deviceManagement</span></span>](../resources/intune_onboarding_devicemanagement.md)|<span data-ttu-id="8cc50-113">[deviceManagement](../resources/intune_onboarding_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8cc50-113">Update the properties of a [calendar](../resources/intune_onboarding_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="8cc50-114">verifyWindowsEnrollmentAutoDiscovery function</span><span class="sxs-lookup"><span data-stu-id="8cc50-114">verifyWindowsEnrollmentAutoDiscovery function</span></span>](../api/intune_onboarding_devicemanagement_verifywindowsenrollmentautodiscovery.md)|<span data-ttu-id="8cc50-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc50-115">Boolean</span></span>|<span data-ttu-id="8cc50-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8cc50-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8cc50-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cc50-117">Properties</span></span>
|<span data-ttu-id="8cc50-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cc50-118">Property</span></span>|<span data-ttu-id="8cc50-119">型</span><span class="sxs-lookup"><span data-stu-id="8cc50-119">Type</span></span>|<span data-ttu-id="8cc50-120">説明</span><span class="sxs-lookup"><span data-stu-id="8cc50-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc50-121">id</span><span class="sxs-lookup"><span data-stu-id="8cc50-121">id</span></span>|<span data-ttu-id="8cc50-122">String</span><span class="sxs-lookup"><span data-stu-id="8cc50-122">String</span></span>|<span data-ttu-id="8cc50-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8cc50-123">Not yet documented</span></span>|
|<span data-ttu-id="8cc50-124">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="8cc50-124">intuneBrand</span></span>|[<span data-ttu-id="8cc50-125">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="8cc50-125">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="8cc50-126">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8cc50-126">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cc50-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cc50-127">Relationships</span></span>
|<span data-ttu-id="8cc50-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cc50-128">Relationship</span></span>|<span data-ttu-id="8cc50-129">型</span><span class="sxs-lookup"><span data-stu-id="8cc50-129">Type</span></span>|<span data-ttu-id="8cc50-130">説明</span><span class="sxs-lookup"><span data-stu-id="8cc50-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc50-131">deviceCategories</span><span class="sxs-lookup"><span data-stu-id="8cc50-131">deviceCategories</span></span>|<span data-ttu-id="8cc50-132">[deviceCategory](../resources/intune_onboarding_devicecategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8cc50-132">[deviceCategory](../resources/intune_onboarding_devicecategory.md) collection</span></span>|<span data-ttu-id="8cc50-133">テナントを含むデバイスのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="8cc50-133">The list of device categories with the tenant.</span></span>|
|<span data-ttu-id="8cc50-134">exchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="8cc50-134">exchangeConnectors</span></span>|<span data-ttu-id="8cc50-135">[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8cc50-135">[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) collection</span></span>|<span data-ttu-id="8cc50-136">テナントによって構成されている Exchange Connector のリスト。</span><span class="sxs-lookup"><span data-stu-id="8cc50-136">The list of Exchange Connectors configured by the tenant.</span></span>|
|<span data-ttu-id="8cc50-137">deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="8cc50-137">deviceEnrollmentConfigurations</span></span>|<span data-ttu-id="8cc50-138">[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8cc50-138">[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="8cc50-139">デバイス登録の構成のリスト</span><span class="sxs-lookup"><span data-stu-id="8cc50-139">The list of device enrollment configurations</span></span>|
|<span data-ttu-id="8cc50-140">conditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8cc50-140">conditionalAccessSettings</span></span>|[<span data-ttu-id="8cc50-141">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8cc50-141">onpremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="8cc50-142">Exchange のオンプレミスでの条件付きアクセス設定。</span><span class="sxs-lookup"><span data-stu-id="8cc50-142">The Exchange on premises conditional access settings.</span></span> <span data-ttu-id="8cc50-143">オンプレミスの条件付きアクセスでは、デバイスを登録し、メール アクセスに準拠させる必要があります</span><span class="sxs-lookup"><span data-stu-id="8cc50-143">On premises conditional access will require devices to be both enrolled and compliant for mail access</span></span>|
|<span data-ttu-id="8cc50-144">mobileThreatDefenseConnectors</span><span class="sxs-lookup"><span data-stu-id="8cc50-144">mobileThreatDefenseConnectors</span></span>|<span data-ttu-id="8cc50-145">[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8cc50-145">[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) collection</span></span>|<span data-ttu-id="8cc50-146">テナントによって構成されている、モバイルの脅威保護コネクタのリスト。</span><span class="sxs-lookup"><span data-stu-id="8cc50-146">The list of Mobile threat Defense connectors configured by the tenant.</span></span>|
|<span data-ttu-id="8cc50-147">deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="8cc50-147">deviceManagementPartners</span></span>|<span data-ttu-id="8cc50-148">[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8cc50-148">[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="8cc50-149">テナントによって構成されているデバイス管理パートナーのリスト。</span><span class="sxs-lookup"><span data-stu-id="8cc50-149">The list of Device Management Partners configured by the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cc50-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cc50-150">JSON Representation</span></span>
<span data-ttu-id="8cc50-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cc50-151">Here is a JSON representation of the resource.</span></span>
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
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "String",
    "contactITName": "String",
    "contactITPhoneNumber": "String",
    "contactITEmailAddress": "String",
    "contactITNotes": "String",
    "privacyUrl": "String",
    "onlineSupportSiteUrl": "String",
    "onlineSupportSiteName": "String",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1024,
      "g": 1024,
      "b": 1024
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true
  }
}
```



