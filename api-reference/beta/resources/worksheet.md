---
title: ワークシート リソースの種類
description: Excel のワークシートは、セルのグリッドになっています。そこに、データ、表、グラフなどを含めることができます。
ms.openlocfilehash: 513a1fceb8e0b7e2c7667d5fac2e4a5978ed7c04
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067471"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="f0be0-104">ワークシート リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0be0-104">Worksheet resource type</span></span>

> <span data-ttu-id="f0be0-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0be0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0be0-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0be0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0be0-p103">Excel のワークシートは、セルのグリッドになっています。そこに、データ、表、グラフなどを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p103">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="f0be0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f0be0-109">Methods</span></span>

| <span data-ttu-id="f0be0-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f0be0-110">Method</span></span>           | <span data-ttu-id="f0be0-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f0be0-111">Return Type</span></span>    |<span data-ttu-id="f0be0-112">説明</span><span class="sxs-lookup"><span data-stu-id="f0be0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0be0-113">ワークシートを取得する</span><span class="sxs-lookup"><span data-stu-id="f0be0-113">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="f0be0-114">Worksheet</span><span class="sxs-lookup"><span data-stu-id="f0be0-114">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="f0be0-115">ワークシート オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f0be0-115">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="f0be0-116">グラフを作成する</span><span class="sxs-lookup"><span data-stu-id="f0be0-116">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="f0be0-117">Chart</span><span class="sxs-lookup"><span data-stu-id="f0be0-117">Chart</span></span>](chart.md)| <span data-ttu-id="f0be0-118">グラフ コレクションに投稿して、新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-118">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="f0be0-119">名前を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f0be0-119">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="f0be0-120">[NamedItem](nameditem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-120">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="f0be0-121">ワークシートに関連付けられている名前付きのアイテムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-121">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="f0be0-122">グラフを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f0be0-122">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="f0be0-123">[Chart](chart.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-123">[Chart](chart.md) collection</span></span>| <span data-ttu-id="f0be0-124">グラフ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-124">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="f0be0-125">テーブルを作成する</span><span class="sxs-lookup"><span data-stu-id="f0be0-125">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="f0be0-126">Table</span><span class="sxs-lookup"><span data-stu-id="f0be0-126">Table</span></span>](table.md)| <span data-ttu-id="f0be0-127">テーブル コレクションに投稿して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-127">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="f0be0-128">テーブルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f0be0-128">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="f0be0-129">[Table](table.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-129">[Table](table.md) collection</span></span>| <span data-ttu-id="f0be0-130">テーブル オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-130">Get a Table object collection.</span></span>|
|[<span data-ttu-id="f0be0-131">Update</span><span class="sxs-lookup"><span data-stu-id="f0be0-131">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="f0be0-132">Worksheet</span><span class="sxs-lookup"><span data-stu-id="f0be0-132">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="f0be0-133">ワークシート オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-133">Update Worksheet object.</span></span> |
|[<span data-ttu-id="f0be0-134">Cell</span><span class="sxs-lookup"><span data-stu-id="f0be0-134">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="f0be0-135">印刷範囲</span><span class="sxs-lookup"><span data-stu-id="f0be0-135">Range</span></span>](range.md)|<span data-ttu-id="f0be0-p104">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p104">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="f0be0-138">Range</span><span class="sxs-lookup"><span data-stu-id="f0be0-138">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="f0be0-139">Range</span><span class="sxs-lookup"><span data-stu-id="f0be0-139">Range</span></span>](range.md)|<span data-ttu-id="f0be0-140">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-140">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="f0be0-141">Usedrange</span><span class="sxs-lookup"><span data-stu-id="f0be0-141">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="f0be0-142">印刷範囲</span><span class="sxs-lookup"><span data-stu-id="f0be0-142">Range</span></span>](range.md)|<span data-ttu-id="f0be0-p105">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p105">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="f0be0-145">削除</span><span class="sxs-lookup"><span data-stu-id="f0be0-145">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="f0be0-146">なし</span><span class="sxs-lookup"><span data-stu-id="f0be0-146">None</span></span>|<span data-ttu-id="f0be0-147">ブックからワークシートを削除します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-147">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="f0be0-148">List</span><span class="sxs-lookup"><span data-stu-id="f0be0-148">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="f0be0-149">[Worksheet](worksheet.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-149">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="f0be0-150">ワークシート オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-150">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="f0be0-151">追加</span><span class="sxs-lookup"><span data-stu-id="f0be0-151">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="f0be0-152">Worksheet</span><span class="sxs-lookup"><span data-stu-id="f0be0-152">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="f0be0-p106">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p106">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="f0be0-155">pivotTables を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f0be0-155">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="f0be0-156">[workbookPivotTable](workbookpivottable.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-156">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="f0be0-157">workbookPivotTable オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f0be0-157">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0be0-158">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0be0-158">Properties</span></span>
| <span data-ttu-id="f0be0-159">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0be0-159">Property</span></span>     | <span data-ttu-id="f0be0-160">型</span><span class="sxs-lookup"><span data-stu-id="f0be0-160">Type</span></span>   |<span data-ttu-id="f0be0-161">説明</span><span class="sxs-lookup"><span data-stu-id="f0be0-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0be0-162">ID</span><span class="sxs-lookup"><span data-stu-id="f0be0-162">id</span></span>|<span data-ttu-id="f0be0-163">文字列</span><span class="sxs-lookup"><span data-stu-id="f0be0-163">string</span></span>|<span data-ttu-id="f0be0-p107">指定されたブックのワークシートを一意に識別する値を返します。この識別子の値は、ワークシートの名前を変更したり移動したりしても同じままです。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p107">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="f0be0-167">name</span><span class="sxs-lookup"><span data-stu-id="f0be0-167">name</span></span>|<span data-ttu-id="f0be0-168">文字列</span><span class="sxs-lookup"><span data-stu-id="f0be0-168">string</span></span>|<span data-ttu-id="f0be0-169">ワークシートの表示名。</span><span class="sxs-lookup"><span data-stu-id="f0be0-169">The display name of the worksheet.</span></span>|
|<span data-ttu-id="f0be0-170">position</span><span class="sxs-lookup"><span data-stu-id="f0be0-170">position</span></span>|<span data-ttu-id="f0be0-171">int</span><span class="sxs-lookup"><span data-stu-id="f0be0-171">int</span></span>|<span data-ttu-id="f0be0-172">0 を起点とした、ブック内のワークシートの位置。</span><span class="sxs-lookup"><span data-stu-id="f0be0-172">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="f0be0-173">visibility</span><span class="sxs-lookup"><span data-stu-id="f0be0-173">visibility</span></span>|<span data-ttu-id="f0be0-174">文字列</span><span class="sxs-lookup"><span data-stu-id="f0be0-174">string</span></span>|<span data-ttu-id="f0be0-p108">ワークシートの可視性。可能な値は、`Visible`、`Hidden`、`VeryHidden` です。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p108">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0be0-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0be0-177">Relationships</span></span>
| <span data-ttu-id="f0be0-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0be0-178">Relationship</span></span> | <span data-ttu-id="f0be0-179">型</span><span class="sxs-lookup"><span data-stu-id="f0be0-179">Type</span></span>   |<span data-ttu-id="f0be0-180">説明</span><span class="sxs-lookup"><span data-stu-id="f0be0-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0be0-181">charts</span><span class="sxs-lookup"><span data-stu-id="f0be0-181">charts</span></span>|<span data-ttu-id="f0be0-182">[Chart](chart.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-182">[Chart](chart.md) collection</span></span>|<span data-ttu-id="f0be0-p109">ワークシートの一部になっているグラフのコレクションを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p109">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="f0be0-185">names</span><span class="sxs-lookup"><span data-stu-id="f0be0-185">names</span></span>|<span data-ttu-id="f0be0-186">[NamedItem](nameditem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-186">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="f0be0-p110">ワークシートに関連付けられている名前のコレクションを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p110">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="f0be0-189">pivotTables</span><span class="sxs-lookup"><span data-stu-id="f0be0-189">pivotTables</span></span>|<span data-ttu-id="f0be0-190">[workbookPivotTable](workbookpivottable.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-190">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="f0be0-191">ワークシートの一部になっているピボットテーブルのコレクション。</span><span class="sxs-lookup"><span data-stu-id="f0be0-191">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="f0be0-192">protection</span><span class="sxs-lookup"><span data-stu-id="f0be0-192">protection</span></span>|[<span data-ttu-id="f0be0-193">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="f0be0-193">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="f0be0-p111">ワークシートのシート保護オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p111">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="f0be0-196">テーブル</span><span class="sxs-lookup"><span data-stu-id="f0be0-196">tables</span></span>|<span data-ttu-id="f0be0-197">[Table](table.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f0be0-197">[Table](table.md) collection</span></span>|<span data-ttu-id="f0be0-p112">ワークシートの一部になっているグラフのコレクション。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f0be0-p112">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0be0-200">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0be0-200">JSON representation</span></span>

<span data-ttu-id="f0be0-201">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0be0-201">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
