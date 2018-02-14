# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="653d4-101">locateDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="653d4-101">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="653d4-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="653d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="653d4-103">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="653d4-103">Locate device action result</span></span>

<span data-ttu-id="653d4-104">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="653d4-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="653d4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="653d4-105">Properties</span></span>
|<span data-ttu-id="653d4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="653d4-106">Property</span></span>|<span data-ttu-id="653d4-107">型</span><span class="sxs-lookup"><span data-stu-id="653d4-107">Type</span></span>|<span data-ttu-id="653d4-108">説明</span><span class="sxs-lookup"><span data-stu-id="653d4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="653d4-109">actionName</span><span class="sxs-lookup"><span data-stu-id="653d4-109">ActionName</span></span>|<span data-ttu-id="653d4-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="653d4-110">String</span></span>|<span data-ttu-id="653d4-111">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="653d4-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="653d4-112">actionState</span><span class="sxs-lookup"><span data-stu-id="653d4-112">actionState</span></span>|<span data-ttu-id="653d4-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="653d4-113">String</span></span>|<span data-ttu-id="653d4-114">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクションの状態。可能な値: `none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="653d4-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="653d4-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="653d4-115">startDateTime</span></span>|<span data-ttu-id="653d4-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="653d4-116">DateTimeOffset</span></span>|<span data-ttu-id="653d4-117">アクションが開始された時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="653d4-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="653d4-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="653d4-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="653d4-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="653d4-119">DateTimeOffset</span></span>|<span data-ttu-id="653d4-120">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="653d4-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="653d4-121">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="653d4-121">deviceLocation</span></span>|[<span data-ttu-id="653d4-122">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="653d4-122">deviceGeoLocation</span></span>](../resources/intune_devices_devicegeolocation.md)|<span data-ttu-id="653d4-123">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="653d4-123">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="653d4-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="653d4-124">Relationships</span></span>
<span data-ttu-id="653d4-125">なし</span><span class="sxs-lookup"><span data-stu-id="653d4-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="653d4-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="653d4-126">JSON Representation</span></span>
<span data-ttu-id="653d4-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="653d4-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
    "lastCollectedDateTime": "String (timestamp)",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "altitude": "<Unknown Primitive Type Edm.Double>",
    "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "heading": "<Unknown Primitive Type Edm.Double>",
    "speed": "<Unknown Primitive Type Edm.Double>"
  }
}
```



