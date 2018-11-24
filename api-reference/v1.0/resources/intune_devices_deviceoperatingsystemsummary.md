# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="ab506-101">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab506-101">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="ab506-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab506-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab506-103">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="ab506-103">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="ab506-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab506-104">Properties</span></span>
|<span data-ttu-id="ab506-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab506-105">Property</span></span>|<span data-ttu-id="ab506-106">型</span><span class="sxs-lookup"><span data-stu-id="ab506-106">Type</span></span>|<span data-ttu-id="ab506-107">説明</span><span class="sxs-lookup"><span data-stu-id="ab506-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab506-108">androidCount</span><span class="sxs-lookup"><span data-stu-id="ab506-108">androidCount</span></span>|<span data-ttu-id="ab506-109">Int32</span><span class="sxs-lookup"><span data-stu-id="ab506-109">Int32</span></span>|<span data-ttu-id="ab506-110">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ab506-110">Number of android device count.</span></span>|
|<span data-ttu-id="ab506-111">iosCount</span><span class="sxs-lookup"><span data-stu-id="ab506-111">iosCount</span></span>|<span data-ttu-id="ab506-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ab506-112">Int32</span></span>|<span data-ttu-id="ab506-113">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ab506-113">Number of iOS device count.</span></span>|
|<span data-ttu-id="ab506-114">macOSCount</span><span class="sxs-lookup"><span data-stu-id="ab506-114">macOSCount</span></span>|<span data-ttu-id="ab506-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ab506-115">Int32</span></span>|<span data-ttu-id="ab506-116">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ab506-116">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="ab506-117">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="ab506-117">windowsMobileCount</span></span>|<span data-ttu-id="ab506-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ab506-118">Int32</span></span>|<span data-ttu-id="ab506-119">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ab506-119">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="ab506-120">windowsCount</span><span class="sxs-lookup"><span data-stu-id="ab506-120">windowsCount</span></span>|<span data-ttu-id="ab506-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ab506-121">Int32</span></span>|<span data-ttu-id="ab506-122">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ab506-122">Number of Windows device count.</span></span>|
|<span data-ttu-id="ab506-123">unknownCount</span><span class="sxs-lookup"><span data-stu-id="ab506-123">unknownCount</span></span>|<span data-ttu-id="ab506-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ab506-124">Int32</span></span>|<span data-ttu-id="ab506-125">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ab506-125">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab506-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab506-126">Relationships</span></span>
<span data-ttu-id="ab506-127">なし</span><span class="sxs-lookup"><span data-stu-id="ab506-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ab506-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab506-128">JSON Representation</span></span>
<span data-ttu-id="ab506-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ab506-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



