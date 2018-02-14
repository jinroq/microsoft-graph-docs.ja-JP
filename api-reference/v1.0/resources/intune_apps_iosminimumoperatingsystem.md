# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="955f4-101">iosMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="955f4-101">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="955f4-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="955f4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="955f4-103">iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="955f4-103">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="955f4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="955f4-104">Properties</span></span>
|<span data-ttu-id="955f4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="955f4-105">Property</span></span>|<span data-ttu-id="955f4-106">型</span><span class="sxs-lookup"><span data-stu-id="955f4-106">Type</span></span>|<span data-ttu-id="955f4-107">説明</span><span class="sxs-lookup"><span data-stu-id="955f4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="955f4-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="955f4-108">v8_0</span></span>|<span data-ttu-id="955f4-109">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="955f4-109">Boolean</span></span>|<span data-ttu-id="955f4-110">バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="955f4-110">Version 8.0 or later.</span></span>|
|<span data-ttu-id="955f4-111">v9_0</span><span class="sxs-lookup"><span data-stu-id="955f4-111">v9_0</span></span>|<span data-ttu-id="955f4-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="955f4-112">Boolean</span></span>|<span data-ttu-id="955f4-113">バージョン 9.0 以降。</span><span class="sxs-lookup"><span data-stu-id="955f4-113">Version 9.0 or later.</span></span>|
|<span data-ttu-id="955f4-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="955f4-114">v10_0</span></span>|<span data-ttu-id="955f4-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="955f4-115">Boolean</span></span>|<span data-ttu-id="955f4-116">バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="955f4-116">Version 10.0 or later.</span></span>|
|<span data-ttu-id="955f4-117">v11_0</span><span class="sxs-lookup"><span data-stu-id="955f4-117">v11_0</span></span>|<span data-ttu-id="955f4-118">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="955f4-118">Boolean</span></span>|<span data-ttu-id="955f4-119">バージョン 11.0 以降。</span><span class="sxs-lookup"><span data-stu-id="955f4-119">Version 11.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="955f4-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="955f4-120">Relationships</span></span>
<span data-ttu-id="955f4-121">なし</span><span class="sxs-lookup"><span data-stu-id="955f4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="955f4-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="955f4-122">JSON Representation</span></span>
<span data-ttu-id="955f4-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="955f4-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true
}
```



