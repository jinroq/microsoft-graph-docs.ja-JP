# <a name="rangeview-resource-type"></a><span data-ttu-id="82114-101">rangeView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82114-101">rangeView resource type</span></span>
<span data-ttu-id="82114-102">RangeView は、親の範囲の表示されているセルのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="82114-102">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="82114-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="82114-103">Methods</span></span>

| <span data-ttu-id="82114-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="82114-104">Method</span></span>           | <span data-ttu-id="82114-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="82114-105">Return Type</span></span>    |<span data-ttu-id="82114-106">説明</span><span class="sxs-lookup"><span data-stu-id="82114-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82114-107">行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="82114-107">List rows</span></span>](../api/workbookrangeview_list_rows.md) |<span data-ttu-id="82114-108">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="82114-108">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="82114-109">workbookRangeView オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="82114-109">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="82114-110">Itemat</span><span class="sxs-lookup"><span data-stu-id="82114-110">Itemat</span></span>](../api/workbookrangeview_itemat.md)|[<span data-ttu-id="82114-111">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="82114-111">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="82114-112">インデックスに基づいて範囲ビューの項目を取得します。</span><span class="sxs-lookup"><span data-stu-id="82114-112">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="82114-113">Range</span><span class="sxs-lookup"><span data-stu-id="82114-113">Range</span></span>](../api/workbookrangeview_range.md)|[<span data-ttu-id="82114-114">workbookRange</span><span class="sxs-lookup"><span data-stu-id="82114-114">workbookRange</span></span>](range.md)|<span data-ttu-id="82114-115">範囲ビューに関連付けられた範囲オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82114-115">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="82114-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82114-116">Properties</span></span>
| <span data-ttu-id="82114-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82114-117">Property</span></span>     | <span data-ttu-id="82114-118">型</span><span class="sxs-lookup"><span data-stu-id="82114-118">Type</span></span>   |<span data-ttu-id="82114-119">説明</span><span class="sxs-lookup"><span data-stu-id="82114-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82114-120">columnCount</span><span class="sxs-lookup"><span data-stu-id="82114-120">columnCount</span></span>|<span data-ttu-id="82114-121">Int32</span><span class="sxs-lookup"><span data-stu-id="82114-121">Int32</span></span>|<span data-ttu-id="82114-p101">表示されている列の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="82114-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="82114-124">formulas</span><span class="sxs-lookup"><span data-stu-id="82114-124">formulas</span></span>|<span data-ttu-id="82114-125">Json</span><span class="sxs-lookup"><span data-stu-id="82114-125">Json</span></span>|<span data-ttu-id="82114-126">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="82114-126">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="82114-127">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="82114-127">formulasLocal</span></span>|<span data-ttu-id="82114-128">Json</span><span class="sxs-lookup"><span data-stu-id="82114-128">Json</span></span>|<span data-ttu-id="82114-p102">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="82114-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="82114-131">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="82114-131">formulasR1C1</span></span>|<span data-ttu-id="82114-132">Json</span><span class="sxs-lookup"><span data-stu-id="82114-132">Json</span></span>|<span data-ttu-id="82114-133">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="82114-133">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="82114-134">index</span><span class="sxs-lookup"><span data-stu-id="82114-134">index</span></span>|<span data-ttu-id="82114-135">Int32</span><span class="sxs-lookup"><span data-stu-id="82114-135">Int32</span></span>|<span data-ttu-id="82114-136">範囲のインデックス。</span><span class="sxs-lookup"><span data-stu-id="82114-136">Index of the range.</span></span>|
|<span data-ttu-id="82114-137">numberFormat</span><span class="sxs-lookup"><span data-stu-id="82114-137">numberFormat</span></span>|<span data-ttu-id="82114-138">Json</span><span class="sxs-lookup"><span data-stu-id="82114-138">Json</span></span>|<span data-ttu-id="82114-p103">指定したセルの Excel の数値書式コードを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="82114-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="82114-141">rowCount</span><span class="sxs-lookup"><span data-stu-id="82114-141">rowCount</span></span>|<span data-ttu-id="82114-142">Int32</span><span class="sxs-lookup"><span data-stu-id="82114-142">Int32</span></span>|<span data-ttu-id="82114-p104">表示されている行の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="82114-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="82114-145">text</span><span class="sxs-lookup"><span data-stu-id="82114-145">text</span></span>|<span data-ttu-id="82114-146">Json</span><span class="sxs-lookup"><span data-stu-id="82114-146">Json</span></span>|<span data-ttu-id="82114-p105">指定した範囲のテキスト値。テキスト値は、セルの幅には依存しません。Excel UI で発生する # 記号による置換は、この API から返されるテキスト値には影響しません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="82114-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="82114-151">valueTypes</span><span class="sxs-lookup"><span data-stu-id="82114-151">valueTypes</span></span>|<span data-ttu-id="82114-152">Json</span><span class="sxs-lookup"><span data-stu-id="82114-152">Json</span></span>|<span data-ttu-id="82114-p106">各セルのデータの種類を表します。読み取り専用です。使用可能な値は次のとおりです。Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="82114-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="82114-156">values</span><span class="sxs-lookup"><span data-stu-id="82114-156">values</span></span>|<span data-ttu-id="82114-157">Json</span><span class="sxs-lookup"><span data-stu-id="82114-157">Json</span></span>|<span data-ttu-id="82114-p107">指定した範囲ビューの Raw 値を表します。返されるデータの型は、文字列、数値、ブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="82114-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="82114-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82114-161">Relationships</span></span>
| <span data-ttu-id="82114-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82114-162">Relationship</span></span> | <span data-ttu-id="82114-163">型</span><span class="sxs-lookup"><span data-stu-id="82114-163">Type</span></span>   |<span data-ttu-id="82114-164">説明</span><span class="sxs-lookup"><span data-stu-id="82114-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82114-165">rows</span><span class="sxs-lookup"><span data-stu-id="82114-165">rows</span></span>|<span data-ttu-id="82114-166">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="82114-166">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="82114-p108">範囲に関連付けられている範囲ビューのコレクションを表します。読み取り専用です。  読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="82114-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82114-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82114-170">JSON representation</span></span>
<span data-ttu-id="82114-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82114-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
