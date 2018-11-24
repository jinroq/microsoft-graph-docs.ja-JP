# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="17fd4-101">deviceGeoLocation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17fd4-101">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="17fd4-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="17fd4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17fd4-103">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="17fd4-103">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="17fd4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17fd4-104">Properties</span></span>
|<span data-ttu-id="17fd4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17fd4-105">Property</span></span>|<span data-ttu-id="17fd4-106">型</span><span class="sxs-lookup"><span data-stu-id="17fd4-106">Type</span></span>|<span data-ttu-id="17fd4-107">説明</span><span class="sxs-lookup"><span data-stu-id="17fd4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17fd4-108">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="17fd4-108">lastCollectedDateTime</span></span>|<span data-ttu-id="17fd4-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17fd4-109">DateTimeOffset</span></span>|<span data-ttu-id="17fd4-110">場所が記録された、UTC を基準とする時刻</span><span class="sxs-lookup"><span data-stu-id="17fd4-110">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="17fd4-111">longitude</span><span class="sxs-lookup"><span data-stu-id="17fd4-111">longitude</span></span>|<span data-ttu-id="17fd4-112">Double</span><span class="sxs-lookup"><span data-stu-id="17fd4-112">Double</span></span>|<span data-ttu-id="17fd4-113">デバイスの場所の経度座標</span><span class="sxs-lookup"><span data-stu-id="17fd4-113">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="17fd4-114">latitude</span><span class="sxs-lookup"><span data-stu-id="17fd4-114">latitude</span></span>|<span data-ttu-id="17fd4-115">Double</span><span class="sxs-lookup"><span data-stu-id="17fd4-115">Double</span></span>|<span data-ttu-id="17fd4-116">デバイスの場所の緯度座標</span><span class="sxs-lookup"><span data-stu-id="17fd4-116">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="17fd4-117">altitude</span><span class="sxs-lookup"><span data-stu-id="17fd4-117">altitude</span></span>|<span data-ttu-id="17fd4-118">Double</span><span class="sxs-lookup"><span data-stu-id="17fd4-118">Double</span></span>|<span data-ttu-id="17fd4-119">海抜標高 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="17fd4-119">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="17fd4-120">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="17fd4-120">horizontalAccuracy</span></span>|<span data-ttu-id="17fd4-121">Double</span><span class="sxs-lookup"><span data-stu-id="17fd4-121">Double</span></span>|<span data-ttu-id="17fd4-122">経度と緯度の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="17fd4-122">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="17fd4-123">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="17fd4-123">verticalAccuracy</span></span>|<span data-ttu-id="17fd4-124">Double</span><span class="sxs-lookup"><span data-stu-id="17fd4-124">Double</span></span>|<span data-ttu-id="17fd4-125">標高の精度 (メートル単位)</span><span class="sxs-lookup"><span data-stu-id="17fd4-125">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="17fd4-126">heading</span><span class="sxs-lookup"><span data-stu-id="17fd4-126">heading</span></span>|<span data-ttu-id="17fd4-127">Double</span><span class="sxs-lookup"><span data-stu-id="17fd4-127">Double</span></span>|<span data-ttu-id="17fd4-128">真北を基準とする方角</span><span class="sxs-lookup"><span data-stu-id="17fd4-128">Heading in degrees from true north</span></span>|
|<span data-ttu-id="17fd4-129">speed</span><span class="sxs-lookup"><span data-stu-id="17fd4-129">speed</span></span>|<span data-ttu-id="17fd4-130">Double</span><span class="sxs-lookup"><span data-stu-id="17fd4-130">Double</span></span>|<span data-ttu-id="17fd4-131">デバイスの移動速度 (m/秒)</span><span class="sxs-lookup"><span data-stu-id="17fd4-131">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="17fd4-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17fd4-132">Relationships</span></span>
<span data-ttu-id="17fd4-133">なし</span><span class="sxs-lookup"><span data-stu-id="17fd4-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17fd4-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17fd4-134">JSON Representation</span></span>
<span data-ttu-id="17fd4-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17fd4-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
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



