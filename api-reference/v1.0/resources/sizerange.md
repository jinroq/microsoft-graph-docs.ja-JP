# <a name="sizerange-resource-type"></a><span data-ttu-id="74f66-101">sizeRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="74f66-101">sizeRange resource type</span></span>


<span data-ttu-id="74f66-102">条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。</span><span class="sxs-lookup"><span data-stu-id="74f66-102">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="74f66-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74f66-103">Properties</span></span>
| <span data-ttu-id="74f66-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74f66-104">Property</span></span>     | <span data-ttu-id="74f66-105">型</span><span class="sxs-lookup"><span data-stu-id="74f66-105">Type</span></span>   |<span data-ttu-id="74f66-106">説明</span><span class="sxs-lookup"><span data-stu-id="74f66-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74f66-107">maximumSize</span><span class="sxs-lookup"><span data-stu-id="74f66-107">MaximumSize</span></span> | <span data-ttu-id="74f66-108">Int32</span><span class="sxs-lookup"><span data-stu-id="74f66-108">Int32</span></span> | <span data-ttu-id="74f66-109">条件または例外を適用するために、受信メッセージに想定される最大サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="74f66-109">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="74f66-110">minimumSize</span><span class="sxs-lookup"><span data-stu-id="74f66-110">MinimumSize</span></span> | <span data-ttu-id="74f66-111">Int32</span><span class="sxs-lookup"><span data-stu-id="74f66-111">Int32</span></span> | <span data-ttu-id="74f66-112">条件または例外を適用するために、受信メッセージに想定される最小サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="74f66-112">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="74f66-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74f66-113">JSON representation</span></span>
<span data-ttu-id="74f66-114">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="74f66-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->