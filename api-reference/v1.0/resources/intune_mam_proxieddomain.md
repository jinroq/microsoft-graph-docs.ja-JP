# <a name="proxieddomain-resource-type"></a><span data-ttu-id="59017-101">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59017-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="59017-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59017-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59017-103">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="59017-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="59017-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59017-104">Properties</span></span>
|<span data-ttu-id="59017-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59017-105">Property</span></span>|<span data-ttu-id="59017-106">型</span><span class="sxs-lookup"><span data-stu-id="59017-106">Type</span></span>|<span data-ttu-id="59017-107">説明</span><span class="sxs-lookup"><span data-stu-id="59017-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59017-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="59017-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="59017-109">文字列</span><span class="sxs-lookup"><span data-stu-id="59017-109">String</span></span>|<span data-ttu-id="59017-110">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="59017-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="59017-111">プロキシ</span><span class="sxs-lookup"><span data-stu-id="59017-111">proxy</span></span>|<span data-ttu-id="59017-112">文字列</span><span class="sxs-lookup"><span data-stu-id="59017-112">String</span></span>|<span data-ttu-id="59017-113">プロキシ IP</span><span class="sxs-lookup"><span data-stu-id="59017-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="59017-114">関係</span><span class="sxs-lookup"><span data-stu-id="59017-114">Relationships</span></span>
<span data-ttu-id="59017-115">なし</span><span class="sxs-lookup"><span data-stu-id="59017-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59017-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59017-116">JSON Representation</span></span>
<span data-ttu-id="59017-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59017-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



