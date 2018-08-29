# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="5c5de-101">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c5de-101">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="5c5de-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c5de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c5de-103">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="5c5de-103">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="5c5de-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c5de-104">Properties</span></span>
|<span data-ttu-id="5c5de-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c5de-105">Property</span></span>|<span data-ttu-id="5c5de-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="5c5de-106">Type</span></span>|<span data-ttu-id="5c5de-107">説明</span><span class="sxs-lookup"><span data-stu-id="5c5de-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c5de-108">inventory</span><span class="sxs-lookup"><span data-stu-id="5c5de-108">inventory</span></span>|<span data-ttu-id="5c5de-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c5de-109">Boolean</span></span>|<span data-ttu-id="5c5de-110">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="5c5de-110">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="5c5de-111">modernApps</span><span class="sxs-lookup"><span data-stu-id="5c5de-111">modernApps</span></span>|<span data-ttu-id="5c5de-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c5de-112">Boolean</span></span>|<span data-ttu-id="5c5de-113">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="5c5de-113">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="5c5de-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="5c5de-114">resourceAccess</span></span>|<span data-ttu-id="5c5de-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c5de-115">Boolean</span></span>|<span data-ttu-id="5c5de-116">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="5c5de-116">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="5c5de-117">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c5de-117">deviceConfiguration</span></span>|<span data-ttu-id="5c5de-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c5de-118">Boolean</span></span>|<span data-ttu-id="5c5de-119">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="5c5de-119">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="5c5de-120">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5c5de-120">compliancePolicy</span></span>|<span data-ttu-id="5c5de-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c5de-121">Boolean</span></span>|<span data-ttu-id="5c5de-122">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="5c5de-122">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="5c5de-123">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="5c5de-123">windowsUpdateForBusiness</span></span>|<span data-ttu-id="5c5de-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c5de-124">Boolean</span></span>|<span data-ttu-id="5c5de-125">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="5c5de-125">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c5de-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5c5de-126">Relationships</span></span>
<span data-ttu-id="5c5de-127">なし</span><span class="sxs-lookup"><span data-stu-id="5c5de-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5c5de-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c5de-128">JSON Representation</span></span>
<span data-ttu-id="5c5de-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c5de-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



