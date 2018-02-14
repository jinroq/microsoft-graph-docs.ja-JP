# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="ea3c6-101">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ea3c6-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="ea3c6-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ea3c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea3c6-103">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="ea3c6-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="ea3c6-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea3c6-104">Properties</span></span>
|<span data-ttu-id="ea3c6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea3c6-105">Property</span></span>|<span data-ttu-id="ea3c6-106">型</span><span class="sxs-lookup"><span data-stu-id="ea3c6-106">Type</span></span>|<span data-ttu-id="ea3c6-107">説明</span><span class="sxs-lookup"><span data-stu-id="ea3c6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea3c6-108">actionName</span><span class="sxs-lookup"><span data-stu-id="ea3c6-108">ActionName</span></span>|<span data-ttu-id="ea3c6-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ea3c6-109">String</span></span>|<span data-ttu-id="ea3c6-110">アクション名</span><span class="sxs-lookup"><span data-stu-id="ea3c6-110">Action name</span></span>|
|<span data-ttu-id="ea3c6-111">actionState</span><span class="sxs-lookup"><span data-stu-id="ea3c6-111">actionState</span></span>|<span data-ttu-id="ea3c6-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ea3c6-112">String</span></span>|<span data-ttu-id="ea3c6-113">アクションの状態。可能な値: `none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="ea3c6-113">State of the action Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ea3c6-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ea3c6-114">startDateTime</span></span>|<span data-ttu-id="ea3c6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea3c6-115">DateTimeOffset</span></span>|<span data-ttu-id="ea3c6-116">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="ea3c6-116">Time the action was initiated</span></span>|
|<span data-ttu-id="ea3c6-117">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea3c6-117">lastUpdatedDateTime</span></span>|<span data-ttu-id="ea3c6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea3c6-118">DateTimeOffset</span></span>|<span data-ttu-id="ea3c6-119">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="ea3c6-119">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea3c6-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ea3c6-120">Relationships</span></span>
<span data-ttu-id="ea3c6-121">なし</span><span class="sxs-lookup"><span data-stu-id="ea3c6-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea3c6-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ea3c6-122">JSON Representation</span></span>
<span data-ttu-id="ea3c6-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ea3c6-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



