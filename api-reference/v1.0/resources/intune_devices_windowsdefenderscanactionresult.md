# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="d1116-101">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1116-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="d1116-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1116-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1116-103">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="d1116-103">Windows Defender last scan result</span></span>

<span data-ttu-id="d1116-104">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d1116-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1116-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1116-105">Properties</span></span>
|<span data-ttu-id="d1116-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1116-106">Property</span></span>|<span data-ttu-id="d1116-107">型</span><span class="sxs-lookup"><span data-stu-id="d1116-107">Type</span></span>|<span data-ttu-id="d1116-108">説明</span><span class="sxs-lookup"><span data-stu-id="d1116-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1116-109">actionName</span><span class="sxs-lookup"><span data-stu-id="d1116-109">actionName</span></span>|<span data-ttu-id="d1116-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d1116-110">String</span></span>|<span data-ttu-id="d1116-111">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="d1116-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="d1116-112">actionState</span><span class="sxs-lookup"><span data-stu-id="d1116-112">actionState</span></span>|[<span data-ttu-id="d1116-113">actionState</span><span class="sxs-lookup"><span data-stu-id="d1116-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="d1116-114">[DeviceActionResult](../resources/intune_devices_deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="d1116-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span></span> <span data-ttu-id="d1116-115">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="d1116-115">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d1116-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d1116-116">startDateTime</span></span>|<span data-ttu-id="d1116-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1116-117">DateTimeOffset</span></span>|<span data-ttu-id="d1116-118">アクションが開始された時刻 ([deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="d1116-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="d1116-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1116-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="d1116-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1116-120">DateTimeOffset</span></span>|<span data-ttu-id="d1116-121">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="d1116-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="d1116-122">scanType</span><span class="sxs-lookup"><span data-stu-id="d1116-122">scanType</span></span>|<span data-ttu-id="d1116-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d1116-123">String</span></span>|<span data-ttu-id="d1116-124">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="d1116-124">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1116-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1116-125">Relationships</span></span>
<span data-ttu-id="d1116-126">なし</span><span class="sxs-lookup"><span data-stu-id="d1116-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1116-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1116-127">JSON Representation</span></span>
<span data-ttu-id="d1116-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1116-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



