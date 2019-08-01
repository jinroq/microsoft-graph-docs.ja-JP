---
title: TableColumn リソースの種類
description: テーブル内にある 1 つの列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 095317b36c5242cd5e78f58192a242bd4e1f2993
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033979"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="0ac16-103">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ac16-103">TableColumn resource type</span></span>

<span data-ttu-id="0ac16-104">テーブル内にある 1 つの列を表します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-104">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="0ac16-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0ac16-105">Methods</span></span>

| <span data-ttu-id="0ac16-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0ac16-106">Method</span></span>           | <span data-ttu-id="0ac16-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0ac16-107">Return Type</span></span>    |<span data-ttu-id="0ac16-108">説明</span><span class="sxs-lookup"><span data-stu-id="0ac16-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ac16-109">TableColumn を取得する</span><span class="sxs-lookup"><span data-stu-id="0ac16-109">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="0ac16-110">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="0ac16-110">WorkbookTableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="0ac16-111">tableColumn オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0ac16-111">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="0ac16-112">Update</span><span class="sxs-lookup"><span data-stu-id="0ac16-112">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="0ac16-113">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="0ac16-113">WorkbookTableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="0ac16-114">TableColumn オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-114">Update TableColumn object.</span></span> |
|[<span data-ttu-id="0ac16-115">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="0ac16-115">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="0ac16-116">Range</span><span class="sxs-lookup"><span data-stu-id="0ac16-116">Range</span></span>](range.md)|<span data-ttu-id="0ac16-117">列のデータ本体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-117">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="0ac16-118">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="0ac16-118">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="0ac16-119">Range</span><span class="sxs-lookup"><span data-stu-id="0ac16-119">Range</span></span>](range.md)|<span data-ttu-id="0ac16-120">列のヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-120">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="0ac16-121">Range</span><span class="sxs-lookup"><span data-stu-id="0ac16-121">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="0ac16-122">Range</span><span class="sxs-lookup"><span data-stu-id="0ac16-122">Range</span></span>](range.md)|<span data-ttu-id="0ac16-123">列全体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-123">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="0ac16-124">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="0ac16-124">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="0ac16-125">Range</span><span class="sxs-lookup"><span data-stu-id="0ac16-125">Range</span></span>](range.md)|<span data-ttu-id="0ac16-126">列の集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-126">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="0ac16-127">Delete</span><span class="sxs-lookup"><span data-stu-id="0ac16-127">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="0ac16-128">None</span><span class="sxs-lookup"><span data-stu-id="0ac16-128">None</span></span>|<span data-ttu-id="0ac16-129">テーブルから列を削除します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-129">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="0ac16-130">List</span><span class="sxs-lookup"><span data-stu-id="0ac16-130">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="0ac16-131">[WorkbookTableColumn](tablecolumn.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0ac16-131">[WorkbookTableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="0ac16-132">tableColumn オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-132">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="0ac16-133">Itemat</span><span class="sxs-lookup"><span data-stu-id="0ac16-133">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="0ac16-134">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="0ac16-134">WorkbookTableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="0ac16-135">コレクション内の位置に基づいて列を取得します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-135">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="0ac16-136">Add</span><span class="sxs-lookup"><span data-stu-id="0ac16-136">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="0ac16-137">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="0ac16-137">WorkbookTableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="0ac16-138">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-138">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ac16-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ac16-139">Properties</span></span>
| <span data-ttu-id="0ac16-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ac16-140">Property</span></span>     | <span data-ttu-id="0ac16-141">型</span><span class="sxs-lookup"><span data-stu-id="0ac16-141">Type</span></span>   |<span data-ttu-id="0ac16-142">説明</span><span class="sxs-lookup"><span data-stu-id="0ac16-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ac16-143">id</span><span class="sxs-lookup"><span data-stu-id="0ac16-143">id</span></span>|<span data-ttu-id="0ac16-144">string</span><span class="sxs-lookup"><span data-stu-id="0ac16-144">string</span></span>|<span data-ttu-id="0ac16-145">テーブル内の列を識別する一意のキーを返します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-145">Returns a unique key that identifies the column within the table.</span></span> <span data-ttu-id="0ac16-146">このプロパティは符号化文字列値として解釈し、その他の型に解析すべきではありません。</span><span class="sxs-lookup"><span data-stu-id="0ac16-146">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="0ac16-147">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0ac16-147">Read-only.</span></span>|
|<span data-ttu-id="0ac16-148">index</span><span class="sxs-lookup"><span data-stu-id="0ac16-148">index</span></span>|<span data-ttu-id="0ac16-149">int</span><span class="sxs-lookup"><span data-stu-id="0ac16-149">int</span></span>|<span data-ttu-id="0ac16-p102">テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0ac16-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="0ac16-153">name</span><span class="sxs-lookup"><span data-stu-id="0ac16-153">name</span></span>|<span data-ttu-id="0ac16-154">string</span><span class="sxs-lookup"><span data-stu-id="0ac16-154">string</span></span>|<span data-ttu-id="0ac16-p103">テーブル列の名前を取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0ac16-p103">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="0ac16-157">values</span><span class="sxs-lookup"><span data-stu-id="0ac16-157">values</span></span>|<span data-ttu-id="0ac16-158">Json</span><span class="sxs-lookup"><span data-stu-id="0ac16-158">Json</span></span>|<span data-ttu-id="0ac16-p104">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="0ac16-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ac16-162">関係</span><span class="sxs-lookup"><span data-stu-id="0ac16-162">Relationships</span></span>
| <span data-ttu-id="0ac16-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0ac16-163">Relationship</span></span> | <span data-ttu-id="0ac16-164">型</span><span class="sxs-lookup"><span data-stu-id="0ac16-164">Type</span></span>   |<span data-ttu-id="0ac16-165">説明</span><span class="sxs-lookup"><span data-stu-id="0ac16-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ac16-166">フィルター</span><span class="sxs-lookup"><span data-stu-id="0ac16-166">filter</span></span>|[<span data-ttu-id="0ac16-167">WorkbookFilter</span><span class="sxs-lookup"><span data-stu-id="0ac16-167">WorkbookFilter</span></span>](filter.md)|<span data-ttu-id="0ac16-p105">列に適用されるフィルターを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0ac16-p105">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ac16-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ac16-170">JSON representation</span></span>

<span data-ttu-id="0ac16-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0ac16-171">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
