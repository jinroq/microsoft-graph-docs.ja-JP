# <a name="windowsdeviceadaccount-resource-type"></a><span data-ttu-id="ebc0c-101">windowsDeviceADAccount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebc0c-101">windowsDeviceADAccount resource type</span></span>

> <span data-ttu-id="ebc0c-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ebc0c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebc0c-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebc0c-103">Not yet documented</span></span>

<span data-ttu-id="ebc0c-104">[windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ebc0c-104">Inherits from [windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ebc0c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebc0c-105">Properties</span></span>
|<span data-ttu-id="ebc0c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebc0c-106">Property</span></span>|<span data-ttu-id="ebc0c-107">型</span><span class="sxs-lookup"><span data-stu-id="ebc0c-107">Type</span></span>|<span data-ttu-id="ebc0c-108">説明</span><span class="sxs-lookup"><span data-stu-id="ebc0c-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebc0c-109">password</span><span class="sxs-lookup"><span data-stu-id="ebc0c-109">password</span></span>|<span data-ttu-id="ebc0c-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ebc0c-110">String</span></span>|<span data-ttu-id="ebc0c-111">まだ文書化されていない。[windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ebc0c-111">Not yet documented Inherited from [windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)</span></span>|
|<span data-ttu-id="ebc0c-112">domainName</span><span class="sxs-lookup"><span data-stu-id="ebc0c-112">domainName</span></span>|<span data-ttu-id="ebc0c-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ebc0c-113">String</span></span>|<span data-ttu-id="ebc0c-114">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebc0c-114">Not yet documented</span></span>|
|<span data-ttu-id="ebc0c-115">userName</span><span class="sxs-lookup"><span data-stu-id="ebc0c-115">Username</span></span>|<span data-ttu-id="ebc0c-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ebc0c-116">String</span></span>|<span data-ttu-id="ebc0c-117">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebc0c-117">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebc0c-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ebc0c-118">Relationships</span></span>
<span data-ttu-id="ebc0c-119">なし</span><span class="sxs-lookup"><span data-stu-id="ebc0c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebc0c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebc0c-120">JSON Representation</span></span>
<span data-ttu-id="ebc0c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ebc0c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDeviceADAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceADAccount",
  "password": "String",
  "domainName": "String",
  "userName": "String"
}
```



