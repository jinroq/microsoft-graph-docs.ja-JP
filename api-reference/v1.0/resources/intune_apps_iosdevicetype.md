# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="24049-101">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24049-101">iosDeviceType resource type</span></span>

> <span data-ttu-id="24049-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24049-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24049-103">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="24049-103">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="24049-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24049-104">Properties</span></span>
|<span data-ttu-id="24049-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24049-105">Property</span></span>|<span data-ttu-id="24049-106">型</span><span class="sxs-lookup"><span data-stu-id="24049-106">Type</span></span>|<span data-ttu-id="24049-107">説明</span><span class="sxs-lookup"><span data-stu-id="24049-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24049-108">iPad</span><span class="sxs-lookup"><span data-stu-id="24049-108">iPad</span></span>|<span data-ttu-id="24049-109">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="24049-109">Boolean</span></span>|<span data-ttu-id="24049-110">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="24049-110">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="24049-111">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="24049-111">iPhoneAndIPod</span></span>|<span data-ttu-id="24049-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="24049-112">Boolean</span></span>|<span data-ttu-id="24049-113">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="24049-113">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24049-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24049-114">Relationships</span></span>
<span data-ttu-id="24049-115">なし</span><span class="sxs-lookup"><span data-stu-id="24049-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24049-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24049-116">JSON Representation</span></span>
<span data-ttu-id="24049-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24049-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



