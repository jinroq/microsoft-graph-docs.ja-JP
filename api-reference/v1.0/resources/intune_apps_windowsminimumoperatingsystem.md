# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="d7ac4-101">windowsMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7ac4-101">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="d7ac4-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7ac4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7ac4-103">Windows モバイル アプリに必要な最小オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="d7ac4-103">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="d7ac4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7ac4-104">Properties</span></span>
|<span data-ttu-id="d7ac4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7ac4-105">Property</span></span>|<span data-ttu-id="d7ac4-106">型</span><span class="sxs-lookup"><span data-stu-id="d7ac4-106">Type</span></span>|<span data-ttu-id="d7ac4-107">説明</span><span class="sxs-lookup"><span data-stu-id="d7ac4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7ac4-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="d7ac4-108">v8_0</span></span>|<span data-ttu-id="d7ac4-109">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="d7ac4-109">Boolean</span></span>|<span data-ttu-id="d7ac4-110">Windows バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="d7ac4-110">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="d7ac4-111">v8_1</span><span class="sxs-lookup"><span data-stu-id="d7ac4-111">v8_1</span></span>|<span data-ttu-id="d7ac4-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="d7ac4-112">Boolean</span></span>|<span data-ttu-id="d7ac4-113">Windows バージョン 8.1 以降。</span><span class="sxs-lookup"><span data-stu-id="d7ac4-113">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="d7ac4-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="d7ac4-114">v10_0</span></span>|<span data-ttu-id="d7ac4-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="d7ac4-115">Boolean</span></span>|<span data-ttu-id="d7ac4-116">Windows バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="d7ac4-116">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7ac4-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7ac4-117">Relationships</span></span>
<span data-ttu-id="d7ac4-118">なし</span><span class="sxs-lookup"><span data-stu-id="d7ac4-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d7ac4-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7ac4-119">JSON Representation</span></span>
<span data-ttu-id="d7ac4-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d7ac4-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



