# <a name="location-resource-type"></a><span data-ttu-id="0ac4a-101">場所リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ac4a-101">Location resource type</span></span>

<span data-ttu-id="0ac4a-102">イベントの場所の情報を表します。</span><span class="sxs-lookup"><span data-stu-id="0ac4a-102">Represents location information of an event.</span></span>


## <a name="properties"></a><span data-ttu-id="0ac4a-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ac4a-103">Properties</span></span>
| <span data-ttu-id="0ac4a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ac4a-104">Property</span></span>  | <span data-ttu-id="0ac4a-105">型</span><span class="sxs-lookup"><span data-stu-id="0ac4a-105">Type</span></span>   | <span data-ttu-id="0ac4a-106">説明</span><span class="sxs-lookup"><span data-stu-id="0ac4a-106">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="0ac4a-107">address</span><span class="sxs-lookup"><span data-stu-id="0ac4a-107">address</span></span> | [<span data-ttu-id="0ac4a-108">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="0ac4a-108">physicalAddress</span></span>](physicalAddress.md) |<span data-ttu-id="0ac4a-109">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="0ac4a-109">The street address of the location.</span></span> |
| <span data-ttu-id="0ac4a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac4a-110">displayName</span></span>  | <span data-ttu-id="0ac4a-111">String</span><span class="sxs-lookup"><span data-stu-id="0ac4a-111">String</span></span> | <span data-ttu-id="0ac4a-112">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="0ac4a-112">The name associated with the location.</span></span>                       |
| <span data-ttu-id="0ac4a-113">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0ac4a-113">locationEmailAddress</span></span> | <span data-ttu-id="0ac4a-114">String</span><span class="sxs-lookup"><span data-stu-id="0ac4a-114">String</span></span> | <span data-ttu-id="0ac4a-115">場所の電子メール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="0ac4a-115">Optional email address of the location.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="0ac4a-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ac4a-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```

## <a name="remarks"></a><span data-ttu-id="0ac4a-117">注釈</span><span class="sxs-lookup"><span data-stu-id="0ac4a-117">Remarks</span></span>

<span data-ttu-id="0ac4a-118">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ac4a-118">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->