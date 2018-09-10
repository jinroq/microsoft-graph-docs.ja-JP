# <a name="windowsdeviceadaccount-resource-type"></a><span data-ttu-id="f4935-101">windowsDeviceADAccount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4935-101">windowsDeviceADAccount resource type</span></span>

> <span data-ttu-id="f4935-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4935-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4935-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f4935-103">Not yet documented</span></span>

<span data-ttu-id="f4935-104">[windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f4935-104">Inherits from [windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f4935-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4935-105">Properties</span></span>
|<span data-ttu-id="f4935-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4935-106">Property</span></span>|<span data-ttu-id="f4935-107">型</span><span class="sxs-lookup"><span data-stu-id="f4935-107">Type</span></span>|<span data-ttu-id="f4935-108">説明</span><span class="sxs-lookup"><span data-stu-id="f4935-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4935-109">password</span><span class="sxs-lookup"><span data-stu-id="f4935-109">password</span></span>|<span data-ttu-id="f4935-110">文字列</span><span class="sxs-lookup"><span data-stu-id="f4935-110">String</span></span>|<span data-ttu-id="f4935-111">まだ文書化されていない。[windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f4935-111">Not yet documented Inherited from [windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)</span></span>|
|<span data-ttu-id="f4935-112">domainName</span><span class="sxs-lookup"><span data-stu-id="f4935-112">domainName</span></span>|<span data-ttu-id="f4935-113">String</span><span class="sxs-lookup"><span data-stu-id="f4935-113">String</span></span>|<span data-ttu-id="f4935-114">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f4935-114">Not yet documented</span></span>|
|<span data-ttu-id="f4935-115">userName</span><span class="sxs-lookup"><span data-stu-id="f4935-115">userName</span></span>|<span data-ttu-id="f4935-116">文字列</span><span class="sxs-lookup"><span data-stu-id="f4935-116">String</span></span>|<span data-ttu-id="f4935-117">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f4935-117">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4935-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f4935-118">Relationships</span></span>
<span data-ttu-id="f4935-119">なし</span><span class="sxs-lookup"><span data-stu-id="f4935-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f4935-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4935-120">JSON Representation</span></span>
<span data-ttu-id="f4935-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f4935-121">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceADAccount"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceADAccount",
  "password": "String",
  "domainName": "String",
  "userName": "String"
}
```








