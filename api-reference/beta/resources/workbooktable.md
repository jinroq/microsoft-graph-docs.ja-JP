---
title: workbookTable リソースの種類
description: Excel の表を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1568cc1f08ded8ffdbac04e040bccefe63e9dd02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963886"
---
# <a name="workbooktable-resource-type"></a><span data-ttu-id="b2694-103">workbookTable リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2694-103">workbookTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2694-104">Excel の表を表します。</span><span class="sxs-lookup"><span data-stu-id="b2694-104">Represents an Excel table.</span></span>

## <a name="methods"></a><span data-ttu-id="b2694-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b2694-105">Methods</span></span>

| <span data-ttu-id="b2694-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b2694-106">Method</span></span>           | <span data-ttu-id="b2694-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b2694-107">Return Type</span></span>    |<span data-ttu-id="b2694-108">説明</span><span class="sxs-lookup"><span data-stu-id="b2694-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2694-109">WorkbookTable を取得する</span><span class="sxs-lookup"><span data-stu-id="b2694-109">Get workbookTable</span></span>](../api/table-get.md) | [<span data-ttu-id="b2694-110">workbookTable</span><span class="sxs-lookup"><span data-stu-id="b2694-110">workbookTable</span></span>](workbooktable.md) |<span data-ttu-id="b2694-111">テーブル オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b2694-111">Read properties and relationships of table object.</span></span>|
|[<span data-ttu-id="b2694-112">WorkbookTableColumn を作成する</span><span class="sxs-lookup"><span data-stu-id="b2694-112">Create workbookTableColumn</span></span>](../api/table-post-columns.md) |[<span data-ttu-id="b2694-113">workbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="b2694-113">workbookTableColumn</span></span>](workbooktablecolumn.md)| <span data-ttu-id="b2694-114">列コレクションに投稿して、新しい TableColumn を作成します。</span><span class="sxs-lookup"><span data-stu-id="b2694-114">Create a new TableColumn by posting to the columns collection.</span></span>|
|[<span data-ttu-id="b2694-115">列を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b2694-115">List columns</span></span>](../api/table-list-columns.md) |<span data-ttu-id="b2694-116">[workbookTableColumn](workbooktablecolumn.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b2694-116">[workbookTableColumn](workbooktablecolumn.md) collection</span></span>| <span data-ttu-id="b2694-117">TableColumn オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2694-117">Get a TableColumn object collection.</span></span>|
|[<span data-ttu-id="b2694-118">WorkbookTableRow を作成する</span><span class="sxs-lookup"><span data-stu-id="b2694-118">Create workbookTableRow</span></span>](../api/table-post-rows.md) |[<span data-ttu-id="b2694-119">workbookTableRow</span><span class="sxs-lookup"><span data-stu-id="b2694-119">workbookTableRow</span></span>](workbooktablerow.md)| <span data-ttu-id="b2694-120">行コレクションに投稿して、新しい TableRow を作成します。</span><span class="sxs-lookup"><span data-stu-id="b2694-120">Create a new TableRow by posting to the rows collection.</span></span>|
|[<span data-ttu-id="b2694-121">行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b2694-121">List rows</span></span>](../api/table-list-rows.md) |<span data-ttu-id="b2694-122">[workbookTableRow](workbooktablerow.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b2694-122">[workbookTableRow](workbooktablerow.md) collection</span></span>| <span data-ttu-id="b2694-123">TableRow オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2694-123">Get a TableRow object collection.</span></span>|
|[<span data-ttu-id="b2694-124">Update</span><span class="sxs-lookup"><span data-stu-id="b2694-124">Update</span></span>](../api/table-update.md) | [<span data-ttu-id="b2694-125">workbookTable</span><span class="sxs-lookup"><span data-stu-id="b2694-125">workbookTable</span></span>](workbooktable.md)   |<span data-ttu-id="b2694-126">テーブル オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b2694-126">Update Table object.</span></span> |
|[<span data-ttu-id="b2694-127">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="b2694-127">Databodyrange</span></span>](../api/table-databodyrange.md)|[<span data-ttu-id="b2694-128">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b2694-128">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b2694-129">テーブルのデータ本体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2694-129">Gets the range object associated with the data body of the table.</span></span>|
|[<span data-ttu-id="b2694-130">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="b2694-130">Headerrowrange</span></span>](../api/table-headerrowrange.md)|[<span data-ttu-id="b2694-131">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b2694-131">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b2694-132">テーブルのヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2694-132">Gets the range object associated with header row of the table.</span></span>|
|[<span data-ttu-id="b2694-133">Range</span><span class="sxs-lookup"><span data-stu-id="b2694-133">Range</span></span>](../api/table-range.md)|[<span data-ttu-id="b2694-134">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b2694-134">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b2694-135">テーブル全体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2694-135">Gets the range object associated with the entire table.</span></span>|
|[<span data-ttu-id="b2694-136">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="b2694-136">Totalrowrange</span></span>](../api/table-totalrowrange.md)|[<span data-ttu-id="b2694-137">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b2694-137">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b2694-138">テーブルの集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2694-138">Gets the range object associated with totals row of the table.</span></span>|
|[<span data-ttu-id="b2694-139">Clearfilters</span><span class="sxs-lookup"><span data-stu-id="b2694-139">Clearfilters</span></span>](../api/table-clearfilters.md)|<span data-ttu-id="b2694-140">なし</span><span class="sxs-lookup"><span data-stu-id="b2694-140">None</span></span>|<span data-ttu-id="b2694-141">現在テーブルに適用されているすべてのフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="b2694-141">Clears all the filters currently applied on the table.</span></span>|
|[<span data-ttu-id="b2694-142">Converttorange</span><span class="sxs-lookup"><span data-stu-id="b2694-142">Converttorange</span></span>](../api/table-converttorange.md)|[<span data-ttu-id="b2694-143">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b2694-143">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b2694-p101">テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="b2694-p101">Converts the table into a normal range of cells. All data is preserved.</span></span>|
|[<span data-ttu-id="b2694-146">Delete</span><span class="sxs-lookup"><span data-stu-id="b2694-146">Delete</span></span>](../api/table-delete.md)|<span data-ttu-id="b2694-147">None</span><span class="sxs-lookup"><span data-stu-id="b2694-147">None</span></span>|<span data-ttu-id="b2694-148">テーブルを削除します。</span><span class="sxs-lookup"><span data-stu-id="b2694-148">Deletes the table.</span></span>|
|[<span data-ttu-id="b2694-149">Reapplyfilters</span><span class="sxs-lookup"><span data-stu-id="b2694-149">Reapplyfilters</span></span>](../api/table-reapplyfilters.md)|<span data-ttu-id="b2694-150">なし</span><span class="sxs-lookup"><span data-stu-id="b2694-150">None</span></span>|<span data-ttu-id="b2694-151">現在テーブルにあるすべてのフィルターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="b2694-151">Reapplies all the filters currently on the table.</span></span>|
|[<span data-ttu-id="b2694-152">List</span><span class="sxs-lookup"><span data-stu-id="b2694-152">List</span></span>](../api/table-list.md) | <span data-ttu-id="b2694-153">[workbookTable](workbooktable.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b2694-153">[workbookTable](workbooktable.md) collection</span></span> |<span data-ttu-id="b2694-154">テーブル オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b2694-154">Get table object collection.</span></span> |
|[<span data-ttu-id="b2694-155">Add</span><span class="sxs-lookup"><span data-stu-id="b2694-155">Add</span></span>](../api/tablecollection-add.md)|[<span data-ttu-id="b2694-156">workbookTable</span><span class="sxs-lookup"><span data-stu-id="b2694-156">workbookTable</span></span>](workbooktable.md)|<span data-ttu-id="b2694-p102">新しいテーブルを作成します。範囲のソース アドレスにより、テーブルが追加されるワークシートが判断されます。テーブルが追加できない場合 (たとえば、アドレスが無効な場合や、テーブルが別のテーブルと重複している場合) は、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="b2694-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2694-160">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2694-160">Properties</span></span>
| <span data-ttu-id="b2694-161">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2694-161">Property</span></span>     | <span data-ttu-id="b2694-162">型</span><span class="sxs-lookup"><span data-stu-id="b2694-162">Type</span></span>   |<span data-ttu-id="b2694-163">説明</span><span class="sxs-lookup"><span data-stu-id="b2694-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2694-164">id</span><span class="sxs-lookup"><span data-stu-id="b2694-164">id</span></span>|<span data-ttu-id="b2694-165">string</span><span class="sxs-lookup"><span data-stu-id="b2694-165">string</span></span>|<span data-ttu-id="b2694-166">指定されたブックのテーブルを一意に識別する値を返します。</span><span class="sxs-lookup"><span data-stu-id="b2694-166">Returns a value that uniquely identifies the table in a given workbook.</span></span> <span data-ttu-id="b2694-167">識別子の値は、テーブルの名前が変更された場合も変わりません。</span><span class="sxs-lookup"><span data-stu-id="b2694-167">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="b2694-168">このプロパティは符号化文字列値として解釈し、その他の型に解析すべきではありません。</span><span class="sxs-lookup"><span data-stu-id="b2694-168">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="b2694-169">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b2694-169">Read-only.</span></span>|
|<span data-ttu-id="b2694-170">name</span><span class="sxs-lookup"><span data-stu-id="b2694-170">name</span></span>|<span data-ttu-id="b2694-171">string</span><span class="sxs-lookup"><span data-stu-id="b2694-171">string</span></span>|<span data-ttu-id="b2694-172">テーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="b2694-172">Name of the table.</span></span>|
|<span data-ttu-id="b2694-173">showHeaders</span><span class="sxs-lookup"><span data-stu-id="b2694-173">showHeaders</span></span>|<span data-ttu-id="b2694-174">ブール値</span><span class="sxs-lookup"><span data-stu-id="b2694-174">boolean</span></span>|<span data-ttu-id="b2694-p104">ヘッダー行を表示するかどうかを示します。この値によって、ヘッダー行の表示または削除を設定できます。</span><span class="sxs-lookup"><span data-stu-id="b2694-p104">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="b2694-177">showTotals</span><span class="sxs-lookup"><span data-stu-id="b2694-177">showTotals</span></span>|<span data-ttu-id="b2694-178">boolean</span><span class="sxs-lookup"><span data-stu-id="b2694-178">boolean</span></span>|<span data-ttu-id="b2694-p105">集計行を表示するかどうかを示します。この値によって、集計行の表示または削除を設定できます。</span><span class="sxs-lookup"><span data-stu-id="b2694-p105">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="b2694-181">style</span><span class="sxs-lookup"><span data-stu-id="b2694-181">style</span></span>|<span data-ttu-id="b2694-182">string</span><span class="sxs-lookup"><span data-stu-id="b2694-182">string</span></span>|<span data-ttu-id="b2694-p106">テーブル スタイルを表す定数値。使用可能な値は次のとおりです。TableStyleLight1 から TableStyleLight21、TableStyleMedium1 から TableStyleMedium28、TableStyleStyleDark1 から TableStyleStyleDark11。ブックに存在するカスタムのユーザー定義スタイルも指定できます。</span><span class="sxs-lookup"><span data-stu-id="b2694-p106">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|
|<span data-ttu-id="b2694-186">highlightFirstColumn</span><span class="sxs-lookup"><span data-stu-id="b2694-186">highlightFirstColumn</span></span>|<span data-ttu-id="b2694-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2694-187">Boolean</span></span>|<span data-ttu-id="b2694-188">最初の列に特別な書式設定が含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b2694-188">Indicates whether the first column contains special formatting.</span></span>   |
|<span data-ttu-id="b2694-189">highlightLastColumn</span><span class="sxs-lookup"><span data-stu-id="b2694-189">highlightLastColumn</span></span>|<span data-ttu-id="b2694-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2694-190">Boolean</span></span>|<span data-ttu-id="b2694-191">最後の列に特別な書式設定が含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b2694-191">Indicates whether the last column contains special formatting.</span></span> |
|<span data-ttu-id="b2694-192">showBandedColumns</span><span class="sxs-lookup"><span data-stu-id="b2694-192">showBandedColumns</span></span>|<span data-ttu-id="b2694-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2694-193">Boolean</span></span>|<span data-ttu-id="b2694-194">テーブルを見やすくするため、奇数列を偶数列とは異なる方法で強調表示する書式設定にして、列を縞模様で表示するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b2694-194">Indicates whether the columns show banded formatting in which odd columns are highlighted differently from even ones to make reading the table easier.</span></span>   |
|<span data-ttu-id="b2694-195">showBandedRows</span><span class="sxs-lookup"><span data-stu-id="b2694-195">showBandedRows</span></span>|<span data-ttu-id="b2694-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2694-196">Boolean</span></span>|<span data-ttu-id="b2694-197">テーブルを見やすくするため、奇数行を偶数行とは異なる方法で強調表示する書式設定にして、行を縞模様で表示するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b2694-197">Indicates whether the rows show banded formatting in which odd rows are highlighted differently from even ones to make reading the table easier.</span></span>    |
|<span data-ttu-id="b2694-198">showFilterButton</span><span class="sxs-lookup"><span data-stu-id="b2694-198">showFilterButton</span></span>|<span data-ttu-id="b2694-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2694-199">Boolean</span></span>|<span data-ttu-id="b2694-p107">フィルター ボタンを各列のヘッダーの上部に表示するかどうかを示します。これは、テーブルにヘッダー行が含まれている場合のみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="b2694-p107">Indicates whether the filter buttons are visible at the top of each column header. Setting this is only allowed if the table contains a header row.</span></span>   |
|<span data-ttu-id="b2694-202">legacyId</span><span class="sxs-lookup"><span data-stu-id="b2694-202">legacyId</span></span>|<span data-ttu-id="b2694-203">String</span><span class="sxs-lookup"><span data-stu-id="b2694-203">String</span></span>|<span data-ttu-id="b2694-204">以前の Excle クライアントで使用されていたレガシ Id です。</span><span class="sxs-lookup"><span data-stu-id="b2694-204">Legacy Id used in older Excle clients.</span></span> <span data-ttu-id="b2694-205">識別子の値は、テーブルの名前が変更された場合も変わりません。</span><span class="sxs-lookup"><span data-stu-id="b2694-205">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="b2694-206">このプロパティは符号化文字列値として解釈し、その他の型に解析すべきではありません。</span><span class="sxs-lookup"><span data-stu-id="b2694-206">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="b2694-207">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2694-207">Read-only.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="b2694-208">関係</span><span class="sxs-lookup"><span data-stu-id="b2694-208">Relationships</span></span>
| <span data-ttu-id="b2694-209">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2694-209">Relationship</span></span> | <span data-ttu-id="b2694-210">型</span><span class="sxs-lookup"><span data-stu-id="b2694-210">Type</span></span>   |<span data-ttu-id="b2694-211">説明</span><span class="sxs-lookup"><span data-stu-id="b2694-211">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2694-212">columns</span><span class="sxs-lookup"><span data-stu-id="b2694-212">columns</span></span>|<span data-ttu-id="b2694-213">[workbookTableColumn](workbooktablecolumn.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b2694-213">[workbookTableColumn](workbooktablecolumn.md) collection</span></span>|<span data-ttu-id="b2694-p109">テーブルに含まれるすべての列のコレクションを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2694-p109">Represents a collection of all the columns in the table. Read-only.</span></span>|
|<span data-ttu-id="b2694-216">rows</span><span class="sxs-lookup"><span data-stu-id="b2694-216">rows</span></span>|<span data-ttu-id="b2694-217">[workbookTableRow](workbooktablerow.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b2694-217">[workbookTableRow](workbooktablerow.md) collection</span></span>|<span data-ttu-id="b2694-p110">テーブルに含まれるすべての行のコレクションを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2694-p110">Represents a collection of all the rows in the table. Read-only.</span></span>|
|<span data-ttu-id="b2694-220">sort</span><span class="sxs-lookup"><span data-stu-id="b2694-220">sort</span></span>|[<span data-ttu-id="b2694-221">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="b2694-221">workbookTableSort</span></span>](workbooktablesort.md)|<span data-ttu-id="b2694-p111">テーブル内の並べ替えを表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b2694-p111">Represents the sorting for the table. Read-only.</span></span>|
|<span data-ttu-id="b2694-224">worksheet</span><span class="sxs-lookup"><span data-stu-id="b2694-224">worksheet</span></span>|[<span data-ttu-id="b2694-225">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="b2694-225">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="b2694-p112">現在のテーブルを含んでいるワークシート。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2694-p112">The worksheet containing the current table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2694-228">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2694-228">JSON representation</span></span>

<span data-ttu-id="b2694-229">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2694-229">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTable"
}-->

```json
{
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "id": "String (identifier)",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String",
  "legacyId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
