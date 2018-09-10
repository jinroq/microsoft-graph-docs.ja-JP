# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="b6b15-101">iosMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b6b15-101">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="b6b15-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6b15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6b15-103">iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b6b15-103">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="b6b15-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6b15-104">Properties</span></span>
|<span data-ttu-id="b6b15-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6b15-105">Property</span></span>|<span data-ttu-id="b6b15-106">型</span><span class="sxs-lookup"><span data-stu-id="b6b15-106">Type</span></span>|<span data-ttu-id="b6b15-107">説明</span><span class="sxs-lookup"><span data-stu-id="b6b15-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6b15-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="b6b15-108">v8_0</span></span>|<span data-ttu-id="b6b15-109">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b6b15-109">Boolean</span></span>|<span data-ttu-id="b6b15-110">バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="b6b15-110">Version 8.0 or later.</span></span>|
|<span data-ttu-id="b6b15-111">v9_0</span><span class="sxs-lookup"><span data-stu-id="b6b15-111">v9_0</span></span>|<span data-ttu-id="b6b15-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b6b15-112">Boolean</span></span>|<span data-ttu-id="b6b15-113">バージョン 9.0 以降。</span><span class="sxs-lookup"><span data-stu-id="b6b15-113">Version 9.0 or later.</span></span>|
|<span data-ttu-id="b6b15-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="b6b15-114">v10_0</span></span>|<span data-ttu-id="b6b15-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b6b15-115">Boolean</span></span>|<span data-ttu-id="b6b15-116">バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="b6b15-116">Version 10.0 or later.</span></span>|
|<span data-ttu-id="b6b15-117">v11_0</span><span class="sxs-lookup"><span data-stu-id="b6b15-117">v11_0</span></span>|<span data-ttu-id="b6b15-118">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b6b15-118">Boolean</span></span>|<span data-ttu-id="b6b15-119">バージョン 11.0 以降。</span><span class="sxs-lookup"><span data-stu-id="b6b15-119">Version 11.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6b15-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b6b15-120">Relationships</span></span>
<span data-ttu-id="b6b15-121">なし</span><span class="sxs-lookup"><span data-stu-id="b6b15-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b6b15-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b6b15-122">JSON Representation</span></span>
<span data-ttu-id="b6b15-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b6b15-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true
}
```








