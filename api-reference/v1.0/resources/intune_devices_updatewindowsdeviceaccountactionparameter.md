# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="70236-101">updateWindowsDeviceAccountActionParameter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70236-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="70236-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="70236-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70236-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="70236-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="70236-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70236-104">Properties</span></span>
|<span data-ttu-id="70236-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70236-105">Property</span></span>|<span data-ttu-id="70236-106">型</span><span class="sxs-lookup"><span data-stu-id="70236-106">Type</span></span>|<span data-ttu-id="70236-107">説明</span><span class="sxs-lookup"><span data-stu-id="70236-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70236-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="70236-108">deviceAccount</span></span>|[<span data-ttu-id="70236-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="70236-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="70236-110">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="70236-110">Not yet documented</span></span>|
|<span data-ttu-id="70236-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="70236-111">passwordRotationEnabled</span></span>|<span data-ttu-id="70236-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="70236-112">Boolean</span></span>|<span data-ttu-id="70236-113">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="70236-113">Not yet documented</span></span>|
|<span data-ttu-id="70236-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="70236-114">calendarSyncEnabled</span></span>|<span data-ttu-id="70236-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="70236-115">Boolean</span></span>|<span data-ttu-id="70236-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="70236-116">Not yet documented</span></span>|
|<span data-ttu-id="70236-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="70236-117">deviceAccountEmail</span></span>|<span data-ttu-id="70236-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="70236-118">String</span></span>|<span data-ttu-id="70236-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="70236-119">Not yet documented</span></span>|
|<span data-ttu-id="70236-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="70236-120">exchangeServer</span></span>|<span data-ttu-id="70236-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="70236-121">String</span></span>|<span data-ttu-id="70236-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="70236-122">Not yet documented</span></span>|
|<span data-ttu-id="70236-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="70236-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="70236-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="70236-124">String</span></span>|<span data-ttu-id="70236-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="70236-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="70236-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="70236-126">Relationships</span></span>
<span data-ttu-id="70236-127">なし</span><span class="sxs-lookup"><span data-stu-id="70236-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="70236-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70236-128">JSON Representation</span></span>
<span data-ttu-id="70236-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="70236-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```








