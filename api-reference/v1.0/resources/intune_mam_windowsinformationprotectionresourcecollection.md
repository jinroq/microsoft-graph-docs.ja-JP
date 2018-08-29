# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="7dab8-101">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7dab8-101">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="7dab8-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7dab8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7dab8-103">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="7dab8-103">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="7dab8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dab8-104">Properties</span></span>
|<span data-ttu-id="7dab8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dab8-105">Property</span></span>|<span data-ttu-id="7dab8-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="7dab8-106">Type</span></span>|<span data-ttu-id="7dab8-107">説明</span><span class="sxs-lookup"><span data-stu-id="7dab8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dab8-108">displayName</span><span class="sxs-lookup"><span data-stu-id="7dab8-108">displayName</span></span>|<span data-ttu-id="7dab8-109">文字列</span><span class="sxs-lookup"><span data-stu-id="7dab8-109">String</span></span>|<span data-ttu-id="7dab8-110">表示名</span><span class="sxs-lookup"><span data-stu-id="7dab8-110">Display name</span></span>|
|<span data-ttu-id="7dab8-111">リソース</span><span class="sxs-lookup"><span data-stu-id="7dab8-111">resources</span></span>|<span data-ttu-id="7dab8-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7dab8-112">String collection</span></span>|<span data-ttu-id="7dab8-113">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="7dab8-113">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dab8-114">関係</span><span class="sxs-lookup"><span data-stu-id="7dab8-114">Relationships</span></span>
<span data-ttu-id="7dab8-115">なし</span><span class="sxs-lookup"><span data-stu-id="7dab8-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7dab8-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7dab8-116">JSON Representation</span></span>
<span data-ttu-id="7dab8-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7dab8-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



