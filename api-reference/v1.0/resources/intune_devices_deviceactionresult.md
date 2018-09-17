# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="be64f-101">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be64f-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="be64f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="be64f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be64f-103">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="be64f-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="be64f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be64f-104">Properties</span></span>
|<span data-ttu-id="be64f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be64f-105">Property</span></span>|<span data-ttu-id="be64f-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="be64f-106">Type</span></span>|<span data-ttu-id="be64f-107">説明</span><span class="sxs-lookup"><span data-stu-id="be64f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be64f-108">actionName</span><span class="sxs-lookup"><span data-stu-id="be64f-108">actionName</span></span>|<span data-ttu-id="be64f-109">文字列</span><span class="sxs-lookup"><span data-stu-id="be64f-109">String</span></span>|<span data-ttu-id="be64f-110">アクション名</span><span class="sxs-lookup"><span data-stu-id="be64f-110">Action name</span></span>|
|<span data-ttu-id="be64f-111">actionState</span><span class="sxs-lookup"><span data-stu-id="be64f-111">actionState</span></span>|[<span data-ttu-id="be64f-112">actionState</span><span class="sxs-lookup"><span data-stu-id="be64f-112">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="be64f-p101">アクションの状態。指定できる値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="be64f-p101">State of the action Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="be64f-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="be64f-115">startDateTime</span></span>|<span data-ttu-id="be64f-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be64f-116">DateTimeOffset</span></span>|<span data-ttu-id="be64f-117">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="be64f-117">Time the action was initiated</span></span>|
|<span data-ttu-id="be64f-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="be64f-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="be64f-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be64f-119">DateTimeOffset</span></span>|<span data-ttu-id="be64f-120">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="be64f-120">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="be64f-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be64f-121">Relationships</span></span>
<span data-ttu-id="be64f-122">なし</span><span class="sxs-lookup"><span data-stu-id="be64f-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be64f-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be64f-123">JSON Representation</span></span>
<span data-ttu-id="be64f-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be64f-124">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```








