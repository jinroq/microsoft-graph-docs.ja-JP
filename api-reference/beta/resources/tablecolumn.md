---
title: TableColumn リソースの種類
description: テーブル内にある 1 つの列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9f70b5363ccc7552975db8f2396af705d8bf1557
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565612"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="54eef-103">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54eef-103">TableColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54eef-104">テーブル内にある 1 つの列を表します。</span><span class="sxs-lookup"><span data-stu-id="54eef-104">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="54eef-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="54eef-105">Methods</span></span>

| <span data-ttu-id="54eef-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="54eef-106">Method</span></span>           | <span data-ttu-id="54eef-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="54eef-107">Return Type</span></span>    |<span data-ttu-id="54eef-108">説明</span><span class="sxs-lookup"><span data-stu-id="54eef-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54eef-109">TableColumn を取得する</span><span class="sxs-lookup"><span data-stu-id="54eef-109">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="54eef-110">TableColumn</span><span class="sxs-lookup"><span data-stu-id="54eef-110">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="54eef-111">tableColumn オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="54eef-111">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="54eef-112">Update</span><span class="sxs-lookup"><span data-stu-id="54eef-112">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="54eef-113">TableColumn</span><span class="sxs-lookup"><span data-stu-id="54eef-113">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="54eef-114">TableColumn オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="54eef-114">Update TableColumn object.</span></span> |
|[<span data-ttu-id="54eef-115">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="54eef-115">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="54eef-116">Range</span><span class="sxs-lookup"><span data-stu-id="54eef-116">Range</span></span>](range.md)|<span data-ttu-id="54eef-117">列のデータ本体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="54eef-117">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="54eef-118">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="54eef-118">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="54eef-119">Range</span><span class="sxs-lookup"><span data-stu-id="54eef-119">Range</span></span>](range.md)|<span data-ttu-id="54eef-120">列のヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="54eef-120">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="54eef-121">Range</span><span class="sxs-lookup"><span data-stu-id="54eef-121">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="54eef-122">Range</span><span class="sxs-lookup"><span data-stu-id="54eef-122">Range</span></span>](range.md)|<span data-ttu-id="54eef-123">列全体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="54eef-123">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="54eef-124">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="54eef-124">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="54eef-125">Range</span><span class="sxs-lookup"><span data-stu-id="54eef-125">Range</span></span>](range.md)|<span data-ttu-id="54eef-126">列の集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="54eef-126">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="54eef-127">削除</span><span class="sxs-lookup"><span data-stu-id="54eef-127">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="54eef-128">なし</span><span class="sxs-lookup"><span data-stu-id="54eef-128">None</span></span>|<span data-ttu-id="54eef-129">テーブルから列を削除します。</span><span class="sxs-lookup"><span data-stu-id="54eef-129">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="54eef-130">List</span><span class="sxs-lookup"><span data-stu-id="54eef-130">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="54eef-131">[TableColumn](tablecolumn.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="54eef-131">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="54eef-132">tableColumn オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="54eef-132">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="54eef-133">Itemat</span><span class="sxs-lookup"><span data-stu-id="54eef-133">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="54eef-134">TableColumn</span><span class="sxs-lookup"><span data-stu-id="54eef-134">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="54eef-135">コレクション内の位置に基づいて列を取得します。</span><span class="sxs-lookup"><span data-stu-id="54eef-135">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="54eef-136">Add</span><span class="sxs-lookup"><span data-stu-id="54eef-136">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="54eef-137">TableColumn</span><span class="sxs-lookup"><span data-stu-id="54eef-137">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="54eef-138">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="54eef-138">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="54eef-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54eef-139">Properties</span></span>
| <span data-ttu-id="54eef-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54eef-140">Property</span></span>     | <span data-ttu-id="54eef-141">型</span><span class="sxs-lookup"><span data-stu-id="54eef-141">Type</span></span>   |<span data-ttu-id="54eef-142">説明</span><span class="sxs-lookup"><span data-stu-id="54eef-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54eef-143">id</span><span class="sxs-lookup"><span data-stu-id="54eef-143">id</span></span>|<span data-ttu-id="54eef-144">int</span><span class="sxs-lookup"><span data-stu-id="54eef-144">int</span></span>|<span data-ttu-id="54eef-p101">テーブル内の列を識別する一意のキーを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54eef-p101">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="54eef-147">index</span><span class="sxs-lookup"><span data-stu-id="54eef-147">index</span></span>|<span data-ttu-id="54eef-148">int</span><span class="sxs-lookup"><span data-stu-id="54eef-148">int</span></span>|<span data-ttu-id="54eef-p102">テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54eef-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="54eef-152">name</span><span class="sxs-lookup"><span data-stu-id="54eef-152">name</span></span>|<span data-ttu-id="54eef-153">string</span><span class="sxs-lookup"><span data-stu-id="54eef-153">string</span></span>|<span data-ttu-id="54eef-p103">テーブル列の名前を取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54eef-p103">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="54eef-156">values</span><span class="sxs-lookup"><span data-stu-id="54eef-156">values</span></span>|<span data-ttu-id="54eef-157">json</span><span class="sxs-lookup"><span data-stu-id="54eef-157">json</span></span>|<span data-ttu-id="54eef-p104">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="54eef-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54eef-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54eef-161">Relationships</span></span>
| <span data-ttu-id="54eef-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54eef-162">Relationship</span></span> | <span data-ttu-id="54eef-163">型</span><span class="sxs-lookup"><span data-stu-id="54eef-163">Type</span></span>   |<span data-ttu-id="54eef-164">説明</span><span class="sxs-lookup"><span data-stu-id="54eef-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54eef-165">フィルター</span><span class="sxs-lookup"><span data-stu-id="54eef-165">filter</span></span>|[<span data-ttu-id="54eef-166">フィルター</span><span class="sxs-lookup"><span data-stu-id="54eef-166">Filter</span></span>](filter.md)|<span data-ttu-id="54eef-p105">列に適用されるフィルターを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="54eef-p105">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54eef-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54eef-169">JSON representation</span></span>

<span data-ttu-id="54eef-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54eef-170">Here is a JSON representation of the resource.</span></span>

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
