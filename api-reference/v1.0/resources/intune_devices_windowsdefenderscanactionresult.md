# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="e96d2-101">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e96d2-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="e96d2-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e96d2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e96d2-103">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="e96d2-103">Windows Defender last scan result</span></span>

<span data-ttu-id="e96d2-104">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e96d2-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e96d2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e96d2-105">Properties</span></span>
|<span data-ttu-id="e96d2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e96d2-106">Property</span></span>|<span data-ttu-id="e96d2-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="e96d2-107">Type</span></span>|<span data-ttu-id="e96d2-108">説明</span><span class="sxs-lookup"><span data-stu-id="e96d2-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e96d2-109">actionName</span><span class="sxs-lookup"><span data-stu-id="e96d2-109">actionName</span></span>|<span data-ttu-id="e96d2-110">文字列</span><span class="sxs-lookup"><span data-stu-id="e96d2-110">String</span></span>|<span data-ttu-id="e96d2-111">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="e96d2-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="e96d2-112">actionState</span><span class="sxs-lookup"><span data-stu-id="e96d2-112">actionState</span></span>|[<span data-ttu-id="e96d2-113">actionState</span><span class="sxs-lookup"><span data-stu-id="e96d2-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="e96d2-p101"> [DeviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承される、アクションの状態です。指定できる値は、`none\`、 `pending\`、 `canceled\`、 `active\`、 `done\`、 `failed\`、 `notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="e96d2-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e96d2-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e96d2-116">startDateTime</span></span>|<span data-ttu-id="e96d2-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e96d2-117">DateTimeOffset</span></span>|<span data-ttu-id="e96d2-118">アクションが開始された時刻 ([deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e96d2-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="e96d2-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e96d2-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="e96d2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e96d2-120">DateTimeOffset</span></span>|<span data-ttu-id="e96d2-121">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="e96d2-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="e96d2-122">scanType</span><span class="sxs-lookup"><span data-stu-id="e96d2-122">scanType</span></span>|<span data-ttu-id="e96d2-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e96d2-123">String</span></span>|<span data-ttu-id="e96d2-124">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="e96d2-124">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="e96d2-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e96d2-125">Relationships</span></span>
<span data-ttu-id="e96d2-126">なし</span><span class="sxs-lookup"><span data-stu-id="e96d2-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e96d2-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e96d2-127">JSON Representation</span></span>
<span data-ttu-id="e96d2-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e96d2-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}-->
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








