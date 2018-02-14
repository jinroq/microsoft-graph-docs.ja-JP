# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="81bbf-101">resetPasscodeActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81bbf-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="81bbf-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81bbf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81bbf-103">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="81bbf-103">Reset passcode action result</span></span>

<span data-ttu-id="81bbf-104">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="81bbf-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81bbf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81bbf-105">Properties</span></span>
|<span data-ttu-id="81bbf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81bbf-106">Property</span></span>|<span data-ttu-id="81bbf-107">型</span><span class="sxs-lookup"><span data-stu-id="81bbf-107">Type</span></span>|<span data-ttu-id="81bbf-108">説明</span><span class="sxs-lookup"><span data-stu-id="81bbf-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81bbf-109">actionName</span><span class="sxs-lookup"><span data-stu-id="81bbf-109">ActionName</span></span>|<span data-ttu-id="81bbf-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="81bbf-110">String</span></span>|<span data-ttu-id="81bbf-111">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="81bbf-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="81bbf-112">actionState</span><span class="sxs-lookup"><span data-stu-id="81bbf-112">actionState</span></span>|<span data-ttu-id="81bbf-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="81bbf-113">String</span></span>|<span data-ttu-id="81bbf-114">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクションの状態。可能な値: `none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="81bbf-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="81bbf-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="81bbf-115">startDateTime</span></span>|<span data-ttu-id="81bbf-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81bbf-116">DateTimeOffset</span></span>|<span data-ttu-id="81bbf-117">アクションが開始された時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="81bbf-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="81bbf-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="81bbf-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="81bbf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81bbf-119">DateTimeOffset</span></span>|<span data-ttu-id="81bbf-120">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="81bbf-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="81bbf-121">passcode</span><span class="sxs-lookup"><span data-stu-id="81bbf-121">passcode</span></span>|<span data-ttu-id="81bbf-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="81bbf-122">String</span></span>|<span data-ttu-id="81bbf-123">デバイス用に新たに生成されたパスコード</span><span class="sxs-lookup"><span data-stu-id="81bbf-123">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="81bbf-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81bbf-124">Relationships</span></span>
<span data-ttu-id="81bbf-125">なし</span><span class="sxs-lookup"><span data-stu-id="81bbf-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81bbf-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81bbf-126">JSON Representation</span></span>
<span data-ttu-id="81bbf-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="81bbf-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
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



