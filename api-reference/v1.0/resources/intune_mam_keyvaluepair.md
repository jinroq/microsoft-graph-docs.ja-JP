# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="cc4b5-101">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc4b5-101">keyValuePair resource type</span></span>

> <span data-ttu-id="cc4b5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc4b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc4b5-103">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="cc4b5-103">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="cc4b5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc4b5-104">Properties</span></span>
|<span data-ttu-id="cc4b5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc4b5-105">Property</span></span>|<span data-ttu-id="cc4b5-106">型</span><span class="sxs-lookup"><span data-stu-id="cc4b5-106">Type</span></span>|<span data-ttu-id="cc4b5-107">説明</span><span class="sxs-lookup"><span data-stu-id="cc4b5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc4b5-108">名前</span><span class="sxs-lookup"><span data-stu-id="cc4b5-108">name</span></span>|<span data-ttu-id="cc4b5-109">文字列</span><span class="sxs-lookup"><span data-stu-id="cc4b5-109">String</span></span>|<span data-ttu-id="cc4b5-110">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="cc4b5-110">Name for this key-value pair</span></span>|
|<span data-ttu-id="cc4b5-111">value</span><span class="sxs-lookup"><span data-stu-id="cc4b5-111">value</span></span>|<span data-ttu-id="cc4b5-112">文字列</span><span class="sxs-lookup"><span data-stu-id="cc4b5-112">String</span></span>|<span data-ttu-id="cc4b5-113">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="cc4b5-113">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc4b5-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc4b5-114">Relationships</span></span>
<span data-ttu-id="cc4b5-115">なし</span><span class="sxs-lookup"><span data-stu-id="cc4b5-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc4b5-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc4b5-116">JSON Representation</span></span>
<span data-ttu-id="cc4b5-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc4b5-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```








