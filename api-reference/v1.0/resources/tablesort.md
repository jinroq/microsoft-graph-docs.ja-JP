# <a name="tablesort-resource-type"></a><span data-ttu-id="a6674-101">TableSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6674-101">TableSort resource type</span></span>

<span data-ttu-id="a6674-102">テーブル オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="a6674-102">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="a6674-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6674-103">Methods</span></span>

| <span data-ttu-id="a6674-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6674-104">Method</span></span>           | <span data-ttu-id="a6674-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a6674-105">Return Type</span></span>    |<span data-ttu-id="a6674-106">説明</span><span class="sxs-lookup"><span data-stu-id="a6674-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6674-107">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="a6674-107">Get TableSort</span></span>](../api/tablesort_get.md) | [<span data-ttu-id="a6674-108">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="a6674-108">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="a6674-109">tableSort オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a6674-109">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="a6674-110">Apply</span><span class="sxs-lookup"><span data-stu-id="a6674-110">Apply</span></span>](../api/tablesort_apply.md)|<span data-ttu-id="a6674-111">なし</span><span class="sxs-lookup"><span data-stu-id="a6674-111">None</span></span>|<span data-ttu-id="a6674-112">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="a6674-112">Perform a sort operation.</span></span>|
|[<span data-ttu-id="a6674-113">Clear</span><span class="sxs-lookup"><span data-stu-id="a6674-113">Clear</span></span>](../api/tablesort_clear.md)|<span data-ttu-id="a6674-114">なし</span><span class="sxs-lookup"><span data-stu-id="a6674-114">None</span></span>|<span data-ttu-id="a6674-p101">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="a6674-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="a6674-117">Reapply</span><span class="sxs-lookup"><span data-stu-id="a6674-117">Reapply</span></span>](../api/tablesort_reapply.md)|<span data-ttu-id="a6674-118">なし</span><span class="sxs-lookup"><span data-stu-id="a6674-118">None</span></span>|<span data-ttu-id="a6674-119">テーブルに、現在の並べ替えパラメーターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="a6674-119">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6674-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6674-120">Properties</span></span>
| <span data-ttu-id="a6674-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6674-121">Property</span></span>     | <span data-ttu-id="a6674-122">タイプ</span><span class="sxs-lookup"><span data-stu-id="a6674-122">Type</span></span>   |<span data-ttu-id="a6674-123">説明</span><span class="sxs-lookup"><span data-stu-id="a6674-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6674-124">fields</span><span class="sxs-lookup"><span data-stu-id="a6674-124">fields</span></span>|<span data-ttu-id="a6674-125">[WorkbookSortField](sortfield.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6674-125">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="a6674-p102">テーブルの最後の並べ替え操作に使用する現在の条件を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6674-p102">Represents the current conditions used to last sort the table. Read-only.</span></span>|
|<span data-ttu-id="a6674-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="a6674-128">matchCase</span></span>|<span data-ttu-id="a6674-129">boolean</span><span class="sxs-lookup"><span data-stu-id="a6674-129">boolean</span></span>|<span data-ttu-id="a6674-p103">大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6674-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="a6674-132">method</span><span class="sxs-lookup"><span data-stu-id="a6674-132">method</span></span>|<span data-ttu-id="a6674-133">string</span><span class="sxs-lookup"><span data-stu-id="a6674-133">string</span></span>|<span data-ttu-id="a6674-134">テーブルの最後の並べ替え操作に使用される中国語文字の順序の指定方法を表します。</span><span class="sxs-lookup"><span data-stu-id="a6674-134">Represents Chinese character ordering method last used to sort the table. Possible values are: , . Read-only.</span></span> <span data-ttu-id="a6674-135">可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="a6674-135">The possible values are:</span></span> <span data-ttu-id="a6674-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a6674-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6674-137">JSON 表現</span><span class="sxs-lookup"><span data-stu-id="a6674-137">JSON representation</span></span>

<span data-ttu-id="a6674-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a6674-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->