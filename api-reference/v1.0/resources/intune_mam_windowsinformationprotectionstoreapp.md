# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="f6112-101">windowsInformationProtectionStoreApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6112-101">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="f6112-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6112-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6112-103">Windows 情報保護のストア アプリ</span><span class="sxs-lookup"><span data-stu-id="f6112-103">Store App for Windows information protection</span></span>

<span data-ttu-id="f6112-104">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f6112-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f6112-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6112-105">Properties</span></span>
|<span data-ttu-id="f6112-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6112-106">Property</span></span>|<span data-ttu-id="f6112-107">型</span><span class="sxs-lookup"><span data-stu-id="f6112-107">Type</span></span>|<span data-ttu-id="f6112-108">説明</span><span class="sxs-lookup"><span data-stu-id="f6112-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6112-109">displayName</span><span class="sxs-lookup"><span data-stu-id="f6112-109">displayName</span></span>|<span data-ttu-id="f6112-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6112-110">String</span></span>|<span data-ttu-id="f6112-111">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="f6112-111">App display name.</span></span> <span data-ttu-id="f6112-112">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f6112-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="f6112-113">description</span><span class="sxs-lookup"><span data-stu-id="f6112-113">description</span></span>|<span data-ttu-id="f6112-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6112-114">String</span></span>|<span data-ttu-id="f6112-115">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f6112-115">The app's description.</span></span> <span data-ttu-id="f6112-116">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f6112-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="f6112-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="f6112-117">publisherName</span></span>|<span data-ttu-id="f6112-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6112-118">String</span></span>|<span data-ttu-id="f6112-119">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="f6112-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="f6112-120">productName</span><span class="sxs-lookup"><span data-stu-id="f6112-120">productName</span></span>|<span data-ttu-id="f6112-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6112-121">String</span></span>|<span data-ttu-id="f6112-122">製品名。</span><span class="sxs-lookup"><span data-stu-id="f6112-122">The product name.</span></span> <span data-ttu-id="f6112-123">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f6112-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="f6112-124">denied</span><span class="sxs-lookup"><span data-stu-id="f6112-124">denied</span></span>|<span data-ttu-id="f6112-125">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="f6112-125">Boolean</span></span>|<span data-ttu-id="f6112-126">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="f6112-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="f6112-127">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f6112-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6112-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f6112-128">Relationships</span></span>
<span data-ttu-id="f6112-129">なし</span><span class="sxs-lookup"><span data-stu-id="f6112-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6112-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6112-130">JSON Representation</span></span>
<span data-ttu-id="f6112-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f6112-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



