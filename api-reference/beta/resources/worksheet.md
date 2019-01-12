---
title: ワークシート リソースの種類
description: Excel のワークシートは、セルのグリッドになっています。そこに、データ、表、グラフなどを含めることができます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: d04ebafda64f9a081096fbf0fd94461b9765a6db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926527"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="93634-104">ワークシート リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93634-104">Worksheet resource type</span></span>

> <span data-ttu-id="93634-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="93634-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93634-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93634-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93634-p103">Excel のワークシートは、セルのグリッドになっています。そこに、データ、表、グラフなどを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="93634-p103">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="93634-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="93634-109">Methods</span></span>

| <span data-ttu-id="93634-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="93634-110">Method</span></span>           | <span data-ttu-id="93634-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93634-111">Return Type</span></span>    |<span data-ttu-id="93634-112">説明</span><span class="sxs-lookup"><span data-stu-id="93634-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93634-113">ワークシートを取得する</span><span class="sxs-lookup"><span data-stu-id="93634-113">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="93634-114">Worksheet</span><span class="sxs-lookup"><span data-stu-id="93634-114">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="93634-115">ワークシート オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="93634-115">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="93634-116">グラフを作成する</span><span class="sxs-lookup"><span data-stu-id="93634-116">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="93634-117">Chart</span><span class="sxs-lookup"><span data-stu-id="93634-117">Chart</span></span>](chart.md)| <span data-ttu-id="93634-118">グラフ コレクションに投稿して、新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="93634-118">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="93634-119">名前を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="93634-119">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="93634-120">[NamedItem](nameditem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-120">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="93634-121">ワークシートに関連付けられている名前付きのアイテムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="93634-121">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="93634-122">グラフを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="93634-122">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="93634-123">[Chart](chart.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-123">[Chart](chart.md) collection</span></span>| <span data-ttu-id="93634-124">グラフ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="93634-124">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="93634-125">テーブルを作成する</span><span class="sxs-lookup"><span data-stu-id="93634-125">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="93634-126">Table</span><span class="sxs-lookup"><span data-stu-id="93634-126">Table</span></span>](table.md)| <span data-ttu-id="93634-127">テーブル コレクションに投稿して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="93634-127">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="93634-128">テーブルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="93634-128">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="93634-129">[Table](table.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-129">[Table](table.md) collection</span></span>| <span data-ttu-id="93634-130">テーブル オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="93634-130">Get a Table object collection.</span></span>|
|[<span data-ttu-id="93634-131">Update</span><span class="sxs-lookup"><span data-stu-id="93634-131">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="93634-132">Worksheet</span><span class="sxs-lookup"><span data-stu-id="93634-132">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="93634-133">ワークシート オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="93634-133">Update Worksheet object.</span></span> |
|[<span data-ttu-id="93634-134">Cell</span><span class="sxs-lookup"><span data-stu-id="93634-134">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="93634-135">Range</span><span class="sxs-lookup"><span data-stu-id="93634-135">Range</span></span>](range.md)|<span data-ttu-id="93634-p104">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="93634-p104">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="93634-138">Range</span><span class="sxs-lookup"><span data-stu-id="93634-138">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="93634-139">Range</span><span class="sxs-lookup"><span data-stu-id="93634-139">Range</span></span>](range.md)|<span data-ttu-id="93634-140">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="93634-140">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="93634-141">Usedrange</span><span class="sxs-lookup"><span data-stu-id="93634-141">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="93634-142">Range</span><span class="sxs-lookup"><span data-stu-id="93634-142">Range</span></span>](range.md)|<span data-ttu-id="93634-p105">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="93634-p105">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="93634-145">Delete</span><span class="sxs-lookup"><span data-stu-id="93634-145">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="93634-146">なし</span><span class="sxs-lookup"><span data-stu-id="93634-146">None</span></span>|<span data-ttu-id="93634-147">ブックからワークシートを削除します。</span><span class="sxs-lookup"><span data-stu-id="93634-147">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="93634-148">List</span><span class="sxs-lookup"><span data-stu-id="93634-148">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="93634-149">[Worksheet](worksheet.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-149">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="93634-150">ワークシート オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="93634-150">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="93634-151">Add</span><span class="sxs-lookup"><span data-stu-id="93634-151">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="93634-152">Worksheet</span><span class="sxs-lookup"><span data-stu-id="93634-152">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="93634-p106">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。</span><span class="sxs-lookup"><span data-stu-id="93634-p106">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="93634-155">pivotTables を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="93634-155">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="93634-156">[workbookPivotTable](workbookpivottable.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-156">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="93634-157">workbookPivotTable オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="93634-157">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="93634-158">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93634-158">Properties</span></span>
| <span data-ttu-id="93634-159">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93634-159">Property</span></span>     | <span data-ttu-id="93634-160">型</span><span class="sxs-lookup"><span data-stu-id="93634-160">Type</span></span>   |<span data-ttu-id="93634-161">説明</span><span class="sxs-lookup"><span data-stu-id="93634-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93634-162">ID</span><span class="sxs-lookup"><span data-stu-id="93634-162">id</span></span>|<span data-ttu-id="93634-163">文字列</span><span class="sxs-lookup"><span data-stu-id="93634-163">string</span></span>|<span data-ttu-id="93634-p107">指定されたブックのワークシートを一意に識別する値を返します。この識別子の値は、ワークシートの名前を変更したり移動したりしても同じままです。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="93634-p107">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="93634-167">name</span><span class="sxs-lookup"><span data-stu-id="93634-167">name</span></span>|<span data-ttu-id="93634-168">文字列</span><span class="sxs-lookup"><span data-stu-id="93634-168">string</span></span>|<span data-ttu-id="93634-169">ワークシートの表示名。</span><span class="sxs-lookup"><span data-stu-id="93634-169">The display name of the worksheet.</span></span>|
|<span data-ttu-id="93634-170">position</span><span class="sxs-lookup"><span data-stu-id="93634-170">position</span></span>|<span data-ttu-id="93634-171">int</span><span class="sxs-lookup"><span data-stu-id="93634-171">int</span></span>|<span data-ttu-id="93634-172">0 を起点とした、ブック内のワークシートの位置。</span><span class="sxs-lookup"><span data-stu-id="93634-172">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="93634-173">visibility</span><span class="sxs-lookup"><span data-stu-id="93634-173">visibility</span></span>|<span data-ttu-id="93634-174">文字列</span><span class="sxs-lookup"><span data-stu-id="93634-174">string</span></span>|<span data-ttu-id="93634-p108">ワークシートの可視性。可能な値は、`Visible`、`Hidden`、`VeryHidden` です。</span><span class="sxs-lookup"><span data-stu-id="93634-p108">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93634-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93634-177">Relationships</span></span>
| <span data-ttu-id="93634-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93634-178">Relationship</span></span> | <span data-ttu-id="93634-179">型</span><span class="sxs-lookup"><span data-stu-id="93634-179">Type</span></span>   |<span data-ttu-id="93634-180">説明</span><span class="sxs-lookup"><span data-stu-id="93634-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93634-181">charts</span><span class="sxs-lookup"><span data-stu-id="93634-181">charts</span></span>|<span data-ttu-id="93634-182">[Chart](chart.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-182">[Chart](chart.md) collection</span></span>|<span data-ttu-id="93634-p109">ワークシートの一部になっているグラフのコレクションを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93634-p109">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="93634-185">names</span><span class="sxs-lookup"><span data-stu-id="93634-185">names</span></span>|<span data-ttu-id="93634-186">[NamedItem](nameditem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-186">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="93634-p110">ワークシートに関連付けられている名前のコレクションを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93634-p110">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="93634-189">pivotTables</span><span class="sxs-lookup"><span data-stu-id="93634-189">pivotTables</span></span>|<span data-ttu-id="93634-190">[workbookPivotTable](workbookpivottable.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-190">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="93634-191">ワークシートの一部になっているピボットテーブルのコレクション。</span><span class="sxs-lookup"><span data-stu-id="93634-191">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="93634-192">protection</span><span class="sxs-lookup"><span data-stu-id="93634-192">protection</span></span>|[<span data-ttu-id="93634-193">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="93634-193">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="93634-p111">ワークシートのシート保護オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93634-p111">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="93634-196">テーブル</span><span class="sxs-lookup"><span data-stu-id="93634-196">tables</span></span>|<span data-ttu-id="93634-197">[Table](table.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93634-197">[Table](table.md) collection</span></span>|<span data-ttu-id="93634-p112">ワークシートの一部になっているグラフのコレクション。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="93634-p112">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93634-200">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93634-200">JSON representation</span></span>

<span data-ttu-id="93634-201">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="93634-201">Here is a JSON representation of the resource.</span></span>

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
