# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="20e50-101">omaSettingFloatingPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20e50-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="20e50-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="20e50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20e50-103">OMA 設定の浮動小数点の定義です。</span><span class="sxs-lookup"><span data-stu-id="20e50-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="20e50-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="20e50-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="20e50-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20e50-105">Properties</span></span>
|<span data-ttu-id="20e50-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20e50-106">Property</span></span>|<span data-ttu-id="20e50-107">型</span><span class="sxs-lookup"><span data-stu-id="20e50-107">Type</span></span>|<span data-ttu-id="20e50-108">説明</span><span class="sxs-lookup"><span data-stu-id="20e50-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20e50-109">displayName</span><span class="sxs-lookup"><span data-stu-id="20e50-109">displayName</span></span>|<span data-ttu-id="20e50-110">文字列</span><span class="sxs-lookup"><span data-stu-id="20e50-110">String</span></span>|<span data-ttu-id="20e50-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="20e50-111">Display Name.</span></span> <span data-ttu-id="20e50-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="20e50-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="20e50-113">説明</span><span class="sxs-lookup"><span data-stu-id="20e50-113">description</span></span>|<span data-ttu-id="20e50-114">文字列</span><span class="sxs-lookup"><span data-stu-id="20e50-114">String</span></span>|<span data-ttu-id="20e50-115">説明。</span><span class="sxs-lookup"><span data-stu-id="20e50-115">Description.</span></span> <span data-ttu-id="20e50-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="20e50-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="20e50-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="20e50-117">omaUri</span></span>|<span data-ttu-id="20e50-118">文字列</span><span class="sxs-lookup"><span data-stu-id="20e50-118">String</span></span>|<span data-ttu-id="20e50-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="20e50-119">OMA.</span></span> <span data-ttu-id="20e50-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="20e50-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="20e50-121">値</span><span class="sxs-lookup"><span data-stu-id="20e50-121">value</span></span>|<span data-ttu-id="20e50-122">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="20e50-122">Single</span></span>|<span data-ttu-id="20e50-123">値。</span><span class="sxs-lookup"><span data-stu-id="20e50-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20e50-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="20e50-124">Relationships</span></span>
<span data-ttu-id="20e50-125">なし</span><span class="sxs-lookup"><span data-stu-id="20e50-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20e50-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20e50-126">JSON Representation</span></span>
<span data-ttu-id="20e50-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20e50-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```








