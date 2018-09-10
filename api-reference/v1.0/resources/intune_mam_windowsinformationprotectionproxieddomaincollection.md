# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="73d6c-101">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73d6c-101">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="73d6c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="73d6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73d6c-103">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="73d6c-103">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="73d6c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73d6c-104">Properties</span></span>
|<span data-ttu-id="73d6c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73d6c-105">Property</span></span>|<span data-ttu-id="73d6c-106">型</span><span class="sxs-lookup"><span data-stu-id="73d6c-106">Type</span></span>|<span data-ttu-id="73d6c-107">説明</span><span class="sxs-lookup"><span data-stu-id="73d6c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73d6c-108">displayName</span><span class="sxs-lookup"><span data-stu-id="73d6c-108">displayName</span></span>|<span data-ttu-id="73d6c-109">文字列</span><span class="sxs-lookup"><span data-stu-id="73d6c-109">String</span></span>|<span data-ttu-id="73d6c-110">表示名</span><span class="sxs-lookup"><span data-stu-id="73d6c-110">Display name</span></span>|
|<span data-ttu-id="73d6c-111">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="73d6c-111">proxiedDomains</span></span>|<span data-ttu-id="73d6c-112">[proxiedDomain](../resources/intune_mam_proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="73d6c-112">[proxiedDomain](../resources/intune_mam_proxieddomain.md) collection</span></span>|<span data-ttu-id="73d6c-113">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="73d6c-113">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="73d6c-114">関係</span><span class="sxs-lookup"><span data-stu-id="73d6c-114">Relationships</span></span>
<span data-ttu-id="73d6c-115">なし</span><span class="sxs-lookup"><span data-stu-id="73d6c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73d6c-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73d6c-116">JSON Representation</span></span>
<span data-ttu-id="73d6c-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="73d6c-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```








