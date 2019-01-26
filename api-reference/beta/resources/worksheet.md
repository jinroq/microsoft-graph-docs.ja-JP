---
title: ワークシート リソースの種類
description: Excel のワークシートは、セルのグリッドになっています。そこに、データ、表、グラフなどを含めることができます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6a3a5fbb222c9228b55b2dac2a38b699ed15f213
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574377"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="28b6e-104">ワークシート リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28b6e-104">Worksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b6e-p102">Excel のワークシートは、セルのグリッドになっています。そこに、データ、表、グラフなどを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="28b6e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="28b6e-107">Methods</span></span>

| <span data-ttu-id="28b6e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="28b6e-108">Method</span></span>           | <span data-ttu-id="28b6e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="28b6e-109">Return Type</span></span>    |<span data-ttu-id="28b6e-110">説明</span><span class="sxs-lookup"><span data-stu-id="28b6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28b6e-111">ワークシートを取得する</span><span class="sxs-lookup"><span data-stu-id="28b6e-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="28b6e-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="28b6e-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="28b6e-113">ワークシート オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="28b6e-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="28b6e-114">グラフを作成する</span><span class="sxs-lookup"><span data-stu-id="28b6e-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="28b6e-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="28b6e-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="28b6e-116">グラフ コレクションに投稿して、新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="28b6e-117">名前を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="28b6e-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="28b6e-118">[WorkbookNamedItem](workbooknameditem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-118">[WorkbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="28b6e-119">ワークシートに関連付けられている名前付きのアイテムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="28b6e-120">グラフを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="28b6e-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="28b6e-121">[WorkbookChart](chart.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="28b6e-122">グラフ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="28b6e-123">テーブルを作成する</span><span class="sxs-lookup"><span data-stu-id="28b6e-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="28b6e-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="28b6e-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="28b6e-125">テーブル コレクションに投稿して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="28b6e-126">テーブルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="28b6e-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="28b6e-127">[WorkbookTable](table.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="28b6e-128">テーブル オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="28b6e-129">Update</span><span class="sxs-lookup"><span data-stu-id="28b6e-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="28b6e-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="28b6e-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="28b6e-131">ワークシート オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="28b6e-132">Cell</span><span class="sxs-lookup"><span data-stu-id="28b6e-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="28b6e-133">Range</span><span class="sxs-lookup"><span data-stu-id="28b6e-133">Range</span></span>](range.md)|<span data-ttu-id="28b6e-p103">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="28b6e-136">Range</span><span class="sxs-lookup"><span data-stu-id="28b6e-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="28b6e-137">Range</span><span class="sxs-lookup"><span data-stu-id="28b6e-137">Range</span></span>](range.md)|<span data-ttu-id="28b6e-138">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="28b6e-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="28b6e-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="28b6e-140">Range</span><span class="sxs-lookup"><span data-stu-id="28b6e-140">Range</span></span>](range.md)|<span data-ttu-id="28b6e-p104">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="28b6e-143">Delete</span><span class="sxs-lookup"><span data-stu-id="28b6e-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="28b6e-144">なし</span><span class="sxs-lookup"><span data-stu-id="28b6e-144">None</span></span>|<span data-ttu-id="28b6e-145">ブックからワークシートを削除します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="28b6e-146">List</span><span class="sxs-lookup"><span data-stu-id="28b6e-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="28b6e-147">[WorkbookWorksheet](worksheet.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="28b6e-148">ワークシート オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="28b6e-149">Add</span><span class="sxs-lookup"><span data-stu-id="28b6e-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="28b6e-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="28b6e-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="28b6e-p105">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="28b6e-153">pivotTables を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="28b6e-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="28b6e-154">[workbookPivotTable](workbookpivottable.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="28b6e-155">workbookPivotTable オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="28b6e-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="28b6e-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28b6e-156">Properties</span></span>
| <span data-ttu-id="28b6e-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28b6e-157">Property</span></span>     | <span data-ttu-id="28b6e-158">型</span><span class="sxs-lookup"><span data-stu-id="28b6e-158">Type</span></span>   |<span data-ttu-id="28b6e-159">説明</span><span class="sxs-lookup"><span data-stu-id="28b6e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28b6e-160">id</span><span class="sxs-lookup"><span data-stu-id="28b6e-160">id</span></span>|<span data-ttu-id="28b6e-161">文字列</span><span class="sxs-lookup"><span data-stu-id="28b6e-161">string</span></span>|<span data-ttu-id="28b6e-p106">指定されたブックのワークシートを一意に識別する値を返します。この識別子の値は、ワークシートの名前を変更したり移動したりしても同じままです。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="28b6e-165">name</span><span class="sxs-lookup"><span data-stu-id="28b6e-165">name</span></span>|<span data-ttu-id="28b6e-166">文字列</span><span class="sxs-lookup"><span data-stu-id="28b6e-166">string</span></span>|<span data-ttu-id="28b6e-167">ワークシートの表示名。</span><span class="sxs-lookup"><span data-stu-id="28b6e-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="28b6e-168">position</span><span class="sxs-lookup"><span data-stu-id="28b6e-168">position</span></span>|<span data-ttu-id="28b6e-169">int</span><span class="sxs-lookup"><span data-stu-id="28b6e-169">int</span></span>|<span data-ttu-id="28b6e-170">0 を起点とした、ブック内のワークシートの位置。</span><span class="sxs-lookup"><span data-stu-id="28b6e-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="28b6e-171">visibility</span><span class="sxs-lookup"><span data-stu-id="28b6e-171">visibility</span></span>|<span data-ttu-id="28b6e-172">文字列</span><span class="sxs-lookup"><span data-stu-id="28b6e-172">string</span></span>|<span data-ttu-id="28b6e-173">ワークシートの可視性。</span><span class="sxs-lookup"><span data-stu-id="28b6e-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="28b6e-174">可能な値: `Visible`、 `Hidden`、 `VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="28b6e-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28b6e-175">関係</span><span class="sxs-lookup"><span data-stu-id="28b6e-175">Relationships</span></span>
| <span data-ttu-id="28b6e-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28b6e-176">Relationship</span></span> | <span data-ttu-id="28b6e-177">型</span><span class="sxs-lookup"><span data-stu-id="28b6e-177">Type</span></span>   |<span data-ttu-id="28b6e-178">説明</span><span class="sxs-lookup"><span data-stu-id="28b6e-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28b6e-179">charts</span><span class="sxs-lookup"><span data-stu-id="28b6e-179">charts</span></span>|<span data-ttu-id="28b6e-180">[WorkbookChart](chart.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="28b6e-p108">ワークシートの一部になっているグラフのコレクションを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="28b6e-183">names</span><span class="sxs-lookup"><span data-stu-id="28b6e-183">names</span></span>|<span data-ttu-id="28b6e-184">[workbookNamedItem](workbooknameditem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-184">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="28b6e-p109">ワークシートに関連付けられている名前のコレクションを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="28b6e-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="28b6e-187">pivotTables</span></span>|<span data-ttu-id="28b6e-188">[workbookPivotTable](workbookpivottable.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="28b6e-189">ワークシートの一部になっているピボットテーブルのコレクション。</span><span class="sxs-lookup"><span data-stu-id="28b6e-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="28b6e-190">protection</span><span class="sxs-lookup"><span data-stu-id="28b6e-190">protection</span></span>|[<span data-ttu-id="28b6e-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="28b6e-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="28b6e-p110">ワークシートのシート保護オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="28b6e-194">テーブル</span><span class="sxs-lookup"><span data-stu-id="28b6e-194">tables</span></span>|<span data-ttu-id="28b6e-195">[WorkbookTable](table.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="28b6e-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="28b6e-p111">ワークシートの一部になっているグラフのコレクション。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="28b6e-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28b6e-198">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28b6e-198">JSON representation</span></span>

<span data-ttu-id="28b6e-199">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="28b6e-199">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
