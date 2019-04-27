---
title: workbookTableColumn リソースの種類
description: テーブル内にある 1 つの列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: af0472d5cfdd95af731a4d9280b90d3ed1b44621
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348899"
---
# <a name="workbooktablecolumn-resource-type"></a><span data-ttu-id="d66ee-103">workbookTableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d66ee-103">workbookTableColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d66ee-104">テーブル内にある 1 つの列を表します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-104">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="d66ee-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d66ee-105">Methods</span></span>

| <span data-ttu-id="d66ee-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d66ee-106">Method</span></span>           | <span data-ttu-id="d66ee-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d66ee-107">Return Type</span></span>    |<span data-ttu-id="d66ee-108">説明</span><span class="sxs-lookup"><span data-stu-id="d66ee-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d66ee-109">TableColumn を取得する</span><span class="sxs-lookup"><span data-stu-id="d66ee-109">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="d66ee-110">workbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d66ee-110">workbookTableColumn</span></span>](workbooktablecolumn.md) |<span data-ttu-id="d66ee-111">tableColumn オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d66ee-111">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="d66ee-112">Update</span><span class="sxs-lookup"><span data-stu-id="d66ee-112">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="d66ee-113">workbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d66ee-113">workbookTableColumn</span></span>](workbooktablecolumn.md) |<span data-ttu-id="d66ee-114">TableColumn オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-114">Update TableColumn object.</span></span> |
|[<span data-ttu-id="d66ee-115">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="d66ee-115">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="d66ee-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d66ee-116">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d66ee-117">列のデータ本体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-117">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="d66ee-118">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="d66ee-118">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="d66ee-119">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d66ee-119">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d66ee-120">列のヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-120">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="d66ee-121">Range</span><span class="sxs-lookup"><span data-stu-id="d66ee-121">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="d66ee-122">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d66ee-122">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d66ee-123">列全体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-123">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="d66ee-124">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="d66ee-124">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="d66ee-125">workbookRange</span><span class="sxs-lookup"><span data-stu-id="d66ee-125">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="d66ee-126">列の集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-126">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="d66ee-127">Delete</span><span class="sxs-lookup"><span data-stu-id="d66ee-127">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="d66ee-128">なし</span><span class="sxs-lookup"><span data-stu-id="d66ee-128">None</span></span>|<span data-ttu-id="d66ee-129">テーブルから列を削除します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-129">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="d66ee-130">List</span><span class="sxs-lookup"><span data-stu-id="d66ee-130">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="d66ee-131">[workbookTableColumn](workbooktablecolumn.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d66ee-131">[workbookTableColumn](workbooktablecolumn.md) collection</span></span> |<span data-ttu-id="d66ee-132">tableColumn オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-132">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="d66ee-133">Itemat</span><span class="sxs-lookup"><span data-stu-id="d66ee-133">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="d66ee-134">workbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d66ee-134">workbookTableColumn</span></span>](workbooktablecolumn.md)|<span data-ttu-id="d66ee-135">コレクション内の位置に基づいて列を取得します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-135">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="d66ee-136">Add</span><span class="sxs-lookup"><span data-stu-id="d66ee-136">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="d66ee-137">workbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d66ee-137">workbookTableColumn</span></span>](workbooktablecolumn.md)|<span data-ttu-id="d66ee-138">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-138">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="d66ee-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d66ee-139">Properties</span></span>
| <span data-ttu-id="d66ee-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d66ee-140">Property</span></span>     | <span data-ttu-id="d66ee-141">種類</span><span class="sxs-lookup"><span data-stu-id="d66ee-141">Type</span></span>   |<span data-ttu-id="d66ee-142">説明</span><span class="sxs-lookup"><span data-stu-id="d66ee-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d66ee-143">id</span><span class="sxs-lookup"><span data-stu-id="d66ee-143">id</span></span>|<span data-ttu-id="d66ee-144">int</span><span class="sxs-lookup"><span data-stu-id="d66ee-144">int</span></span>|<span data-ttu-id="d66ee-p101">テーブル内の列を識別する一意のキーを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d66ee-p101">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="d66ee-147">index</span><span class="sxs-lookup"><span data-stu-id="d66ee-147">index</span></span>|<span data-ttu-id="d66ee-148">int</span><span class="sxs-lookup"><span data-stu-id="d66ee-148">int</span></span>|<span data-ttu-id="d66ee-p102">テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d66ee-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="d66ee-152">name</span><span class="sxs-lookup"><span data-stu-id="d66ee-152">name</span></span>|<span data-ttu-id="d66ee-153">string</span><span class="sxs-lookup"><span data-stu-id="d66ee-153">string</span></span>|<span data-ttu-id="d66ee-p103">テーブル列の名前を取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d66ee-p103">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="d66ee-156">values</span><span class="sxs-lookup"><span data-stu-id="d66ee-156">values</span></span>|<span data-ttu-id="d66ee-157">Json</span><span class="sxs-lookup"><span data-stu-id="d66ee-157">Json</span></span>|<span data-ttu-id="d66ee-p104">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="d66ee-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d66ee-161">関係</span><span class="sxs-lookup"><span data-stu-id="d66ee-161">Relationships</span></span>
| <span data-ttu-id="d66ee-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d66ee-162">Relationship</span></span> | <span data-ttu-id="d66ee-163">型</span><span class="sxs-lookup"><span data-stu-id="d66ee-163">Type</span></span>   |<span data-ttu-id="d66ee-164">説明</span><span class="sxs-lookup"><span data-stu-id="d66ee-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d66ee-165">フィルター</span><span class="sxs-lookup"><span data-stu-id="d66ee-165">filter</span></span>|[<span data-ttu-id="d66ee-166">workbookFilter</span><span class="sxs-lookup"><span data-stu-id="d66ee-166">workbookFilter</span></span>](workbookfilter.md)|<span data-ttu-id="d66ee-p105">列に適用されるフィルターを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d66ee-p105">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d66ee-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d66ee-169">JSON representation</span></span>

<span data-ttu-id="d66ee-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d66ee-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
