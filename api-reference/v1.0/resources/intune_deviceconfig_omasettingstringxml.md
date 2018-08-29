# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="bf921-101">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf921-101">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="bf921-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf921-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf921-103">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="bf921-103">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="bf921-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bf921-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf921-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf921-105">Properties</span></span>
|<span data-ttu-id="bf921-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf921-106">Property</span></span>|<span data-ttu-id="bf921-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="bf921-107">Type</span></span>|<span data-ttu-id="bf921-108">説明</span><span class="sxs-lookup"><span data-stu-id="bf921-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf921-109">displayName</span><span class="sxs-lookup"><span data-stu-id="bf921-109">displayName</span></span>|<span data-ttu-id="bf921-110">文字列</span><span class="sxs-lookup"><span data-stu-id="bf921-110">String</span></span>|<span data-ttu-id="bf921-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="bf921-111">Display Name.</span></span> <span data-ttu-id="bf921-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bf921-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="bf921-113">説明</span><span class="sxs-lookup"><span data-stu-id="bf921-113">description</span></span>|<span data-ttu-id="bf921-114">String</span><span class="sxs-lookup"><span data-stu-id="bf921-114">String</span></span>|<span data-ttu-id="bf921-115">説明。</span><span class="sxs-lookup"><span data-stu-id="bf921-115">Description.</span></span> <span data-ttu-id="bf921-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bf921-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="bf921-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="bf921-117">omaUri</span></span>|<span data-ttu-id="bf921-118">文字列</span><span class="sxs-lookup"><span data-stu-id="bf921-118">String</span></span>|<span data-ttu-id="bf921-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="bf921-119">OMA.</span></span> <span data-ttu-id="bf921-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bf921-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="bf921-121">fileName</span><span class="sxs-lookup"><span data-stu-id="bf921-121">fileName</span></span>|<span data-ttu-id="bf921-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bf921-122">String</span></span>|<span data-ttu-id="bf921-123">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="bf921-123">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="bf921-124">value</span><span class="sxs-lookup"><span data-stu-id="bf921-124">value</span></span>|<span data-ttu-id="bf921-125">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="bf921-125">Binary</span></span>|<span data-ttu-id="bf921-126">値。</span><span class="sxs-lookup"><span data-stu-id="bf921-126">Value.</span></span> <span data-ttu-id="bf921-127">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="bf921-127">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf921-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf921-128">Relationships</span></span>
<span data-ttu-id="bf921-129">なし</span><span class="sxs-lookup"><span data-stu-id="bf921-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf921-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf921-130">JSON Representation</span></span>
<span data-ttu-id="bf921-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf921-131">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



