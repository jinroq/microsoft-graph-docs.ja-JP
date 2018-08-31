# <a name="sortfield-resource-type"></a><span data-ttu-id="05895-101">SortField リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05895-101">SortField resource type</span></span>

<span data-ttu-id="05895-102">並べ替え操作の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="05895-102">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="05895-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05895-103">Properties</span></span>
| <span data-ttu-id="05895-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05895-104">Property</span></span>     | <span data-ttu-id="05895-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="05895-105">Type</span></span>   |<span data-ttu-id="05895-106">説明</span><span class="sxs-lookup"><span data-stu-id="05895-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05895-107">昇順</span><span class="sxs-lookup"><span data-stu-id="05895-107">ascending</span></span>|<span data-ttu-id="05895-108">ブール値</span><span class="sxs-lookup"><span data-stu-id="05895-108">boolean</span></span>|<span data-ttu-id="05895-109">昇順の方法で並べ替えを行うかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="05895-109">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="05895-110">色</span><span class="sxs-lookup"><span data-stu-id="05895-110">color</span></span>|<span data-ttu-id="05895-111">文字列</span><span class="sxs-lookup"><span data-stu-id="05895-111">string</span></span>|<span data-ttu-id="05895-112">並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。</span><span class="sxs-lookup"><span data-stu-id="05895-112">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="05895-113">dataOption</span><span class="sxs-lookup"><span data-stu-id="05895-113">dataOption</span></span>|<span data-ttu-id="05895-114">文字列</span><span class="sxs-lookup"><span data-stu-id="05895-114">string</span></span>|<span data-ttu-id="05895-115">このフィールドの他の並べ替えオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="05895-115">Represents additional sorting options for this field. Possible values are: , .</span></span> <span data-ttu-id="05895-116">指定できる値は、`Normal`、`TextAsNumber` です。</span><span class="sxs-lookup"><span data-stu-id="05895-116">The possible values are:</span></span>|
|<span data-ttu-id="05895-117">鍵</span><span class="sxs-lookup"><span data-stu-id="05895-117">key</span></span>|<span data-ttu-id="05895-118">int</span><span class="sxs-lookup"><span data-stu-id="05895-118">int</span></span>|<span data-ttu-id="05895-p102">条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。</span><span class="sxs-lookup"><span data-stu-id="05895-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="05895-121">sortOn</span><span class="sxs-lookup"><span data-stu-id="05895-121">sortOn</span></span>|<span data-ttu-id="05895-122">文字列</span><span class="sxs-lookup"><span data-stu-id="05895-122">string</span></span>|<span data-ttu-id="05895-123">この条件の並べ替えの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="05895-123">Represents the type of sorting of this condition. Possible values are: , , , .</span></span> <span data-ttu-id="05895-124">可能な値は、`Value`、`CellColor`、`FontColor`、`Icon` です。</span><span class="sxs-lookup"><span data-stu-id="05895-124">The possible values are `Value`, `CellColor`, `FontColor`, `Icon`, , , , , , , , or .</span></span>|
|<span data-ttu-id="05895-125">アイコン</span><span class="sxs-lookup"><span data-stu-id="05895-125">icon</span></span>|[<span data-ttu-id="05895-126">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="05895-126">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="05895-127">並べ替えがセルのアイコンで行われるときに条件の対象となるアイコンを表します。</span><span class="sxs-lookup"><span data-stu-id="05895-127">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05895-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05895-128">JSON representation</span></span>

<span data-ttu-id="05895-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05895-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->