# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="1ea31-101">deviceExchangeAccessStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1ea31-101">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="1ea31-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ea31-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ea31-103">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="1ea31-103">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="1ea31-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ea31-104">Properties</span></span>
|<span data-ttu-id="1ea31-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ea31-105">Property</span></span>|<span data-ttu-id="1ea31-106">型</span><span class="sxs-lookup"><span data-stu-id="1ea31-106">Type</span></span>|<span data-ttu-id="1ea31-107">説明</span><span class="sxs-lookup"><span data-stu-id="1ea31-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ea31-108">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1ea31-108">allowedDeviceCount</span></span>|<span data-ttu-id="1ea31-109">Int32</span><span class="sxs-lookup"><span data-stu-id="1ea31-109">Int32</span></span>|<span data-ttu-id="1ea31-110">Exchange アクセス状態が Allowed のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="1ea31-110">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="1ea31-111">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1ea31-111">blockedDeviceCount</span></span>|<span data-ttu-id="1ea31-112">Int32</span><span class="sxs-lookup"><span data-stu-id="1ea31-112">Int32</span></span>|<span data-ttu-id="1ea31-113">Exchange アクセス状態が Blocked のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="1ea31-113">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="1ea31-114">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1ea31-114">quarantinedDeviceCount</span></span>|<span data-ttu-id="1ea31-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1ea31-115">Int32</span></span>|<span data-ttu-id="1ea31-116">Exchange アクセス状態が Quarantined のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="1ea31-116">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="1ea31-117">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1ea31-117">unknownDeviceCount</span></span>|<span data-ttu-id="1ea31-118">Int32</span><span class="sxs-lookup"><span data-stu-id="1ea31-118">Int32</span></span>|<span data-ttu-id="1ea31-119">Exchange アクセス状態が Unknown のデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="1ea31-119">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="1ea31-120">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1ea31-120">unavailableDeviceCount</span></span>|<span data-ttu-id="1ea31-121">Int32</span><span class="sxs-lookup"><span data-stu-id="1ea31-121">Int32</span></span>|<span data-ttu-id="1ea31-122">Exchange アクセス状態を検出できなかったデバイスの総数です。</span><span class="sxs-lookup"><span data-stu-id="1ea31-122">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ea31-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ea31-123">Relationships</span></span>
<span data-ttu-id="1ea31-124">なし</span><span class="sxs-lookup"><span data-stu-id="1ea31-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ea31-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ea31-125">JSON Representation</span></span>
<span data-ttu-id="1ea31-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1ea31-126">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```








