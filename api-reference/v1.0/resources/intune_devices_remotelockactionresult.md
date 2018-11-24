# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="9136f-101">remoteLockActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9136f-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="9136f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9136f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9136f-103">ロック解除するためのピンが含まれるアクション結果のロック。</span><span class="sxs-lookup"><span data-stu-id="9136f-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="9136f-104">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9136f-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9136f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9136f-105">Properties</span></span>
|<span data-ttu-id="9136f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9136f-106">Property</span></span>|<span data-ttu-id="9136f-107">型</span><span class="sxs-lookup"><span data-stu-id="9136f-107">Type</span></span>|<span data-ttu-id="9136f-108">説明</span><span class="sxs-lookup"><span data-stu-id="9136f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9136f-109">actionName</span><span class="sxs-lookup"><span data-stu-id="9136f-109">actionName</span></span>|<span data-ttu-id="9136f-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9136f-110">String</span></span>|<span data-ttu-id="9136f-111">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="9136f-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9136f-112">actionState</span><span class="sxs-lookup"><span data-stu-id="9136f-112">actionState</span></span>|[<span data-ttu-id="9136f-113">actionState</span><span class="sxs-lookup"><span data-stu-id="9136f-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="9136f-114">[DeviceActionResult](../resources/intune_devices_deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="9136f-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span></span> <span data-ttu-id="9136f-115">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="9136f-115">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9136f-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9136f-116">startDateTime</span></span>|<span data-ttu-id="9136f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9136f-117">DateTimeOffset</span></span>|<span data-ttu-id="9136f-118">アクションが開始された時刻 ([deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="9136f-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9136f-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9136f-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="9136f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9136f-120">DateTimeOffset</span></span>|<span data-ttu-id="9136f-121">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="9136f-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9136f-122">unlockPin</span><span class="sxs-lookup"><span data-stu-id="9136f-122">unlockPin</span></span>|<span data-ttu-id="9136f-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9136f-123">String</span></span>|<span data-ttu-id="9136f-124">クライアントをロック解除するためのピン</span><span class="sxs-lookup"><span data-stu-id="9136f-124">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="9136f-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9136f-125">Relationships</span></span>
<span data-ttu-id="9136f-126">なし</span><span class="sxs-lookup"><span data-stu-id="9136f-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9136f-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9136f-127">JSON Representation</span></span>
<span data-ttu-id="9136f-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9136f-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



