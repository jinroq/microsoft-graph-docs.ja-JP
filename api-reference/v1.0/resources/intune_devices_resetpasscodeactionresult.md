# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="76737-101">resetPasscodeActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76737-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="76737-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="76737-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76737-103">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="76737-103">Reset passcode action result</span></span>

<span data-ttu-id="76737-104">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="76737-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76737-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76737-105">Properties</span></span>
|<span data-ttu-id="76737-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76737-106">Property</span></span>|<span data-ttu-id="76737-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="76737-107">Type</span></span>|<span data-ttu-id="76737-108">説明</span><span class="sxs-lookup"><span data-stu-id="76737-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76737-109">actionName</span><span class="sxs-lookup"><span data-stu-id="76737-109">actionName</span></span>|<span data-ttu-id="76737-110">文字列</span><span class="sxs-lookup"><span data-stu-id="76737-110">String</span></span>|<span data-ttu-id="76737-111">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="76737-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="76737-112">actionState</span><span class="sxs-lookup"><span data-stu-id="76737-112">actionState</span></span>|[<span data-ttu-id="76737-113">actionState</span><span class="sxs-lookup"><span data-stu-id="76737-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="76737-p101">[DeviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承される、アクションの状態です。指定できる値は、`none`、 `pending`、 `canceled`、 `active`、 `done`、 `failed`、 `notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="76737-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="76737-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="76737-116">startDateTime</span></span>|<span data-ttu-id="76737-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76737-117">DateTimeOffset</span></span>|<span data-ttu-id="76737-118">アクションが開始された時刻 ([deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="76737-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="76737-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="76737-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="76737-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76737-120">DateTimeOffset</span></span>|<span data-ttu-id="76737-121">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="76737-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="76737-122">passcode</span><span class="sxs-lookup"><span data-stu-id="76737-122">passcode</span></span>|<span data-ttu-id="76737-123">文字列</span><span class="sxs-lookup"><span data-stu-id="76737-123">String</span></span>|<span data-ttu-id="76737-124">デバイス用に新たに生成されたパスコード</span><span class="sxs-lookup"><span data-stu-id="76737-124">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="76737-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="76737-125">Relationships</span></span>
<span data-ttu-id="76737-126">なし</span><span class="sxs-lookup"><span data-stu-id="76737-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="76737-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76737-127">JSON Representation</span></span>
<span data-ttu-id="76737-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76737-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```








