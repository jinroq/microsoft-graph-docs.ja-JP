# <a name="windowsdeviceazureadaccount-resource-type"></a><span data-ttu-id="44fd2-101">windowsDeviceAzureADAccount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44fd2-101">windowsDeviceAzureADAccount resource type</span></span>

> <span data-ttu-id="44fd2-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="44fd2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44fd2-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="44fd2-103">Not yet documented</span></span>

<span data-ttu-id="44fd2-104">[windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="44fd2-104">Inherits from [windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)</span></span>

## <a name="properties"></a><span data-ttu-id="44fd2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44fd2-105">Properties</span></span>
|<span data-ttu-id="44fd2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44fd2-106">Property</span></span>|<span data-ttu-id="44fd2-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="44fd2-107">Type</span></span>|<span data-ttu-id="44fd2-108">説明</span><span class="sxs-lookup"><span data-stu-id="44fd2-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44fd2-109">password</span><span class="sxs-lookup"><span data-stu-id="44fd2-109">password</span></span>|<span data-ttu-id="44fd2-110">文字列</span><span class="sxs-lookup"><span data-stu-id="44fd2-110">String</span></span>|<span data-ttu-id="44fd2-111">まだ文書化されていない、[windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="44fd2-111">Not yet documented Inherited from [windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)</span></span>|
|<span data-ttu-id="44fd2-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44fd2-112">userPrincipalName</span></span>|<span data-ttu-id="44fd2-113">文字列</span><span class="sxs-lookup"><span data-stu-id="44fd2-113">String</span></span>|<span data-ttu-id="44fd2-114">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="44fd2-114">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="44fd2-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="44fd2-115">Relationships</span></span>
<span data-ttu-id="44fd2-116">なし</span><span class="sxs-lookup"><span data-stu-id="44fd2-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44fd2-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44fd2-117">JSON Representation</span></span>
<span data-ttu-id="44fd2-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="44fd2-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsDeviceAccount",
  "@odata.type": "microsoft.graph.windowsDeviceAzureADAccount"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceAzureADAccount",
  "password": "String",
  "userPrincipalName": "String"
}
```



