# <a name="resourceaction-resource-type"></a><span data-ttu-id="c7054-101">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7054-101">resourceAction resource type</span></span>

> <span data-ttu-id="c7054-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7054-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7054-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c7054-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c7054-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7054-104">Properties</span></span>
|<span data-ttu-id="c7054-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7054-105">Property</span></span>|<span data-ttu-id="c7054-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="c7054-106">Type</span></span>|<span data-ttu-id="c7054-107">説明</span><span class="sxs-lookup"><span data-stu-id="c7054-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7054-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c7054-108">allowedResourceActions</span></span>|<span data-ttu-id="c7054-109">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c7054-109">String collection</span></span>|<span data-ttu-id="c7054-110">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="c7054-110">Allowed Actions</span></span>|
|<span data-ttu-id="c7054-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c7054-111">notAllowedResourceActions</span></span>|<span data-ttu-id="c7054-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c7054-112">String collection</span></span>|<span data-ttu-id="c7054-113">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="c7054-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7054-114">関係</span><span class="sxs-lookup"><span data-stu-id="c7054-114">Relationships</span></span>
<span data-ttu-id="c7054-115">なし</span><span class="sxs-lookup"><span data-stu-id="c7054-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7054-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7054-116">JSON Representation</span></span>
<span data-ttu-id="c7054-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7054-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



