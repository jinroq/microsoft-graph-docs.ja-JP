# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="b40e3-101">windowsInformationProtectionDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b40e3-101">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="b40e3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b40e3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b40e3-103">Windows 情報保護用デスクトップ アプリ</span><span class="sxs-lookup"><span data-stu-id="b40e3-103">Desktop App for Windows information protection</span></span>

<span data-ttu-id="b40e3-104">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b40e3-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b40e3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b40e3-105">Properties</span></span>
|<span data-ttu-id="b40e3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b40e3-106">Property</span></span>|<span data-ttu-id="b40e3-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="b40e3-107">Type</span></span>|<span data-ttu-id="b40e3-108">説明</span><span class="sxs-lookup"><span data-stu-id="b40e3-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b40e3-109">displayName</span><span class="sxs-lookup"><span data-stu-id="b40e3-109">displayName</span></span>|<span data-ttu-id="b40e3-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b40e3-110">String</span></span>|<span data-ttu-id="b40e3-111">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="b40e3-111">App display name.</span></span> <span data-ttu-id="b40e3-112">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b40e3-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b40e3-113">説明</span><span class="sxs-lookup"><span data-stu-id="b40e3-113">description</span></span>|<span data-ttu-id="b40e3-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b40e3-114">String</span></span>|<span data-ttu-id="b40e3-115">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b40e3-115">The app's description.</span></span> <span data-ttu-id="b40e3-116">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b40e3-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b40e3-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="b40e3-117">publisherName</span></span>|<span data-ttu-id="b40e3-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b40e3-118">String</span></span>|<span data-ttu-id="b40e3-119">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="b40e3-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b40e3-120">productName</span><span class="sxs-lookup"><span data-stu-id="b40e3-120">productName</span></span>|<span data-ttu-id="b40e3-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b40e3-121">String</span></span>|<span data-ttu-id="b40e3-122">製品名。</span><span class="sxs-lookup"><span data-stu-id="b40e3-122">The product name.</span></span> <span data-ttu-id="b40e3-123">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b40e3-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b40e3-124">denied</span><span class="sxs-lookup"><span data-stu-id="b40e3-124">denied</span></span>|<span data-ttu-id="b40e3-125">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b40e3-125">Boolean</span></span>|<span data-ttu-id="b40e3-126">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="b40e3-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="b40e3-127">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b40e3-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b40e3-128">binaryName</span><span class="sxs-lookup"><span data-stu-id="b40e3-128">binaryName</span></span>|<span data-ttu-id="b40e3-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b40e3-129">String</span></span>|<span data-ttu-id="b40e3-130">バイナリの名前。</span><span class="sxs-lookup"><span data-stu-id="b40e3-130">The binary name.</span></span>|
|<span data-ttu-id="b40e3-131">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="b40e3-131">binaryVersionLow</span></span>|<span data-ttu-id="b40e3-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b40e3-132">String</span></span>|<span data-ttu-id="b40e3-133">下位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="b40e3-133">The lower binary version.</span></span>|
|<span data-ttu-id="b40e3-134">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="b40e3-134">binaryVersionHigh</span></span>|<span data-ttu-id="b40e3-135">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b40e3-135">String</span></span>|<span data-ttu-id="b40e3-136">上位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="b40e3-136">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b40e3-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b40e3-137">Relationships</span></span>
<span data-ttu-id="b40e3-138">なし</span><span class="sxs-lookup"><span data-stu-id="b40e3-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b40e3-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b40e3-139">JSON Representation</span></span>
<span data-ttu-id="b40e3-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b40e3-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsInformationProtectionApp",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



