# <a name="omasetting-resource-type"></a><span data-ttu-id="4b29f-101">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b29f-101">omaSetting resource type</span></span>

> <span data-ttu-id="4b29f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b29f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b29f-103">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="4b29f-103">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="4b29f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b29f-104">Properties</span></span>
|<span data-ttu-id="4b29f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b29f-105">Property</span></span>|<span data-ttu-id="4b29f-106">型</span><span class="sxs-lookup"><span data-stu-id="4b29f-106">Type</span></span>|<span data-ttu-id="4b29f-107">説明</span><span class="sxs-lookup"><span data-stu-id="4b29f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b29f-108">displayName</span><span class="sxs-lookup"><span data-stu-id="4b29f-108">displayName</span></span>|<span data-ttu-id="4b29f-109">文字列</span><span class="sxs-lookup"><span data-stu-id="4b29f-109">String</span></span>|<span data-ttu-id="4b29f-110">表示名。</span><span class="sxs-lookup"><span data-stu-id="4b29f-110">Display Name.</span></span>|
|<span data-ttu-id="4b29f-111">説明</span><span class="sxs-lookup"><span data-stu-id="4b29f-111">description</span></span>|<span data-ttu-id="4b29f-112">文字列</span><span class="sxs-lookup"><span data-stu-id="4b29f-112">String</span></span>|<span data-ttu-id="4b29f-113">説明。</span><span class="sxs-lookup"><span data-stu-id="4b29f-113">Description.</span></span>|
|<span data-ttu-id="4b29f-114">omaUri</span><span class="sxs-lookup"><span data-stu-id="4b29f-114">omaUri</span></span>|<span data-ttu-id="4b29f-115">文字列</span><span class="sxs-lookup"><span data-stu-id="4b29f-115">String</span></span>|<span data-ttu-id="4b29f-116">OMA。</span><span class="sxs-lookup"><span data-stu-id="4b29f-116">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b29f-117">関係</span><span class="sxs-lookup"><span data-stu-id="4b29f-117">Relationships</span></span>
<span data-ttu-id="4b29f-118">なし</span><span class="sxs-lookup"><span data-stu-id="4b29f-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b29f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b29f-119">JSON Representation</span></span>
<span data-ttu-id="4b29f-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b29f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



