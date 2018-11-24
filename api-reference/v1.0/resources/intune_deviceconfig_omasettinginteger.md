# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="42f4e-101">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42f4e-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="42f4e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="42f4e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42f4e-103">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="42f4e-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="42f4e-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="42f4e-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42f4e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42f4e-105">Properties</span></span>
|<span data-ttu-id="42f4e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42f4e-106">Property</span></span>|<span data-ttu-id="42f4e-107">型</span><span class="sxs-lookup"><span data-stu-id="42f4e-107">Type</span></span>|<span data-ttu-id="42f4e-108">説明</span><span class="sxs-lookup"><span data-stu-id="42f4e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42f4e-109">displayName</span><span class="sxs-lookup"><span data-stu-id="42f4e-109">displayName</span></span>|<span data-ttu-id="42f4e-110">文字列</span><span class="sxs-lookup"><span data-stu-id="42f4e-110">String</span></span>|<span data-ttu-id="42f4e-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="42f4e-111">Display Name.</span></span> <span data-ttu-id="42f4e-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="42f4e-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="42f4e-113">説明</span><span class="sxs-lookup"><span data-stu-id="42f4e-113">description</span></span>|<span data-ttu-id="42f4e-114">文字列</span><span class="sxs-lookup"><span data-stu-id="42f4e-114">String</span></span>|<span data-ttu-id="42f4e-115">説明。</span><span class="sxs-lookup"><span data-stu-id="42f4e-115">Description.</span></span> <span data-ttu-id="42f4e-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="42f4e-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="42f4e-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="42f4e-117">omaUri</span></span>|<span data-ttu-id="42f4e-118">文字列</span><span class="sxs-lookup"><span data-stu-id="42f4e-118">String</span></span>|<span data-ttu-id="42f4e-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="42f4e-119">OMA.</span></span> <span data-ttu-id="42f4e-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="42f4e-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="42f4e-121">値</span><span class="sxs-lookup"><span data-stu-id="42f4e-121">value</span></span>|<span data-ttu-id="42f4e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="42f4e-122">Int32</span></span>|<span data-ttu-id="42f4e-123">値。</span><span class="sxs-lookup"><span data-stu-id="42f4e-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42f4e-124">関係</span><span class="sxs-lookup"><span data-stu-id="42f4e-124">Relationships</span></span>
<span data-ttu-id="42f4e-125">なし</span><span class="sxs-lookup"><span data-stu-id="42f4e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42f4e-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42f4e-126">JSON Representation</span></span>
<span data-ttu-id="42f4e-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42f4e-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



