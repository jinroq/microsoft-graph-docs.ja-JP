# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="a969e-101">outlookGeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a969e-101">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="a969e-102">物理的な場所に関する地理的な座標と標高、およびそれらの値の精度を表します。</span><span class="sxs-lookup"><span data-stu-id="a969e-102">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a969e-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a969e-103">JSON representation</span></span>

<span data-ttu-id="a969e-104">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a969e-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="a969e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a969e-105">Properties</span></span>
| <span data-ttu-id="a969e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a969e-106">Property</span></span>     | <span data-ttu-id="a969e-107">型</span><span class="sxs-lookup"><span data-stu-id="a969e-107">Type</span></span>   |<span data-ttu-id="a969e-108">説明</span><span class="sxs-lookup"><span data-stu-id="a969e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a969e-109">accuracy</span><span class="sxs-lookup"><span data-stu-id="a969e-109">Accuracy</span></span>|<span data-ttu-id="a969e-110">double</span><span class="sxs-lookup"><span data-stu-id="a969e-110">double</span></span>|<span data-ttu-id="a969e-111">緯度と経度の精度です。</span><span class="sxs-lookup"><span data-stu-id="a969e-111">The accuracy of the sensor providing the latitude and longitude.</span></span> <span data-ttu-id="a969e-112">一例として、緯度と経度の精度が 50 メートル以内となるように、精度をメートル単位で測定することができます。</span><span class="sxs-lookup"><span data-stu-id="a969e-112">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="a969e-113">altitude</span><span class="sxs-lookup"><span data-stu-id="a969e-113">altitude</span></span>|<span data-ttu-id="a969e-114">double</span><span class="sxs-lookup"><span data-stu-id="a969e-114">double</span></span>|<span data-ttu-id="a969e-115">場所の標高です。</span><span class="sxs-lookup"><span data-stu-id="a969e-115">The altitude of the location.</span></span>|
|<span data-ttu-id="a969e-116">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="a969e-116">AltitudeAccuracy</span></span>|<span data-ttu-id="a969e-117">double</span><span class="sxs-lookup"><span data-stu-id="a969e-117">double</span></span>|<span data-ttu-id="a969e-118">標高の精度。</span><span class="sxs-lookup"><span data-stu-id="a969e-118">The accuracy of the sensor providing the altitude.</span></span>|
|<span data-ttu-id="a969e-119">latitude</span><span class="sxs-lookup"><span data-stu-id="a969e-119">latitude</span></span>|<span data-ttu-id="a969e-120">double</span><span class="sxs-lookup"><span data-stu-id="a969e-120">double</span></span>|<span data-ttu-id="a969e-121">場所の緯度です。</span><span class="sxs-lookup"><span data-stu-id="a969e-121">The latitude of the location.</span></span>|
|<span data-ttu-id="a969e-122">longitude</span><span class="sxs-lookup"><span data-stu-id="a969e-122">longitude</span></span>|<span data-ttu-id="a969e-123">double</span><span class="sxs-lookup"><span data-stu-id="a969e-123">double</span></span>|<span data-ttu-id="a969e-124">場所の経度です。</span><span class="sxs-lookup"><span data-stu-id="a969e-124">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->