# <a name="mimecontent-resource-type"></a><span data-ttu-id="924aa-101">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="924aa-101">mimeContent resource type</span></span>

> <span data-ttu-id="924aa-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="924aa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="924aa-103">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="924aa-103">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="924aa-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="924aa-104">Properties</span></span>
|<span data-ttu-id="924aa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="924aa-105">Property</span></span>|<span data-ttu-id="924aa-106">型</span><span class="sxs-lookup"><span data-stu-id="924aa-106">Type</span></span>|<span data-ttu-id="924aa-107">説明</span><span class="sxs-lookup"><span data-stu-id="924aa-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="924aa-108">type</span><span class="sxs-lookup"><span data-stu-id="924aa-108">type</span></span>|<span data-ttu-id="924aa-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="924aa-109">String</span></span>|<span data-ttu-id="924aa-110">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="924aa-110">Indicates the content mime type.</span></span>|
|<span data-ttu-id="924aa-111">value</span><span class="sxs-lookup"><span data-stu-id="924aa-111">value</span></span>|<span data-ttu-id="924aa-112">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="924aa-112">Binary</span></span>|<span data-ttu-id="924aa-113">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="924aa-113">A byte array that contains the file content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="924aa-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="924aa-114">Relationships</span></span>
<span data-ttu-id="924aa-115">なし</span><span class="sxs-lookup"><span data-stu-id="924aa-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="924aa-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="924aa-116">JSON Representation</span></span>
<span data-ttu-id="924aa-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="924aa-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



