# <a name="rgbcolor-resource-type"></a><span data-ttu-id="36ccc-101">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="36ccc-101">rgbColor resource type</span></span>

> <span data-ttu-id="36ccc-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="36ccc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36ccc-103">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="36ccc-103">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="36ccc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36ccc-104">Properties</span></span>
|<span data-ttu-id="36ccc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36ccc-105">Property</span></span>|<span data-ttu-id="36ccc-106">型</span><span class="sxs-lookup"><span data-stu-id="36ccc-106">Type</span></span>|<span data-ttu-id="36ccc-107">説明</span><span class="sxs-lookup"><span data-stu-id="36ccc-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36ccc-108">r</span><span class="sxs-lookup"><span data-stu-id="36ccc-108">r</span></span>|<span data-ttu-id="36ccc-109">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="36ccc-109">Byte</span></span>|<span data-ttu-id="36ccc-110">赤の値</span><span class="sxs-lookup"><span data-stu-id="36ccc-110">Red value</span></span>|
|<span data-ttu-id="36ccc-111">g</span><span class="sxs-lookup"><span data-stu-id="36ccc-111">g</span></span>|<span data-ttu-id="36ccc-112">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="36ccc-112">Byte</span></span>|<span data-ttu-id="36ccc-113">緑の値</span><span class="sxs-lookup"><span data-stu-id="36ccc-113">Green value</span></span>|
|<span data-ttu-id="36ccc-114">b</span><span class="sxs-lookup"><span data-stu-id="36ccc-114">b</span></span>|<span data-ttu-id="36ccc-115">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="36ccc-115">Byte</span></span>|<span data-ttu-id="36ccc-116">青の値</span><span class="sxs-lookup"><span data-stu-id="36ccc-116">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="36ccc-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="36ccc-117">Relationships</span></span>
<span data-ttu-id="36ccc-118">なし</span><span class="sxs-lookup"><span data-stu-id="36ccc-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="36ccc-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36ccc-119">JSON Representation</span></span>
<span data-ttu-id="36ccc-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="36ccc-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```



