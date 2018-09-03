# <a name="pivottable-resource-type"></a><span data-ttu-id="cc8a5-101">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc8a5-101">pivotTable resource type</span></span>

<span data-ttu-id="cc8a5-102">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="cc8a5-102">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="cc8a5-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc8a5-103">Methods</span></span>

| <span data-ttu-id="cc8a5-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc8a5-104">Method</span></span>           | <span data-ttu-id="cc8a5-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cc8a5-105">Return Type</span></span>    |<span data-ttu-id="cc8a5-106">説明</span><span class="sxs-lookup"><span data-stu-id="cc8a5-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc8a5-107">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="cc8a5-107">Get workbookPivotTable</span></span>](../api/workbookpivottable_get.md) | [<span data-ttu-id="cc8a5-108">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="cc8a5-108">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="cc8a5-109">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cc8a5-109">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="cc8a5-110">更新</span><span class="sxs-lookup"><span data-stu-id="cc8a5-110">Refresh</span></span>](../api/workbookpivottable_refresh.md)|<span data-ttu-id="cc8a5-111">なし</span><span class="sxs-lookup"><span data-stu-id="cc8a5-111">None</span></span>|<span data-ttu-id="cc8a5-112">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc8a5-112">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="cc8a5-113">Refreshall</span><span class="sxs-lookup"><span data-stu-id="cc8a5-113">Refreshall</span></span>](../api/workbookpivottable_refreshall.md)|<span data-ttu-id="cc8a5-114">なし</span><span class="sxs-lookup"><span data-stu-id="cc8a5-114">None</span></span>|<span data-ttu-id="cc8a5-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="cc8a5-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc8a5-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc8a5-117">Properties</span></span>
| <span data-ttu-id="cc8a5-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc8a5-118">Property</span></span>     | <span data-ttu-id="cc8a5-119">タイプ</span><span class="sxs-lookup"><span data-stu-id="cc8a5-119">Type</span></span>   |<span data-ttu-id="cc8a5-120">説明</span><span class="sxs-lookup"><span data-stu-id="cc8a5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc8a5-121">ID</span><span class="sxs-lookup"><span data-stu-id="cc8a5-121">id</span></span>|<span data-ttu-id="cc8a5-122">文字列</span><span class="sxs-lookup"><span data-stu-id="cc8a5-122">String</span></span>| <span data-ttu-id="cc8a5-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cc8a5-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="cc8a5-125">名前</span><span class="sxs-lookup"><span data-stu-id="cc8a5-125">name</span></span>|<span data-ttu-id="cc8a5-126">文字列</span><span class="sxs-lookup"><span data-stu-id="cc8a5-126">String</span></span>|<span data-ttu-id="cc8a5-127">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="cc8a5-127">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="cc8a5-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc8a5-128">Relationships</span></span>
| <span data-ttu-id="cc8a5-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc8a5-129">Relationship</span></span> | <span data-ttu-id="cc8a5-130">型</span><span class="sxs-lookup"><span data-stu-id="cc8a5-130">Type</span></span>   |<span data-ttu-id="cc8a5-131">説明</span><span class="sxs-lookup"><span data-stu-id="cc8a5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc8a5-132">ワークシート</span><span class="sxs-lookup"><span data-stu-id="cc8a5-132">worksheet</span></span>|[<span data-ttu-id="cc8a5-133">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="cc8a5-133">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="cc8a5-p103">現在の PivotTable を含んでいるワークシート。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cc8a5-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="cc8a5-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc8a5-136">JSON representation</span></span>
<span data-ttu-id="cc8a5-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc8a5-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
