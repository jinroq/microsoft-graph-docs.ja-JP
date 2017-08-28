# <a name="nameditem-resource-type"></a><span data-ttu-id="bf018-101">NamedItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf018-101">NamedItem resource type</span></span>

<span data-ttu-id="bf018-p101">セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="bf018-p101">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="bf018-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf018-105">Methods</span></span>

| <span data-ttu-id="bf018-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf018-106">Method</span></span>           | <span data-ttu-id="bf018-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bf018-107">Return Type</span></span>    |<span data-ttu-id="bf018-108">説明</span><span class="sxs-lookup"><span data-stu-id="bf018-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf018-109">追加</span><span class="sxs-lookup"><span data-stu-id="bf018-109">Add</span></span>](../api/nameditem_add.md)|[<span data-ttu-id="bf018-110">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bf018-110">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="bf018-111">新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="bf018-111">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="bf018-112">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="bf018-112">AddFormulaLocal</span></span>](../api/nameditem_addformulalocal.md)|[<span data-ttu-id="bf018-113">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bf018-113">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="bf018-114">ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="bf018-114">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="bf018-115">NamedItem を取得する</span><span class="sxs-lookup"><span data-stu-id="bf018-115">Get NamedItem</span></span>](../api/nameditem_get.md) | [<span data-ttu-id="bf018-116">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bf018-116">NamedItem</span></span>](nameditem.md) |<span data-ttu-id="bf018-117">namedItem オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bf018-117">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="bf018-118">Update</span><span class="sxs-lookup"><span data-stu-id="bf018-118">Update</span></span>](../api/nameditem_update.md) | [<span data-ttu-id="bf018-119">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bf018-119">NamedItem</span></span>](nameditem.md)   |<span data-ttu-id="bf018-120">NamedItem オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bf018-120">Update NamedItem object.</span></span> |
|[<span data-ttu-id="bf018-121">Range</span><span class="sxs-lookup"><span data-stu-id="bf018-121">Range</span></span>](../api/nameditem_range.md)|[<span data-ttu-id="bf018-122">Range</span><span class="sxs-lookup"><span data-stu-id="bf018-122">Range</span></span>](range.md)|<span data-ttu-id="bf018-p102">名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。</span><span class="sxs-lookup"><span data-stu-id="bf018-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="bf018-125">List</span><span class="sxs-lookup"><span data-stu-id="bf018-125">List</span></span>](../api/nameditem_list.md) | <span data-ttu-id="bf018-126">[NamedItem](nameditem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bf018-126">[NamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="bf018-127">namedItem オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="bf018-127">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="bf018-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf018-128">Properties</span></span>
| <span data-ttu-id="bf018-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf018-129">Property</span></span>     | <span data-ttu-id="bf018-130">型</span><span class="sxs-lookup"><span data-stu-id="bf018-130">Type</span></span>   |<span data-ttu-id="bf018-131">説明</span><span class="sxs-lookup"><span data-stu-id="bf018-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf018-132">name</span><span class="sxs-lookup"><span data-stu-id="bf018-132">name</span></span>|<span data-ttu-id="bf018-133">string</span><span class="sxs-lookup"><span data-stu-id="bf018-133">string</span></span>|<span data-ttu-id="bf018-p103">オブジェクトの名前。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bf018-p103">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="bf018-136">comment</span><span class="sxs-lookup"><span data-stu-id="bf018-136">comment</span></span>|<span data-ttu-id="bf018-137">string</span><span class="sxs-lookup"><span data-stu-id="bf018-137">string</span></span>|<span data-ttu-id="bf018-138">この名前に関連付けられているコメントを表します。</span><span class="sxs-lookup"><span data-stu-id="bf018-138">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="bf018-139">scope</span><span class="sxs-lookup"><span data-stu-id="bf018-139">scope</span></span>|<span data-ttu-id="bf018-140">string</span><span class="sxs-lookup"><span data-stu-id="bf018-140">string</span></span>|<span data-ttu-id="bf018-p104">名前がブックを対象にしているのか、特定のワークシートを対象にしているのかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bf018-p104">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="bf018-143">type</span><span class="sxs-lookup"><span data-stu-id="bf018-143">type</span></span>|<span data-ttu-id="bf018-144">string</span><span class="sxs-lookup"><span data-stu-id="bf018-144">string</span></span>|<span data-ttu-id="bf018-p105">名前に関連付けられている参照の型を示します。可能な値は、`String`、`Integer`、`Double`、`Boolean`、`Range` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bf018-p105">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="bf018-148">value</span><span class="sxs-lookup"><span data-stu-id="bf018-148">value</span></span>|<span data-ttu-id="bf018-149">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="bf018-149">object</span></span>|<span data-ttu-id="bf018-p106">定義されている名前が参照する数式を表します。例: =Sheet14!$B$2:$H$12、=4.75, など。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bf018-p106">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="bf018-153">visible</span><span class="sxs-lookup"><span data-stu-id="bf018-153">visible</span></span>|<span data-ttu-id="bf018-154">boolean</span><span class="sxs-lookup"><span data-stu-id="bf018-154">boolean</span></span>|<span data-ttu-id="bf018-155">オブジェクトを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bf018-155">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf018-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf018-156">Relationships</span></span>
| <span data-ttu-id="bf018-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf018-157">Relationship</span></span>     | <span data-ttu-id="bf018-158">型</span><span class="sxs-lookup"><span data-stu-id="bf018-158">Type</span></span>   |<span data-ttu-id="bf018-159">説明</span><span class="sxs-lookup"><span data-stu-id="bf018-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf018-160">ワークシート</span><span class="sxs-lookup"><span data-stu-id="bf018-160">worksheet</span></span>|[<span data-ttu-id="bf018-161">worksheet</span><span class="sxs-lookup"><span data-stu-id="bf018-161">worksheet</span></span>](worksheet.md)|<span data-ttu-id="bf018-p107">名前付きのアイテムの対象になるワークシートを返します。アイテムの対象がワークシートの場合にのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bf018-p107">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf018-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf018-165">JSON representation</span></span>

<span data-ttu-id="bf018-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf018-166">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.range"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
