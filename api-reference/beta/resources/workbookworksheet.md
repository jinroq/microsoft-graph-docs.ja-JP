---
title: workbookWorksheet リソースの種類
description: Excel のワークシートは、セルのグリッドです。 データ、表、グラフなどを含めることができます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 1700c61ed84b1ac218163e2cff3ac812f59cc8ed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348863"
---
# <a name="workbookworksheet-resource-type"></a><span data-ttu-id="d407e-104">workbookWorksheet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d407e-104">workbookWorksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d407e-105">Excel のワークシートは、セルのグリッドです。</span><span class="sxs-lookup"><span data-stu-id="d407e-105">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="d407e-106">データ、表、グラフなどを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d407e-106">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="d407e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d407e-107">Methods</span></span>

| <span data-ttu-id="d407e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d407e-108">Method</span></span>           | <span data-ttu-id="d407e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d407e-109">Return Type</span></span>    |<span data-ttu-id="d407e-110">説明</span><span class="sxs-lookup"><span data-stu-id="d407e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d407e-111">ワークシートを取得する</span><span class="sxs-lookup"><span data-stu-id="d407e-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="d407e-112">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d407e-112">workbookWorksheet</span></span>](workbookworksheet.md) |<span data-ttu-id="d407e-113">ワークシート オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d407e-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="d407e-114">グラフを作成する</span><span class="sxs-lookup"><span data-stu-id="d407e-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="d407e-115">workbookChart</span><span class="sxs-lookup"><span data-stu-id="d407e-115">workbookChart</span></span>](workbookchart.md)| <span data-ttu-id="d407e-116">グラフ コレクションに投稿して、新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="d407e-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="d407e-117">名前を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d407e-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="d407e-118">[workbookNamedItem](workbooknameditem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-118">[workbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="d407e-119">ワークシートに関連付けられている名前付きのアイテムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d407e-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="d407e-120">グラフを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d407e-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="d407e-121">[workbookChart](workbookchart.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-121">[workbookChart](workbookchart.md) collection</span></span>| <span data-ttu-id="d407e-122">グラフ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d407e-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="d407e-123">テーブルを作成する</span><span class="sxs-lookup"><span data-stu-id="d407e-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="d407e-124">workbookTable</span><span class="sxs-lookup"><span data-stu-id="d407e-124">workbookTable</span></span>](workbooktable.md)| <span data-ttu-id="d407e-125">テーブル コレクションに投稿して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="d407e-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="d407e-126">テーブルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d407e-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="d407e-127">[workbookTable](workbooktable.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-127">[workbookTable](workbooktable.md) collection</span></span>| <span data-ttu-id="d407e-128">テーブル オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d407e-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="d407e-129">Update</span><span class="sxs-lookup"><span data-stu-id="d407e-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="d407e-130">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d407e-130">workbookWorksheet</span></span>](workbookworksheet.md)   |<span data-ttu-id="d407e-131">ワークシート オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d407e-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="d407e-132">Cell</span><span class="sxs-lookup"><span data-stu-id="d407e-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="d407e-133">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d407e-133">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d407e-p103">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="d407e-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="d407e-136">Range</span><span class="sxs-lookup"><span data-stu-id="d407e-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="d407e-137">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d407e-137">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d407e-138">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d407e-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="d407e-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="d407e-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="d407e-140">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d407e-140">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d407e-p104">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="d407e-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="d407e-143">Delete</span><span class="sxs-lookup"><span data-stu-id="d407e-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="d407e-144">なし</span><span class="sxs-lookup"><span data-stu-id="d407e-144">None</span></span>|<span data-ttu-id="d407e-145">ブックからワークシートを削除します。</span><span class="sxs-lookup"><span data-stu-id="d407e-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="d407e-146">List</span><span class="sxs-lookup"><span data-stu-id="d407e-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="d407e-147">[workbookWorksheet](workbookworksheet.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-147">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="d407e-148">ワークシート オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d407e-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="d407e-149">Add</span><span class="sxs-lookup"><span data-stu-id="d407e-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="d407e-150">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d407e-150">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="d407e-p105">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。</span><span class="sxs-lookup"><span data-stu-id="d407e-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="d407e-153">pivotTables を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d407e-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="d407e-154">[workbookPivotTable](workbookpivottable.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d407e-155">workbookPivotTable オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d407e-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d407e-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d407e-156">Properties</span></span>
| <span data-ttu-id="d407e-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d407e-157">Property</span></span>     | <span data-ttu-id="d407e-158">種類</span><span class="sxs-lookup"><span data-stu-id="d407e-158">Type</span></span>   |<span data-ttu-id="d407e-159">説明</span><span class="sxs-lookup"><span data-stu-id="d407e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d407e-160">id</span><span class="sxs-lookup"><span data-stu-id="d407e-160">id</span></span>|<span data-ttu-id="d407e-161">string</span><span class="sxs-lookup"><span data-stu-id="d407e-161">string</span></span>|<span data-ttu-id="d407e-p106">指定されたブックのワークシートを一意に識別する値を返します。この識別子の値は、ワークシートの名前を変更したり移動したりしても同じままです。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d407e-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="d407e-165">name</span><span class="sxs-lookup"><span data-stu-id="d407e-165">name</span></span>|<span data-ttu-id="d407e-166">string</span><span class="sxs-lookup"><span data-stu-id="d407e-166">string</span></span>|<span data-ttu-id="d407e-167">ワークシートの表示名。</span><span class="sxs-lookup"><span data-stu-id="d407e-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="d407e-168">position</span><span class="sxs-lookup"><span data-stu-id="d407e-168">position</span></span>|<span data-ttu-id="d407e-169">int</span><span class="sxs-lookup"><span data-stu-id="d407e-169">int</span></span>|<span data-ttu-id="d407e-170">0 を起点とした、ブック内のワークシートの位置。</span><span class="sxs-lookup"><span data-stu-id="d407e-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="d407e-171">visibility</span><span class="sxs-lookup"><span data-stu-id="d407e-171">visibility</span></span>|<span data-ttu-id="d407e-172">string</span><span class="sxs-lookup"><span data-stu-id="d407e-172">string</span></span>|<span data-ttu-id="d407e-173">ワークシートの可視性。</span><span class="sxs-lookup"><span data-stu-id="d407e-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="d407e-174">使用可能な値: `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="d407e-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d407e-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d407e-175">Relationships</span></span>
| <span data-ttu-id="d407e-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d407e-176">Relationship</span></span> | <span data-ttu-id="d407e-177">型</span><span class="sxs-lookup"><span data-stu-id="d407e-177">Type</span></span>   |<span data-ttu-id="d407e-178">説明</span><span class="sxs-lookup"><span data-stu-id="d407e-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d407e-179">グラフ</span><span class="sxs-lookup"><span data-stu-id="d407e-179">charts</span></span>|<span data-ttu-id="d407e-180">[workbookChart](workbookchart.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-180">[workbookChart](workbookchart.md) collection</span></span>|<span data-ttu-id="d407e-181">ワークシートの一部になっているグラフのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d407e-181">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="d407e-182">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d407e-182">Read-only.</span></span>|
|<span data-ttu-id="d407e-183">names</span><span class="sxs-lookup"><span data-stu-id="d407e-183">names</span></span>|<span data-ttu-id="d407e-184">[workbookNamedItem](workbooknameditem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-184">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="d407e-185">ワークシートに関連付けられている名前のコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d407e-185">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="d407e-186">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d407e-186">Read-only.</span></span>|
|<span data-ttu-id="d407e-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="d407e-187">pivotTables</span></span>|<span data-ttu-id="d407e-188">[workbookPivotTable](workbookpivottable.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d407e-189">ワークシートの一部になっているピボットテーブルのコレクション。</span><span class="sxs-lookup"><span data-stu-id="d407e-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="d407e-190">保護</span><span class="sxs-lookup"><span data-stu-id="d407e-190">protection</span></span>|[<span data-ttu-id="d407e-191">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d407e-191">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md)|<span data-ttu-id="d407e-p110">ワークシートのシート保護オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d407e-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="d407e-194">テーブル</span><span class="sxs-lookup"><span data-stu-id="d407e-194">tables</span></span>|<span data-ttu-id="d407e-195">[workbookTable](workbooktable.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d407e-195">[workbookTable](workbooktable.md) collection</span></span>|<span data-ttu-id="d407e-196">ワークシートの一部になっているグラフのコレクション。</span><span class="sxs-lookup"><span data-stu-id="d407e-196">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="d407e-197">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d407e-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d407e-198">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d407e-198">JSON representation</span></span>

<span data-ttu-id="d407e-199">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d407e-199">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
