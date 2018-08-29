# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="80f26-101">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80f26-101">vppLicensingType resource type</span></span>

> <span data-ttu-id="80f26-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80f26-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80f26-103">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="80f26-103">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="80f26-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80f26-104">Properties</span></span>
|<span data-ttu-id="80f26-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80f26-105">Property</span></span>|<span data-ttu-id="80f26-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="80f26-106">Type</span></span>|<span data-ttu-id="80f26-107">説明</span><span class="sxs-lookup"><span data-stu-id="80f26-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80f26-108">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="80f26-108">supportsUserLicensing</span></span>|<span data-ttu-id="80f26-109">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="80f26-109">Boolean</span></span>|<span data-ttu-id="80f26-110">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="80f26-110">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="80f26-111">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="80f26-111">supportsDeviceLicensing</span></span>|<span data-ttu-id="80f26-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="80f26-112">Boolean</span></span>|<span data-ttu-id="80f26-113">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="80f26-113">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80f26-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="80f26-114">Relationships</span></span>
<span data-ttu-id="80f26-115">なし</span><span class="sxs-lookup"><span data-stu-id="80f26-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80f26-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80f26-116">JSON Representation</span></span>
<span data-ttu-id="80f26-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80f26-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



