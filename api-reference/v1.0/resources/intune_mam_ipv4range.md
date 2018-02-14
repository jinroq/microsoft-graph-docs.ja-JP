# <a name="ipv4range-resource-type"></a><span data-ttu-id="fadd4-101">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fadd4-101">iPv4Range resource type</span></span>

> <span data-ttu-id="fadd4-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fadd4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fadd4-103">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="fadd4-103">IP V4 range</span></span>

<span data-ttu-id="fadd4-104">[ipRange](../resources/intune_mam_iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="fadd4-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fadd4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fadd4-105">Properties</span></span>
|<span data-ttu-id="fadd4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fadd4-106">Property</span></span>|<span data-ttu-id="fadd4-107">型</span><span class="sxs-lookup"><span data-stu-id="fadd4-107">Type</span></span>|<span data-ttu-id="fadd4-108">説明</span><span class="sxs-lookup"><span data-stu-id="fadd4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fadd4-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="fadd4-109">lowerAddress</span></span>|<span data-ttu-id="fadd4-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fadd4-110">String</span></span>|<span data-ttu-id="fadd4-111">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="fadd4-111">Lower IP Address</span></span>|
|<span data-ttu-id="fadd4-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="fadd4-112">upperAddress</span></span>|<span data-ttu-id="fadd4-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fadd4-113">String</span></span>|<span data-ttu-id="fadd4-114">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="fadd4-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="fadd4-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fadd4-115">Relationships</span></span>
<span data-ttu-id="fadd4-116">なし</span><span class="sxs-lookup"><span data-stu-id="fadd4-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fadd4-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fadd4-117">JSON Representation</span></span>
<span data-ttu-id="fadd4-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fadd4-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



