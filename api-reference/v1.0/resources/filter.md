# <a name="filter-resource-type"></a><span data-ttu-id="14793-101">フィルター リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14793-101">Filter resource type</span></span>

<span data-ttu-id="14793-102">テーブルの列のフィルター処理を管理します。</span><span class="sxs-lookup"><span data-stu-id="14793-102">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="14793-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="14793-103">Methods</span></span>

| <span data-ttu-id="14793-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="14793-104">Method</span></span>           | <span data-ttu-id="14793-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14793-105">Return Type</span></span>    |<span data-ttu-id="14793-106">説明</span><span class="sxs-lookup"><span data-stu-id="14793-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14793-107">適用する</span><span class="sxs-lookup"><span data-stu-id="14793-107">Apply</span></span>](../api/filter_apply.md)|<span data-ttu-id="14793-108">なし</span><span class="sxs-lookup"><span data-stu-id="14793-108">None</span></span>|<span data-ttu-id="14793-109">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="14793-109">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="14793-110">Clear</span><span class="sxs-lookup"><span data-stu-id="14793-110">Clear</span></span>](../api/filter_clear.md)|<span data-ttu-id="14793-111">なし</span><span class="sxs-lookup"><span data-stu-id="14793-111">None</span></span>|<span data-ttu-id="14793-112">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="14793-112">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="14793-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14793-113">Properties</span></span>

| <span data-ttu-id="14793-114">名前</span><span class="sxs-lookup"><span data-stu-id="14793-114">Name</span></span> | <span data-ttu-id="14793-115">型</span><span class="sxs-lookup"><span data-stu-id="14793-115">Type</span></span>   |<span data-ttu-id="14793-116">説明</span><span class="sxs-lookup"><span data-stu-id="14793-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14793-117">criteria</span><span class="sxs-lookup"><span data-stu-id="14793-117">criteria</span></span>|[<span data-ttu-id="14793-118">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="14793-118">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="14793-p101">指定した列に現在適用されているフィルターです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="14793-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14793-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14793-121">JSON representation</span></span>

<span data-ttu-id="14793-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14793-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->