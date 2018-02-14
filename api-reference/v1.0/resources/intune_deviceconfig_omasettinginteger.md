# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="212c0-101">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="212c0-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="212c0-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="212c0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="212c0-103">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="212c0-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="212c0-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="212c0-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="212c0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="212c0-105">Properties</span></span>
|<span data-ttu-id="212c0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="212c0-106">Property</span></span>|<span data-ttu-id="212c0-107">型</span><span class="sxs-lookup"><span data-stu-id="212c0-107">Type</span></span>|<span data-ttu-id="212c0-108">説明</span><span class="sxs-lookup"><span data-stu-id="212c0-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="212c0-109">displayName</span><span class="sxs-lookup"><span data-stu-id="212c0-109">displayName</span></span>|<span data-ttu-id="212c0-110">文字列</span><span class="sxs-lookup"><span data-stu-id="212c0-110">String</span></span>|<span data-ttu-id="212c0-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="212c0-111">Display Name</span></span> <span data-ttu-id="212c0-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="212c0-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="212c0-113">説明</span><span class="sxs-lookup"><span data-stu-id="212c0-113">description</span></span>|<span data-ttu-id="212c0-114">文字列</span><span class="sxs-lookup"><span data-stu-id="212c0-114">String</span></span>|<span data-ttu-id="212c0-115">説明。</span><span class="sxs-lookup"><span data-stu-id="212c0-115">Description.</span></span> <span data-ttu-id="212c0-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="212c0-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="212c0-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="212c0-117">omaUri</span></span>|<span data-ttu-id="212c0-118">文字列</span><span class="sxs-lookup"><span data-stu-id="212c0-118">String</span></span>|<span data-ttu-id="212c0-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="212c0-119">OMA.</span></span> <span data-ttu-id="212c0-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="212c0-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="212c0-121">値</span><span class="sxs-lookup"><span data-stu-id="212c0-121">value</span></span>|<span data-ttu-id="212c0-122">Int32</span><span class="sxs-lookup"><span data-stu-id="212c0-122">Int32</span></span>|<span data-ttu-id="212c0-123">値。</span><span class="sxs-lookup"><span data-stu-id="212c0-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="212c0-124">関係</span><span class="sxs-lookup"><span data-stu-id="212c0-124">Relationships</span></span>
<span data-ttu-id="212c0-125">なし</span><span class="sxs-lookup"><span data-stu-id="212c0-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="212c0-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="212c0-126">JSON Representation</span></span>
<span data-ttu-id="212c0-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="212c0-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



