# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="be502-101">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be502-101">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="be502-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="be502-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be502-103">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="be502-103">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="be502-104">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="be502-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="be502-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be502-105">Properties</span></span>
|<span data-ttu-id="be502-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be502-106">Property</span></span>|<span data-ttu-id="be502-107">型</span><span class="sxs-lookup"><span data-stu-id="be502-107">Type</span></span>|<span data-ttu-id="be502-108">説明</span><span class="sxs-lookup"><span data-stu-id="be502-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be502-109">displayName</span><span class="sxs-lookup"><span data-stu-id="be502-109">displayName</span></span>|<span data-ttu-id="be502-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be502-110">String</span></span>|<span data-ttu-id="be502-111">表示名。</span><span class="sxs-lookup"><span data-stu-id="be502-111">Display Name</span></span> <span data-ttu-id="be502-112">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="be502-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="be502-113">description</span><span class="sxs-lookup"><span data-stu-id="be502-113">description</span></span>|<span data-ttu-id="be502-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be502-114">String</span></span>|<span data-ttu-id="be502-115">説明。</span><span class="sxs-lookup"><span data-stu-id="be502-115">Description.</span></span> <span data-ttu-id="be502-116">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="be502-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="be502-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="be502-117">omaUri</span></span>|<span data-ttu-id="be502-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be502-118">String</span></span>|<span data-ttu-id="be502-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="be502-119">OMA.</span></span> <span data-ttu-id="be502-120">[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="be502-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="be502-121">fileName</span><span class="sxs-lookup"><span data-stu-id="be502-121">FileName</span></span>|<span data-ttu-id="be502-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be502-122">String</span></span>|<span data-ttu-id="be502-123">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="be502-123">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="be502-124">value</span><span class="sxs-lookup"><span data-stu-id="be502-124">value</span></span>|<span data-ttu-id="be502-125">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="be502-125">Binary</span></span>|<span data-ttu-id="be502-126">値。</span><span class="sxs-lookup"><span data-stu-id="be502-126">Value.</span></span> <span data-ttu-id="be502-127">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="be502-127">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="be502-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be502-128">Relationships</span></span>
<span data-ttu-id="be502-129">なし</span><span class="sxs-lookup"><span data-stu-id="be502-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be502-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be502-130">JSON Representation</span></span>
<span data-ttu-id="be502-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be502-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
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



