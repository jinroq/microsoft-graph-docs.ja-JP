# <a name="ipv6range-resource-type"></a><span data-ttu-id="58465-101">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58465-101">iPv6Range resource type</span></span>

> <span data-ttu-id="58465-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="58465-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58465-103">IP V6 の範囲</span><span class="sxs-lookup"><span data-stu-id="58465-103">IP V6 range</span></span>

<span data-ttu-id="58465-104">[ipRange](../resources/intune_mam_iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="58465-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58465-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58465-105">Properties</span></span>
|<span data-ttu-id="58465-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58465-106">Property</span></span>|<span data-ttu-id="58465-107">型</span><span class="sxs-lookup"><span data-stu-id="58465-107">Type</span></span>|<span data-ttu-id="58465-108">説明</span><span class="sxs-lookup"><span data-stu-id="58465-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58465-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="58465-109">lowerAddress</span></span>|<span data-ttu-id="58465-110">文字列</span><span class="sxs-lookup"><span data-stu-id="58465-110">String</span></span>|<span data-ttu-id="58465-111">低位 IP アドレス</span><span class="sxs-lookup"><span data-stu-id="58465-111">Lower IP Address</span></span>|
|<span data-ttu-id="58465-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="58465-112">upperAddress</span></span>|<span data-ttu-id="58465-113">文字列</span><span class="sxs-lookup"><span data-stu-id="58465-113">String</span></span>|<span data-ttu-id="58465-114">高位 IP アドレス</span><span class="sxs-lookup"><span data-stu-id="58465-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="58465-115">関係</span><span class="sxs-lookup"><span data-stu-id="58465-115">Relationships</span></span>
<span data-ttu-id="58465-116">なし</span><span class="sxs-lookup"><span data-stu-id="58465-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="58465-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58465-117">JSON Representation</span></span>
<span data-ttu-id="58465-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58465-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



