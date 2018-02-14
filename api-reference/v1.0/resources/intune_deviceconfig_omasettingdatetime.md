# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="0c131-101">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c131-101">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="0c131-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c131-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c131-103">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="0c131-103">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="0c131-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c131-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c131-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c131-105">Properties</span></span>
|<span data-ttu-id="0c131-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c131-106">Property</span></span>|<span data-ttu-id="0c131-107">型</span><span class="sxs-lookup"><span data-stu-id="0c131-107">Type</span></span>|<span data-ttu-id="0c131-108">説明</span><span class="sxs-lookup"><span data-stu-id="0c131-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c131-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0c131-109">displayName</span></span>|<span data-ttu-id="0c131-110">文字列</span><span class="sxs-lookup"><span data-stu-id="0c131-110">String</span></span>|<span data-ttu-id="0c131-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="0c131-111">Display Name</span></span> <span data-ttu-id="0c131-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c131-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0c131-113">説明</span><span class="sxs-lookup"><span data-stu-id="0c131-113">description</span></span>|<span data-ttu-id="0c131-114">文字列</span><span class="sxs-lookup"><span data-stu-id="0c131-114">String</span></span>|<span data-ttu-id="0c131-115">説明。</span><span class="sxs-lookup"><span data-stu-id="0c131-115">Description.</span></span> <span data-ttu-id="0c131-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c131-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0c131-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="0c131-117">omaUri</span></span>|<span data-ttu-id="0c131-118">文字列</span><span class="sxs-lookup"><span data-stu-id="0c131-118">String</span></span>|<span data-ttu-id="0c131-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="0c131-119">OMA.</span></span> <span data-ttu-id="0c131-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c131-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0c131-121">値</span><span class="sxs-lookup"><span data-stu-id="0c131-121">value</span></span>|<span data-ttu-id="0c131-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c131-122">DateTimeOffset</span></span>|<span data-ttu-id="0c131-123">値。</span><span class="sxs-lookup"><span data-stu-id="0c131-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c131-124">関係</span><span class="sxs-lookup"><span data-stu-id="0c131-124">Relationships</span></span>
<span data-ttu-id="0c131-125">なし</span><span class="sxs-lookup"><span data-stu-id="0c131-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c131-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c131-126">JSON Representation</span></span>
<span data-ttu-id="0c131-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c131-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



