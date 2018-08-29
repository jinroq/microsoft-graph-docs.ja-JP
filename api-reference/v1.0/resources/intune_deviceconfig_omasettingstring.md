# <a name="omasettingstring-resource-type"></a><span data-ttu-id="0c666-101">omaSettingString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c666-101">omaSettingString resource type</span></span>

> <span data-ttu-id="0c666-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c666-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c666-103">OMA 設定の文字列の定義です。</span><span class="sxs-lookup"><span data-stu-id="0c666-103">OMA Settings String definition.</span></span>

<span data-ttu-id="0c666-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c666-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c666-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c666-105">Properties</span></span>
|<span data-ttu-id="0c666-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c666-106">Property</span></span>|<span data-ttu-id="0c666-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="0c666-107">Type</span></span>|<span data-ttu-id="0c666-108">説明</span><span class="sxs-lookup"><span data-stu-id="0c666-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c666-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0c666-109">displayName</span></span>|<span data-ttu-id="0c666-110">文字列</span><span class="sxs-lookup"><span data-stu-id="0c666-110">String</span></span>|<span data-ttu-id="0c666-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="0c666-111">Display Name.</span></span> <span data-ttu-id="0c666-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c666-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0c666-113">説明</span><span class="sxs-lookup"><span data-stu-id="0c666-113">description</span></span>|<span data-ttu-id="0c666-114">String</span><span class="sxs-lookup"><span data-stu-id="0c666-114">String</span></span>|<span data-ttu-id="0c666-115">説明。</span><span class="sxs-lookup"><span data-stu-id="0c666-115">Description.</span></span> <span data-ttu-id="0c666-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c666-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0c666-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="0c666-117">omaUri</span></span>|<span data-ttu-id="0c666-118">文字列</span><span class="sxs-lookup"><span data-stu-id="0c666-118">String</span></span>|<span data-ttu-id="0c666-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="0c666-119">OMA.</span></span> <span data-ttu-id="0c666-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c666-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0c666-121">value</span><span class="sxs-lookup"><span data-stu-id="0c666-121">value</span></span>|<span data-ttu-id="0c666-122">文字列</span><span class="sxs-lookup"><span data-stu-id="0c666-122">String</span></span>|<span data-ttu-id="0c666-123">値。</span><span class="sxs-lookup"><span data-stu-id="0c666-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c666-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c666-124">Relationships</span></span>
<span data-ttu-id="0c666-125">なし</span><span class="sxs-lookup"><span data-stu-id="0c666-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c666-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c666-126">JSON Representation</span></span>
<span data-ttu-id="0c666-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c666-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
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



