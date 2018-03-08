# <a name="omasettingstring-resource-type"></a><span data-ttu-id="0a4ce-101">omaSettingString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a4ce-101">omaSettingString resource type</span></span>

> <span data-ttu-id="0a4ce-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a4ce-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a4ce-103">OMA 設定の文字列の定義です。</span><span class="sxs-lookup"><span data-stu-id="0a4ce-103">OMA Settings String definition.</span></span>

<span data-ttu-id="0a4ce-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0a4ce-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a4ce-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a4ce-105">Properties</span></span>
|<span data-ttu-id="0a4ce-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a4ce-106">Property</span></span>|<span data-ttu-id="0a4ce-107">型</span><span class="sxs-lookup"><span data-stu-id="0a4ce-107">Type</span></span>|<span data-ttu-id="0a4ce-108">説明</span><span class="sxs-lookup"><span data-stu-id="0a4ce-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a4ce-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0a4ce-109">displayName</span></span>|<span data-ttu-id="0a4ce-110">文字列</span><span class="sxs-lookup"><span data-stu-id="0a4ce-110">String</span></span>|<span data-ttu-id="0a4ce-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="0a4ce-111">Display Name</span></span> <span data-ttu-id="0a4ce-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0a4ce-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0a4ce-113">説明</span><span class="sxs-lookup"><span data-stu-id="0a4ce-113">description</span></span>|<span data-ttu-id="0a4ce-114">文字列</span><span class="sxs-lookup"><span data-stu-id="0a4ce-114">String</span></span>|<span data-ttu-id="0a4ce-115">説明。</span><span class="sxs-lookup"><span data-stu-id="0a4ce-115">Description.</span></span> <span data-ttu-id="0a4ce-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0a4ce-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0a4ce-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="0a4ce-117">omaUri</span></span>|<span data-ttu-id="0a4ce-118">文字列</span><span class="sxs-lookup"><span data-stu-id="0a4ce-118">String</span></span>|<span data-ttu-id="0a4ce-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="0a4ce-119">OMA.</span></span> <span data-ttu-id="0a4ce-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0a4ce-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="0a4ce-121">値</span><span class="sxs-lookup"><span data-stu-id="0a4ce-121">value</span></span>|<span data-ttu-id="0a4ce-122">文字列</span><span class="sxs-lookup"><span data-stu-id="0a4ce-122">String</span></span>|<span data-ttu-id="0a4ce-123">値。</span><span class="sxs-lookup"><span data-stu-id="0a4ce-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a4ce-124">関係</span><span class="sxs-lookup"><span data-stu-id="0a4ce-124">Relationships</span></span>
<span data-ttu-id="0a4ce-125">なし</span><span class="sxs-lookup"><span data-stu-id="0a4ce-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a4ce-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a4ce-126">JSON Representation</span></span>
<span data-ttu-id="0a4ce-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a4ce-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```


