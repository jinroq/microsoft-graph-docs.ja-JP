# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="35b6e-101">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35b6e-101">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="35b6e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="35b6e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35b6e-103">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="35b6e-103">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="35b6e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35b6e-104">Properties</span></span>
|<span data-ttu-id="35b6e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35b6e-105">Property</span></span>|<span data-ttu-id="35b6e-106">型</span><span class="sxs-lookup"><span data-stu-id="35b6e-106">Type</span></span>|<span data-ttu-id="35b6e-107">説明</span><span class="sxs-lookup"><span data-stu-id="35b6e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35b6e-108">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="35b6e-108">lastCollectedDateTime</span></span>|<span data-ttu-id="35b6e-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35b6e-109">DateTimeOffset</span></span>|<span data-ttu-id="35b6e-110">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="35b6e-110">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="35b6e-111">longitude</span><span class="sxs-lookup"><span data-stu-id="35b6e-111">longitude</span></span>|<span data-ttu-id="35b6e-112">Double</span><span class="sxs-lookup"><span data-stu-id="35b6e-112">Double</span></span>|<span data-ttu-id="35b6e-113">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="35b6e-113">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="35b6e-114">latitude</span><span class="sxs-lookup"><span data-stu-id="35b6e-114">latitude</span></span>|<span data-ttu-id="35b6e-115">Double</span><span class="sxs-lookup"><span data-stu-id="35b6e-115">Double</span></span>|<span data-ttu-id="35b6e-116">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="35b6e-116">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="35b6e-117">altitude</span><span class="sxs-lookup"><span data-stu-id="35b6e-117">altitude</span></span>|<span data-ttu-id="35b6e-118">Double</span><span class="sxs-lookup"><span data-stu-id="35b6e-118">Double</span></span>|<span data-ttu-id="35b6e-119">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="35b6e-119">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="35b6e-120">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="35b6e-120">horizontalAccuracy</span></span>|<span data-ttu-id="35b6e-121">Double</span><span class="sxs-lookup"><span data-stu-id="35b6e-121">Double</span></span>|<span data-ttu-id="35b6e-122">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="35b6e-122">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="35b6e-123">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="35b6e-123">verticalAccuracy</span></span>|<span data-ttu-id="35b6e-124">Double</span><span class="sxs-lookup"><span data-stu-id="35b6e-124">Double</span></span>|<span data-ttu-id="35b6e-125">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="35b6e-125">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="35b6e-126">heading</span><span class="sxs-lookup"><span data-stu-id="35b6e-126">heading</span></span>|<span data-ttu-id="35b6e-127">Double</span><span class="sxs-lookup"><span data-stu-id="35b6e-127">Double</span></span>|<span data-ttu-id="35b6e-128">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="35b6e-128">Heading in degrees from true north</span></span>|
|<span data-ttu-id="35b6e-129">speed</span><span class="sxs-lookup"><span data-stu-id="35b6e-129">speed</span></span>|<span data-ttu-id="35b6e-130">Double</span><span class="sxs-lookup"><span data-stu-id="35b6e-130">Double</span></span>|<span data-ttu-id="35b6e-131">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="35b6e-131">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="35b6e-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35b6e-132">Relationships</span></span>
<span data-ttu-id="35b6e-133">なし</span><span class="sxs-lookup"><span data-stu-id="35b6e-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="35b6e-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35b6e-134">JSON Representation</span></span>
<span data-ttu-id="35b6e-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35b6e-135">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```








