# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="e6601-101">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6601-101">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="e6601-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6601-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6601-103">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="e6601-103">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="e6601-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6601-104">Properties</span></span>
|<span data-ttu-id="e6601-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6601-105">Property</span></span>|<span data-ttu-id="e6601-106">型</span><span class="sxs-lookup"><span data-stu-id="e6601-106">Type</span></span>|<span data-ttu-id="e6601-107">説明</span><span class="sxs-lookup"><span data-stu-id="e6601-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6601-108">displayName</span><span class="sxs-lookup"><span data-stu-id="e6601-108">displayName</span></span>|<span data-ttu-id="e6601-109">文字列</span><span class="sxs-lookup"><span data-stu-id="e6601-109">String</span></span>|<span data-ttu-id="e6601-110">表示名</span><span class="sxs-lookup"><span data-stu-id="e6601-110">Display name</span></span>|
|<span data-ttu-id="e6601-111">範囲</span><span class="sxs-lookup"><span data-stu-id="e6601-111">ranges</span></span>|<span data-ttu-id="e6601-112">[ipRange](../resources/intune_mam_iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6601-112">[ipRange](../resources/intune_mam_iprange.md) collection</span></span>|<span data-ttu-id="e6601-113">IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="e6601-113">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6601-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6601-114">Relationships</span></span>
<span data-ttu-id="e6601-115">なし</span><span class="sxs-lookup"><span data-stu-id="e6601-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6601-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6601-116">JSON Representation</span></span>
<span data-ttu-id="e6601-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6601-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```








