# <a name="proxieddomain-resource-type"></a><span data-ttu-id="0e818-101">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e818-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="0e818-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e818-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e818-103">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="0e818-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="0e818-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e818-104">Properties</span></span>
|<span data-ttu-id="0e818-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e818-105">Property</span></span>|<span data-ttu-id="0e818-106">型</span><span class="sxs-lookup"><span data-stu-id="0e818-106">Type</span></span>|<span data-ttu-id="0e818-107">説明</span><span class="sxs-lookup"><span data-stu-id="0e818-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e818-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="0e818-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="0e818-109">文字列</span><span class="sxs-lookup"><span data-stu-id="0e818-109">String</span></span>|<span data-ttu-id="0e818-110">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="0e818-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="0e818-111">プロキシ</span><span class="sxs-lookup"><span data-stu-id="0e818-111">proxy</span></span>|<span data-ttu-id="0e818-112">文字列</span><span class="sxs-lookup"><span data-stu-id="0e818-112">String</span></span>|<span data-ttu-id="0e818-113">プロキシ IP</span><span class="sxs-lookup"><span data-stu-id="0e818-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e818-114">関係</span><span class="sxs-lookup"><span data-stu-id="0e818-114">Relationships</span></span>
<span data-ttu-id="0e818-115">なし</span><span class="sxs-lookup"><span data-stu-id="0e818-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e818-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e818-116">JSON Representation</span></span>
<span data-ttu-id="0e818-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e818-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```








