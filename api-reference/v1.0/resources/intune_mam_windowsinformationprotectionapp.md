# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="cb5a4-101">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb5a4-101">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="cb5a4-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb5a4-103">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="cb5a4-103">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="cb5a4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb5a4-104">Properties</span></span>
|<span data-ttu-id="cb5a4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb5a4-105">Property</span></span>|<span data-ttu-id="cb5a4-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="cb5a4-106">Type</span></span>|<span data-ttu-id="cb5a4-107">説明</span><span class="sxs-lookup"><span data-stu-id="cb5a4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb5a4-108">displayName</span><span class="sxs-lookup"><span data-stu-id="cb5a4-108">displayName</span></span>|<span data-ttu-id="cb5a4-109">文字列</span><span class="sxs-lookup"><span data-stu-id="cb5a4-109">String</span></span>|<span data-ttu-id="cb5a4-110">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-110">App display name.</span></span>|
|<span data-ttu-id="cb5a4-111">説明</span><span class="sxs-lookup"><span data-stu-id="cb5a4-111">description</span></span>|<span data-ttu-id="cb5a4-112">文字列</span><span class="sxs-lookup"><span data-stu-id="cb5a4-112">String</span></span>|<span data-ttu-id="cb5a4-113">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-113">The app's description.</span></span>|
|<span data-ttu-id="cb5a4-114">publisherName</span><span class="sxs-lookup"><span data-stu-id="cb5a4-114">publisherName</span></span>|<span data-ttu-id="cb5a4-115">文字列</span><span class="sxs-lookup"><span data-stu-id="cb5a4-115">String</span></span>|<span data-ttu-id="cb5a4-116">発行元名</span><span class="sxs-lookup"><span data-stu-id="cb5a4-116">The publisher name</span></span>|
|<span data-ttu-id="cb5a4-117">productName</span><span class="sxs-lookup"><span data-stu-id="cb5a4-117">productName</span></span>|<span data-ttu-id="cb5a4-118">文字列</span><span class="sxs-lookup"><span data-stu-id="cb5a4-118">String</span></span>|<span data-ttu-id="cb5a4-119">製品名。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-119">The product name.</span></span>|
|<span data-ttu-id="cb5a4-120">拒否されました</span><span class="sxs-lookup"><span data-stu-id="cb5a4-120">denied</span></span>|<span data-ttu-id="cb5a4-121">ブール型</span><span class="sxs-lookup"><span data-stu-id="cb5a4-121">Boolean</span></span>|<span data-ttu-id="cb5a4-122">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-122">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb5a4-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cb5a4-123">Relationships</span></span>
<span data-ttu-id="cb5a4-124">なし</span><span class="sxs-lookup"><span data-stu-id="cb5a4-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb5a4-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb5a4-125">JSON Representation</span></span>
<span data-ttu-id="cb5a4-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cb5a4-126">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```








