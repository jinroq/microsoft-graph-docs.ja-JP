# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="ece0a-101">omaSettingBoolean リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ece0a-101">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="ece0a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ece0a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ece0a-103">OMA 設定のブール定義。</span><span class="sxs-lookup"><span data-stu-id="ece0a-103">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="ece0a-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ece0a-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ece0a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ece0a-105">Properties</span></span>
|<span data-ttu-id="ece0a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ece0a-106">Property</span></span>|<span data-ttu-id="ece0a-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="ece0a-107">Type</span></span>|<span data-ttu-id="ece0a-108">説明</span><span class="sxs-lookup"><span data-stu-id="ece0a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ece0a-109">displayName</span><span class="sxs-lookup"><span data-stu-id="ece0a-109">displayName</span></span>|<span data-ttu-id="ece0a-110">文字列</span><span class="sxs-lookup"><span data-stu-id="ece0a-110">String</span></span>|<span data-ttu-id="ece0a-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="ece0a-111">Display Name.</span></span> <span data-ttu-id="ece0a-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ece0a-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ece0a-113">説明</span><span class="sxs-lookup"><span data-stu-id="ece0a-113">description</span></span>|<span data-ttu-id="ece0a-114">String</span><span class="sxs-lookup"><span data-stu-id="ece0a-114">String</span></span>|<span data-ttu-id="ece0a-115">説明。</span><span class="sxs-lookup"><span data-stu-id="ece0a-115">Description.</span></span> <span data-ttu-id="ece0a-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ece0a-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ece0a-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="ece0a-117">omaUri</span></span>|<span data-ttu-id="ece0a-118">文字列</span><span class="sxs-lookup"><span data-stu-id="ece0a-118">String</span></span>|<span data-ttu-id="ece0a-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="ece0a-119">OMA.</span></span> <span data-ttu-id="ece0a-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ece0a-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="ece0a-121">value</span><span class="sxs-lookup"><span data-stu-id="ece0a-121">value</span></span>|<span data-ttu-id="ece0a-122">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ece0a-122">Boolean</span></span>|<span data-ttu-id="ece0a-123">値。</span><span class="sxs-lookup"><span data-stu-id="ece0a-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ece0a-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ece0a-124">Relationships</span></span>
<span data-ttu-id="ece0a-125">なし</span><span class="sxs-lookup"><span data-stu-id="ece0a-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ece0a-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ece0a-126">JSON Representation</span></span>
<span data-ttu-id="ece0a-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ece0a-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



