# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="0f6ce-101">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f6ce-101">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="0f6ce-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f6ce-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f6ce-103">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="0f6ce-103">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="0f6ce-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f6ce-104">Properties</span></span>
|<span data-ttu-id="0f6ce-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f6ce-105">Property</span></span>|<span data-ttu-id="0f6ce-106">型</span><span class="sxs-lookup"><span data-stu-id="0f6ce-106">Type</span></span>|<span data-ttu-id="0f6ce-107">説明</span><span class="sxs-lookup"><span data-stu-id="0f6ce-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f6ce-108">inventory</span><span class="sxs-lookup"><span data-stu-id="0f6ce-108">inventory</span></span>|<span data-ttu-id="0f6ce-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6ce-109">Boolean</span></span>|<span data-ttu-id="0f6ce-110">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0f6ce-110">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="0f6ce-111">modernApps</span><span class="sxs-lookup"><span data-stu-id="0f6ce-111">modernApps</span></span>|<span data-ttu-id="0f6ce-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6ce-112">Boolean</span></span>|<span data-ttu-id="0f6ce-113">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0f6ce-113">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="0f6ce-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="0f6ce-114">resourceAccess</span></span>|<span data-ttu-id="0f6ce-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6ce-115">Boolean</span></span>|<span data-ttu-id="0f6ce-116">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0f6ce-116">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="0f6ce-117">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f6ce-117">deviceConfiguration</span></span>|<span data-ttu-id="0f6ce-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6ce-118">Boolean</span></span>|<span data-ttu-id="0f6ce-119">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0f6ce-119">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="0f6ce-120">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0f6ce-120">compliancePolicy</span></span>|<span data-ttu-id="0f6ce-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6ce-121">Boolean</span></span>|<span data-ttu-id="0f6ce-122">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0f6ce-122">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="0f6ce-123">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="0f6ce-123">windowsUpdateForBusiness</span></span>|<span data-ttu-id="0f6ce-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6ce-124">Boolean</span></span>|<span data-ttu-id="0f6ce-125">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0f6ce-125">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f6ce-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f6ce-126">Relationships</span></span>
<span data-ttu-id="0f6ce-127">なし</span><span class="sxs-lookup"><span data-stu-id="0f6ce-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f6ce-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f6ce-128">JSON Representation</span></span>
<span data-ttu-id="0f6ce-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f6ce-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
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



