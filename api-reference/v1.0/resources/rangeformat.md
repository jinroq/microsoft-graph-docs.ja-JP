# <a name="rangeformat-resource-type"></a><span data-ttu-id="8cedc-101">RangeFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cedc-101">RangeFormat resource type</span></span>

<span data-ttu-id="8cedc-102">範囲のフォント、塗りつぶし、境界線、配置などのプロパティをカプセル化する、書式設定オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8cedc-102">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="8cedc-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="8cedc-103">Methods</span></span>

| <span data-ttu-id="8cedc-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="8cedc-104">Method</span></span>           | <span data-ttu-id="8cedc-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8cedc-105">Return Type</span></span>    |<span data-ttu-id="8cedc-106">説明</span><span class="sxs-lookup"><span data-stu-id="8cedc-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8cedc-107">Get RangeFormat</span><span class="sxs-lookup"><span data-stu-id="8cedc-107">Get RangeFormat</span></span>](../api/rangeformat_get.md) | [<span data-ttu-id="8cedc-108">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="8cedc-108">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="8cedc-109">rangeFormat オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8cedc-109">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="8cedc-110">Create RangeBorder</span><span class="sxs-lookup"><span data-stu-id="8cedc-110">Create RangeBorder</span></span>](../api/rangeformat_post_borders.md) |[<span data-ttu-id="8cedc-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="8cedc-111">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="8cedc-112">罫線コレクションに投稿して、新しい RangeBorder を作成します。</span><span class="sxs-lookup"><span data-stu-id="8cedc-112">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="8cedc-113">List borders</span><span class="sxs-lookup"><span data-stu-id="8cedc-113">List borders</span></span>](../api/rangeformat_list_borders.md) |<span data-ttu-id="8cedc-114">[WorkbookRangeBorder](rangeborder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8cedc-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="8cedc-115">RangeBorder オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8cedc-115">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="8cedc-116">Update</span><span class="sxs-lookup"><span data-stu-id="8cedc-116">Update</span></span>](../api/rangeformat_update.md) | [<span data-ttu-id="8cedc-117">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="8cedc-117">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="8cedc-118">RangeFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="8cedc-118">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="8cedc-119">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="8cedc-119">Autofitcolumns</span></span>](../api/rangeformat_autofitcolumns.md)|<span data-ttu-id="8cedc-120">なし</span><span class="sxs-lookup"><span data-stu-id="8cedc-120">None</span></span>|<span data-ttu-id="8cedc-121">列の現在のデータに基づいて、現在の範囲の列の幅が最適なものになるように変更します。</span><span class="sxs-lookup"><span data-stu-id="8cedc-121">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="8cedc-122">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="8cedc-122">Autofitrows</span></span>](../api/rangeformat_autofitrows.md)|<span data-ttu-id="8cedc-123">なし</span><span class="sxs-lookup"><span data-stu-id="8cedc-123">None</span></span>|<span data-ttu-id="8cedc-124">現在の行のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。</span><span class="sxs-lookup"><span data-stu-id="8cedc-124">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cedc-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cedc-125">Properties</span></span>
| <span data-ttu-id="8cedc-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cedc-126">Property</span></span>     | <span data-ttu-id="8cedc-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="8cedc-127">Type</span></span>   |<span data-ttu-id="8cedc-128">説明</span><span class="sxs-lookup"><span data-stu-id="8cedc-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cedc-129">columnWidth</span><span class="sxs-lookup"><span data-stu-id="8cedc-129">columnWidth</span></span>|<span data-ttu-id="8cedc-130">double</span><span class="sxs-lookup"><span data-stu-id="8cedc-130">double</span></span>|<span data-ttu-id="8cedc-p101">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="8cedc-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="8cedc-133">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="8cedc-133">horizontalAlignment</span></span>|<span data-ttu-id="8cedc-134">string</span><span class="sxs-lookup"><span data-stu-id="8cedc-134">string</span></span>|<span data-ttu-id="8cedc-135">指定したオブジェクトの水平方向の配置を表します。</span><span class="sxs-lookup"><span data-stu-id="8cedc-135">Returns or sets the horizontal alignment for the specified object.</span></span> <span data-ttu-id="8cedc-136">指定できる値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="8cedc-136">The possible values are `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`, , , , or .</span></span>|
|<span data-ttu-id="8cedc-137">rowHeight</span><span class="sxs-lookup"><span data-stu-id="8cedc-137">rowHeight</span></span>|<span data-ttu-id="8cedc-138">double</span><span class="sxs-lookup"><span data-stu-id="8cedc-138">double</span></span>|<span data-ttu-id="8cedc-p103">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="8cedc-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="8cedc-141">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="8cedc-141">verticalAlignment</span></span>|<span data-ttu-id="8cedc-142">string</span><span class="sxs-lookup"><span data-stu-id="8cedc-142">string</span></span>|<span data-ttu-id="8cedc-143">指定したオブジェクトの垂直方向の配置を表します。</span><span class="sxs-lookup"><span data-stu-id="8cedc-143">Represents the vertical alignment for the specified object. Possible values are: , , , , .</span></span> <span data-ttu-id="8cedc-144">可能な値は、   `Top`、   `Center`、   `Bottom`、  `Justify`、   `Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="8cedc-144">The possible values are `Top`, `Center`, `Bottom`, `Justify`, `Distributed`, , , , , , , or .</span></span>|
|<span data-ttu-id="8cedc-145">wrapText</span><span class="sxs-lookup"><span data-stu-id="8cedc-145">wrapText</span></span>|<span data-ttu-id="8cedc-146">boolean</span><span class="sxs-lookup"><span data-stu-id="8cedc-146">boolean</span></span>|<span data-ttu-id="8cedc-p105">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="8cedc-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cedc-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cedc-149">Relationships</span></span>
| <span data-ttu-id="8cedc-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cedc-150">Relationship</span></span> | <span data-ttu-id="8cedc-151">型</span><span class="sxs-lookup"><span data-stu-id="8cedc-151">Type</span></span>   |<span data-ttu-id="8cedc-152">説明</span><span class="sxs-lookup"><span data-stu-id="8cedc-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cedc-153">borders</span><span class="sxs-lookup"><span data-stu-id="8cedc-153">borders</span></span>|<span data-ttu-id="8cedc-154">[WorkbookRangeBorder](rangeborder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8cedc-154">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="8cedc-155">選択した範囲全体に適用する罫線オブジェクトのコレクションです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8cedc-155">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="8cedc-156">fill</span><span class="sxs-lookup"><span data-stu-id="8cedc-156">fill</span></span>|[<span data-ttu-id="8cedc-157">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="8cedc-157">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="8cedc-p106">範囲全体に定義された塗りつぶしオブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8cedc-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="8cedc-160">font</span><span class="sxs-lookup"><span data-stu-id="8cedc-160">font</span></span>|[<span data-ttu-id="8cedc-161">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="8cedc-161">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="8cedc-162">選択した範囲全体に定義されているフォント オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8cedc-162">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="8cedc-163">protection</span><span class="sxs-lookup"><span data-stu-id="8cedc-163">protection</span></span>|[<span data-ttu-id="8cedc-164">WorkbookFormatProtection</span><span class="sxs-lookup"><span data-stu-id="8cedc-164">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="8cedc-p107">範囲に対する書式保護オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8cedc-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cedc-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cedc-167">JSON representation</span></span>

<span data-ttu-id="8cedc-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cedc-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->