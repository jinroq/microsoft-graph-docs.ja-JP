# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="c1aa8-101">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1aa8-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="c1aa8-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1aa8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1aa8-103">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="c1aa8-103">Windows Defender last scan result</span></span>

<span data-ttu-id="c1aa8-104">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c1aa8-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1aa8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1aa8-105">Properties</span></span>
|<span data-ttu-id="c1aa8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1aa8-106">Property</span></span>|<span data-ttu-id="c1aa8-107">型</span><span class="sxs-lookup"><span data-stu-id="c1aa8-107">Type</span></span>|<span data-ttu-id="c1aa8-108">説明</span><span class="sxs-lookup"><span data-stu-id="c1aa8-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1aa8-109">actionName</span><span class="sxs-lookup"><span data-stu-id="c1aa8-109">ActionName</span></span>|<span data-ttu-id="c1aa8-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c1aa8-110">String</span></span>|<span data-ttu-id="c1aa8-111">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="c1aa8-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1aa8-112">actionState</span><span class="sxs-lookup"><span data-stu-id="c1aa8-112">actionState</span></span>|<span data-ttu-id="c1aa8-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c1aa8-113">String</span></span>|<span data-ttu-id="c1aa8-114">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクションの状態。可能な値: `none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="c1aa8-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c1aa8-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c1aa8-115">startDateTime</span></span>|<span data-ttu-id="c1aa8-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1aa8-116">DateTimeOffset</span></span>|<span data-ttu-id="c1aa8-117">アクションが開始された時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="c1aa8-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1aa8-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1aa8-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="c1aa8-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1aa8-119">DateTimeOffset</span></span>|<span data-ttu-id="c1aa8-120">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="c1aa8-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1aa8-121">scanType</span><span class="sxs-lookup"><span data-stu-id="c1aa8-121">scanType</span></span>|<span data-ttu-id="c1aa8-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c1aa8-122">String</span></span>|<span data-ttu-id="c1aa8-123">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="c1aa8-123">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1aa8-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1aa8-124">Relationships</span></span>
<span data-ttu-id="c1aa8-125">なし</span><span class="sxs-lookup"><span data-stu-id="c1aa8-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1aa8-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1aa8-126">JSON Representation</span></span>
<span data-ttu-id="c1aa8-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1aa8-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



