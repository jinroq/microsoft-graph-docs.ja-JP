# <a name="omasettingstring-resource-type"></a><span data-ttu-id="769b1-101">omaSettingString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="769b1-101">omaSettingString resource type</span></span>

> <span data-ttu-id="769b1-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="769b1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="769b1-103">OMA 設定の文字列の定義です。</span><span class="sxs-lookup"><span data-stu-id="769b1-103">OMA Settings String definition.</span></span>

<span data-ttu-id="769b1-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="769b1-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="769b1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="769b1-105">Properties</span></span>
|<span data-ttu-id="769b1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="769b1-106">Property</span></span>|<span data-ttu-id="769b1-107">型</span><span class="sxs-lookup"><span data-stu-id="769b1-107">Type</span></span>|<span data-ttu-id="769b1-108">説明</span><span class="sxs-lookup"><span data-stu-id="769b1-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="769b1-109">displayName</span><span class="sxs-lookup"><span data-stu-id="769b1-109">displayName</span></span>|<span data-ttu-id="769b1-110">文字列</span><span class="sxs-lookup"><span data-stu-id="769b1-110">String</span></span>|<span data-ttu-id="769b1-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="769b1-111">Display Name.</span></span> <span data-ttu-id="769b1-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="769b1-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="769b1-113">説明</span><span class="sxs-lookup"><span data-stu-id="769b1-113">description</span></span>|<span data-ttu-id="769b1-114">文字列</span><span class="sxs-lookup"><span data-stu-id="769b1-114">String</span></span>|<span data-ttu-id="769b1-115">説明。</span><span class="sxs-lookup"><span data-stu-id="769b1-115">Description.</span></span> <span data-ttu-id="769b1-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="769b1-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="769b1-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="769b1-117">omaUri</span></span>|<span data-ttu-id="769b1-118">文字列</span><span class="sxs-lookup"><span data-stu-id="769b1-118">String</span></span>|<span data-ttu-id="769b1-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="769b1-119">OMA.</span></span> <span data-ttu-id="769b1-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="769b1-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="769b1-121">value</span><span class="sxs-lookup"><span data-stu-id="769b1-121">value</span></span>|<span data-ttu-id="769b1-122">文字列</span><span class="sxs-lookup"><span data-stu-id="769b1-122">String</span></span>|<span data-ttu-id="769b1-123">値。</span><span class="sxs-lookup"><span data-stu-id="769b1-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="769b1-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="769b1-124">Relationships</span></span>
<span data-ttu-id="769b1-125">なし</span><span class="sxs-lookup"><span data-stu-id="769b1-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="769b1-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="769b1-126">JSON Representation</span></span>
<span data-ttu-id="769b1-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="769b1-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```








