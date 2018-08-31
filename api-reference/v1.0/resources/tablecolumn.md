# <a name="tablecolumn-resource-type"></a><span data-ttu-id="b2415-101">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2415-101">TableColumn resource type</span></span>

<span data-ttu-id="b2415-102">テーブル内にある 1 つの列を表します。</span><span class="sxs-lookup"><span data-stu-id="b2415-102">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="b2415-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="b2415-103">Methods</span></span>

| <span data-ttu-id="b2415-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="b2415-104">Method</span></span>           | <span data-ttu-id="b2415-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b2415-105">Return Type</span></span>    |<span data-ttu-id="b2415-106">説明</span><span class="sxs-lookup"><span data-stu-id="b2415-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2415-107">TableColumn を取得する</span><span class="sxs-lookup"><span data-stu-id="b2415-107">Get TableColumn</span></span>](../api/tablecolumn_get.md) | [<span data-ttu-id="b2415-108">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="b2415-108">WorkbookTableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="b2415-109">tableColumn オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b2415-109">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="b2415-110">更新する</span><span class="sxs-lookup"><span data-stu-id="b2415-110">Update</span></span>](../api/tablecolumn_update.md) | [<span data-ttu-id="b2415-111">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="b2415-111">WorkbookTableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="b2415-112">TableColumn オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b2415-112">Update TableColumn object.</span></span> |
|[<span data-ttu-id="b2415-113">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="b2415-113">Databodyrange</span></span>](../api/tablecolumn_databodyrange.md)|[<span data-ttu-id="b2415-114">範囲</span><span class="sxs-lookup"><span data-stu-id="b2415-114">Range</span></span>](range.md)|<span data-ttu-id="b2415-115">列のデータ本体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2415-115">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="b2415-116">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="b2415-116">Headerrowrange</span></span>](../api/tablecolumn_headerrowrange.md)|[<span data-ttu-id="b2415-117">範囲</span><span class="sxs-lookup"><span data-stu-id="b2415-117">Range</span></span>](range.md)|<span data-ttu-id="b2415-118">列のヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2415-118">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="b2415-119">範囲</span><span class="sxs-lookup"><span data-stu-id="b2415-119">Range</span></span>](../api/tablecolumn_range.md)|[<span data-ttu-id="b2415-120">範囲</span><span class="sxs-lookup"><span data-stu-id="b2415-120">Range</span></span>](range.md)|<span data-ttu-id="b2415-121">列全体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2415-121">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="b2415-122">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="b2415-122">Totalrowrange</span></span>](../api/tablecolumn_totalrowrange.md)|[<span data-ttu-id="b2415-123">範囲</span><span class="sxs-lookup"><span data-stu-id="b2415-123">Range</span></span>](range.md)|<span data-ttu-id="b2415-124">列の集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2415-124">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="b2415-125">削除する</span><span class="sxs-lookup"><span data-stu-id="b2415-125">Delete</span></span>](../api/tablecolumn_delete.md)|<span data-ttu-id="b2415-126">なし</span><span class="sxs-lookup"><span data-stu-id="b2415-126">None</span></span>|<span data-ttu-id="b2415-127">テーブルから列を削除します。</span><span class="sxs-lookup"><span data-stu-id="b2415-127">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="b2415-128">リスト</span><span class="sxs-lookup"><span data-stu-id="b2415-128">List</span></span>](../api/tablecolumn_list.md) | <span data-ttu-id="b2415-129">[WorkbookTableColumn](tablecolumn.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b2415-129">[WorkbookTableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="b2415-130">tableColumn オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2415-130">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="b2415-131">Itemat</span><span class="sxs-lookup"><span data-stu-id="b2415-131">Itemat</span></span>](../api/tablecolumncollection_itemat.md)|[<span data-ttu-id="b2415-132">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="b2415-132">WorkbookTableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="b2415-133">コレクション内の位置に基づいて列を取得します。</span><span class="sxs-lookup"><span data-stu-id="b2415-133">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="b2415-134">追加する</span><span class="sxs-lookup"><span data-stu-id="b2415-134">Add</span></span>](../api/tablecolumncollection_add.md)|[<span data-ttu-id="b2415-135">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="b2415-135">WorkbookTableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="b2415-136">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="b2415-136">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2415-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2415-137">Properties</span></span>
| <span data-ttu-id="b2415-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2415-138">Property</span></span>     | <span data-ttu-id="b2415-139">タイプ</span><span class="sxs-lookup"><span data-stu-id="b2415-139">Type</span></span>   |<span data-ttu-id="b2415-140">説明</span><span class="sxs-lookup"><span data-stu-id="b2415-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2415-141">ID</span><span class="sxs-lookup"><span data-stu-id="b2415-141">id</span></span>|<span data-ttu-id="b2415-142">文字列</span><span class="sxs-lookup"><span data-stu-id="b2415-142">string</span></span>|<span data-ttu-id="b2415-143">テーブル内の列を識別する一意のキーを返します。</span><span class="sxs-lookup"><span data-stu-id="b2415-143">Returns a unique key that identifies the column within the table.</span></span> <span data-ttu-id="b2415-144">このプロパティは符号化文字列値として解釈し、その他の型に解析すべきではありません。</span><span class="sxs-lookup"><span data-stu-id="b2415-144">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="b2415-145">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b2415-145">Read-only.</span></span>|
|<span data-ttu-id="b2415-146">インデックス</span><span class="sxs-lookup"><span data-stu-id="b2415-146">index</span></span>|<span data-ttu-id="b2415-147">int</span><span class="sxs-lookup"><span data-stu-id="b2415-147">int</span></span>|<span data-ttu-id="b2415-p102">テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2415-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="b2415-151">名前</span><span class="sxs-lookup"><span data-stu-id="b2415-151">name</span></span>|<span data-ttu-id="b2415-152">文字列</span><span class="sxs-lookup"><span data-stu-id="b2415-152">string</span></span>|<span data-ttu-id="b2415-p103">テーブル列の名前を取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2415-p103">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="b2415-155">値</span><span class="sxs-lookup"><span data-stu-id="b2415-155">values</span></span>|<span data-ttu-id="b2415-156">Json</span><span class="sxs-lookup"><span data-stu-id="b2415-156">Json</span></span>|<span data-ttu-id="b2415-p104">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="b2415-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2415-160">関係</span><span class="sxs-lookup"><span data-stu-id="b2415-160">Relationships</span></span>
| <span data-ttu-id="b2415-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2415-161">Relationship</span></span> | <span data-ttu-id="b2415-162">型</span><span class="sxs-lookup"><span data-stu-id="b2415-162">Type</span></span>   |<span data-ttu-id="b2415-163">説明</span><span class="sxs-lookup"><span data-stu-id="b2415-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2415-164">フィルター</span><span class="sxs-lookup"><span data-stu-id="b2415-164">filter</span></span>|[<span data-ttu-id="b2415-165">WorkbookFilter</span><span class="sxs-lookup"><span data-stu-id="b2415-165">WorkbookFilter</span></span>](filter.md)|<span data-ttu-id="b2415-p105">列に適用されるフィルターを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2415-p105">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2415-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2415-168">JSON representation</span></span>

<span data-ttu-id="b2415-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2415-169">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
