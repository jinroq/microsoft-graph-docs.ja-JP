# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="7caad-101">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7caad-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="7caad-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7caad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7caad-103">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="7caad-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="7caad-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7caad-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7caad-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7caad-105">Properties</span></span>
|<span data-ttu-id="7caad-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7caad-106">Property</span></span>|<span data-ttu-id="7caad-107">型</span><span class="sxs-lookup"><span data-stu-id="7caad-107">Type</span></span>|<span data-ttu-id="7caad-108">説明</span><span class="sxs-lookup"><span data-stu-id="7caad-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7caad-109">displayName</span><span class="sxs-lookup"><span data-stu-id="7caad-109">displayName</span></span>|<span data-ttu-id="7caad-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7caad-110">String</span></span>|<span data-ttu-id="7caad-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="7caad-111">Display Name</span></span> <span data-ttu-id="7caad-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7caad-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="7caad-113">description</span><span class="sxs-lookup"><span data-stu-id="7caad-113">description</span></span>|<span data-ttu-id="7caad-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7caad-114">String</span></span>|<span data-ttu-id="7caad-115">説明。</span><span class="sxs-lookup"><span data-stu-id="7caad-115">Description.</span></span> <span data-ttu-id="7caad-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7caad-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="7caad-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="7caad-117">omaUri</span></span>|<span data-ttu-id="7caad-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7caad-118">String</span></span>|<span data-ttu-id="7caad-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="7caad-119">OMA.</span></span> <span data-ttu-id="7caad-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7caad-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="7caad-121">fileName</span><span class="sxs-lookup"><span data-stu-id="7caad-121">FileName</span></span>|<span data-ttu-id="7caad-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7caad-122">String</span></span>|<span data-ttu-id="7caad-123">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="7caad-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="7caad-124">\*.crt )。</span><span class="sxs-lookup"><span data-stu-id="7caad-124">\*.crt ).</span></span>|
|<span data-ttu-id="7caad-125">value</span><span class="sxs-lookup"><span data-stu-id="7caad-125">value</span></span>|<span data-ttu-id="7caad-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7caad-126">String</span></span>|<span data-ttu-id="7caad-127">値。</span><span class="sxs-lookup"><span data-stu-id="7caad-127">Value.</span></span> <span data-ttu-id="7caad-128">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="7caad-128">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7caad-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7caad-129">Relationships</span></span>
<span data-ttu-id="7caad-130">なし</span><span class="sxs-lookup"><span data-stu-id="7caad-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7caad-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7caad-131">JSON Representation</span></span>
<span data-ttu-id="7caad-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7caad-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



