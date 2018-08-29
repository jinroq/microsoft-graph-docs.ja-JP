# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="91275-101">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91275-101">iosDeviceType resource type</span></span>

> <span data-ttu-id="91275-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="91275-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91275-103">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="91275-103">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="91275-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91275-104">Properties</span></span>
|<span data-ttu-id="91275-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91275-105">Property</span></span>|<span data-ttu-id="91275-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="91275-106">Type</span></span>|<span data-ttu-id="91275-107">説明</span><span class="sxs-lookup"><span data-stu-id="91275-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91275-108">iPad</span><span class="sxs-lookup"><span data-stu-id="91275-108">iPad</span></span>|<span data-ttu-id="91275-109">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="91275-109">Boolean</span></span>|<span data-ttu-id="91275-110">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="91275-110">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="91275-111">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="91275-111">iPhoneAndIPod</span></span>|<span data-ttu-id="91275-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="91275-112">Boolean</span></span>|<span data-ttu-id="91275-113">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="91275-113">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91275-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91275-114">Relationships</span></span>
<span data-ttu-id="91275-115">なし</span><span class="sxs-lookup"><span data-stu-id="91275-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91275-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91275-116">JSON Representation</span></span>
<span data-ttu-id="91275-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91275-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



