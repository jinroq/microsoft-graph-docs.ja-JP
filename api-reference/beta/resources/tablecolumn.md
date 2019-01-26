---
title: TableColumn リソースの種類
description: テーブル内にある 1 つの列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 10c5dbffcb5460ea029368a4c9b6dcfb6c21f256
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574664"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="1b9a6-103">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1b9a6-103">TableColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b9a6-104">テーブル内にある 1 つの列を表します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-104">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="1b9a6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1b9a6-105">Methods</span></span>

| <span data-ttu-id="1b9a6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1b9a6-106">Method</span></span>           | <span data-ttu-id="1b9a6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1b9a6-107">Return Type</span></span>    |<span data-ttu-id="1b9a6-108">説明</span><span class="sxs-lookup"><span data-stu-id="1b9a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b9a6-109">TableColumn を取得する</span><span class="sxs-lookup"><span data-stu-id="1b9a6-109">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="1b9a6-110">TableColumn</span><span class="sxs-lookup"><span data-stu-id="1b9a6-110">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="1b9a6-111">tableColumn オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-111">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="1b9a6-112">Update</span><span class="sxs-lookup"><span data-stu-id="1b9a6-112">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="1b9a6-113">TableColumn</span><span class="sxs-lookup"><span data-stu-id="1b9a6-113">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="1b9a6-114">TableColumn オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-114">Update TableColumn object.</span></span> |
|[<span data-ttu-id="1b9a6-115">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="1b9a6-115">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="1b9a6-116">Range</span><span class="sxs-lookup"><span data-stu-id="1b9a6-116">Range</span></span>](range.md)|<span data-ttu-id="1b9a6-117">列のデータ本体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-117">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="1b9a6-118">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="1b9a6-118">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="1b9a6-119">Range</span><span class="sxs-lookup"><span data-stu-id="1b9a6-119">Range</span></span>](range.md)|<span data-ttu-id="1b9a6-120">列のヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-120">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="1b9a6-121">Range</span><span class="sxs-lookup"><span data-stu-id="1b9a6-121">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="1b9a6-122">Range</span><span class="sxs-lookup"><span data-stu-id="1b9a6-122">Range</span></span>](range.md)|<span data-ttu-id="1b9a6-123">列全体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-123">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="1b9a6-124">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="1b9a6-124">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="1b9a6-125">Range</span><span class="sxs-lookup"><span data-stu-id="1b9a6-125">Range</span></span>](range.md)|<span data-ttu-id="1b9a6-126">列の集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-126">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="1b9a6-127">Delete</span><span class="sxs-lookup"><span data-stu-id="1b9a6-127">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="1b9a6-128">なし</span><span class="sxs-lookup"><span data-stu-id="1b9a6-128">None</span></span>|<span data-ttu-id="1b9a6-129">テーブルから列を削除します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-129">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="1b9a6-130">List</span><span class="sxs-lookup"><span data-stu-id="1b9a6-130">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="1b9a6-131">[TableColumn](tablecolumn.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1b9a6-131">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="1b9a6-132">tableColumn オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-132">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="1b9a6-133">Itemat</span><span class="sxs-lookup"><span data-stu-id="1b9a6-133">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="1b9a6-134">TableColumn</span><span class="sxs-lookup"><span data-stu-id="1b9a6-134">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="1b9a6-135">コレクション内の位置に基づいて列を取得します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-135">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="1b9a6-136">Add</span><span class="sxs-lookup"><span data-stu-id="1b9a6-136">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="1b9a6-137">TableColumn</span><span class="sxs-lookup"><span data-stu-id="1b9a6-137">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="1b9a6-138">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-138">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b9a6-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b9a6-139">Properties</span></span>
| <span data-ttu-id="1b9a6-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b9a6-140">Property</span></span>     | <span data-ttu-id="1b9a6-141">型</span><span class="sxs-lookup"><span data-stu-id="1b9a6-141">Type</span></span>   |<span data-ttu-id="1b9a6-142">説明</span><span class="sxs-lookup"><span data-stu-id="1b9a6-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b9a6-143">id</span><span class="sxs-lookup"><span data-stu-id="1b9a6-143">id</span></span>|<span data-ttu-id="1b9a6-144">int</span><span class="sxs-lookup"><span data-stu-id="1b9a6-144">int</span></span>|<span data-ttu-id="1b9a6-p101">テーブル内の列を識別する一意のキーを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-p101">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="1b9a6-147">index</span><span class="sxs-lookup"><span data-stu-id="1b9a6-147">index</span></span>|<span data-ttu-id="1b9a6-148">int</span><span class="sxs-lookup"><span data-stu-id="1b9a6-148">int</span></span>|<span data-ttu-id="1b9a6-p102">テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="1b9a6-152">name</span><span class="sxs-lookup"><span data-stu-id="1b9a6-152">name</span></span>|<span data-ttu-id="1b9a6-153">文字列</span><span class="sxs-lookup"><span data-stu-id="1b9a6-153">string</span></span>|<span data-ttu-id="1b9a6-p103">テーブル列の名前を取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-p103">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="1b9a6-156">values</span><span class="sxs-lookup"><span data-stu-id="1b9a6-156">values</span></span>|<span data-ttu-id="1b9a6-157">Json</span><span class="sxs-lookup"><span data-stu-id="1b9a6-157">Json</span></span>|<span data-ttu-id="1b9a6-p104">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b9a6-161">関係</span><span class="sxs-lookup"><span data-stu-id="1b9a6-161">Relationships</span></span>
| <span data-ttu-id="1b9a6-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1b9a6-162">Relationship</span></span> | <span data-ttu-id="1b9a6-163">型</span><span class="sxs-lookup"><span data-stu-id="1b9a6-163">Type</span></span>   |<span data-ttu-id="1b9a6-164">説明</span><span class="sxs-lookup"><span data-stu-id="1b9a6-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b9a6-165">filter</span><span class="sxs-lookup"><span data-stu-id="1b9a6-165">filter</span></span>|[<span data-ttu-id="1b9a6-166">Filter</span><span class="sxs-lookup"><span data-stu-id="1b9a6-166">Filter</span></span>](filter.md)|<span data-ttu-id="1b9a6-p105">列に適用されるフィルターを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-p105">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b9a6-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1b9a6-169">JSON representation</span></span>

<span data-ttu-id="1b9a6-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1b9a6-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
