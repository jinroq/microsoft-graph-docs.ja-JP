# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="d046f-101">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d046f-101">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="d046f-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d046f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d046f-103">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="d046f-103">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="d046f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d046f-104">Properties</span></span>
|<span data-ttu-id="d046f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d046f-105">Property</span></span>|<span data-ttu-id="d046f-106">型</span><span class="sxs-lookup"><span data-stu-id="d046f-106">Type</span></span>|<span data-ttu-id="d046f-107">説明</span><span class="sxs-lookup"><span data-stu-id="d046f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d046f-108">androidCount</span><span class="sxs-lookup"><span data-stu-id="d046f-108">androidCount</span></span>|<span data-ttu-id="d046f-109">Int32</span><span class="sxs-lookup"><span data-stu-id="d046f-109">Int32</span></span>|<span data-ttu-id="d046f-110">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d046f-110">Number of android device count.</span></span>|
|<span data-ttu-id="d046f-111">iosCount</span><span class="sxs-lookup"><span data-stu-id="d046f-111">iosCount</span></span>|<span data-ttu-id="d046f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d046f-112">Int32</span></span>|<span data-ttu-id="d046f-113">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d046f-113">Number of iOS device count.</span></span>|
|<span data-ttu-id="d046f-114">macOSCount</span><span class="sxs-lookup"><span data-stu-id="d046f-114">macOSCount</span></span>|<span data-ttu-id="d046f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d046f-115">Int32</span></span>|<span data-ttu-id="d046f-116">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d046f-116">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="d046f-117">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="d046f-117">windowsMobileCount</span></span>|<span data-ttu-id="d046f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d046f-118">Int32</span></span>|<span data-ttu-id="d046f-119">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d046f-119">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="d046f-120">windowsCount</span><span class="sxs-lookup"><span data-stu-id="d046f-120">windowsCount</span></span>|<span data-ttu-id="d046f-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d046f-121">Int32</span></span>|<span data-ttu-id="d046f-122">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d046f-122">Number of Windows device count.</span></span>|
|<span data-ttu-id="d046f-123">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d046f-123">unknownCount</span></span>|<span data-ttu-id="d046f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d046f-124">Int32</span></span>|<span data-ttu-id="d046f-125">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d046f-125">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d046f-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d046f-126">Relationships</span></span>
<span data-ttu-id="d046f-127">なし</span><span class="sxs-lookup"><span data-stu-id="d046f-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d046f-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d046f-128">JSON Representation</span></span>
<span data-ttu-id="d046f-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d046f-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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


