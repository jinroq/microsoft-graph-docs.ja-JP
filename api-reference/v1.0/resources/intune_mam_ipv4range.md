# <a name="ipv4range-resource-type"></a><span data-ttu-id="2f225-101">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f225-101">iPv4Range resource type</span></span>

> <span data-ttu-id="2f225-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2f225-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f225-103">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="2f225-103">IP V4 range</span></span>

<span data-ttu-id="2f225-104">[ipRange](../resources/intune_mam_iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2f225-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2f225-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f225-105">Properties</span></span>
|<span data-ttu-id="2f225-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f225-106">Property</span></span>|<span data-ttu-id="2f225-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="2f225-107">Type</span></span>|<span data-ttu-id="2f225-108">説明</span><span class="sxs-lookup"><span data-stu-id="2f225-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f225-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="2f225-109">lowerAddress</span></span>|<span data-ttu-id="2f225-110">文字列</span><span class="sxs-lookup"><span data-stu-id="2f225-110">String</span></span>|<span data-ttu-id="2f225-111">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="2f225-111">Lower IP Address</span></span>|
|<span data-ttu-id="2f225-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="2f225-112">upperAddress</span></span>|<span data-ttu-id="2f225-113">文字列</span><span class="sxs-lookup"><span data-stu-id="2f225-113">String</span></span>|<span data-ttu-id="2f225-114">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="2f225-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f225-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2f225-115">Relationships</span></span>
<span data-ttu-id="2f225-116">なし</span><span class="sxs-lookup"><span data-stu-id="2f225-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2f225-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f225-117">JSON Representation</span></span>
<span data-ttu-id="2f225-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2f225-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.ipRange",
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



