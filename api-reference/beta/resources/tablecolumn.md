---
title: TableColumn リソースの種類
description: テーブル内にある 1 つの列を表します。
ms.openlocfilehash: 0195bde59ee2116b064b47b9659f682877efc16b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070019"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="32887-103">TableColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32887-103">TableColumn resource type</span></span>

> <span data-ttu-id="32887-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32887-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32887-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32887-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32887-106">テーブル内にある 1 つの列を表します。</span><span class="sxs-lookup"><span data-stu-id="32887-106">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="32887-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="32887-107">Methods</span></span>

| <span data-ttu-id="32887-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="32887-108">Method</span></span>           | <span data-ttu-id="32887-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="32887-109">Return Type</span></span>    |<span data-ttu-id="32887-110">説明</span><span class="sxs-lookup"><span data-stu-id="32887-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32887-111">TableColumn を取得する</span><span class="sxs-lookup"><span data-stu-id="32887-111">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="32887-112">TableColumn</span><span class="sxs-lookup"><span data-stu-id="32887-112">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="32887-113">tableColumn オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="32887-113">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="32887-114">Update</span><span class="sxs-lookup"><span data-stu-id="32887-114">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="32887-115">TableColumn</span><span class="sxs-lookup"><span data-stu-id="32887-115">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="32887-116">TableColumn オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="32887-116">Update TableColumn object.</span></span> |
|[<span data-ttu-id="32887-117">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="32887-117">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="32887-118">Range</span><span class="sxs-lookup"><span data-stu-id="32887-118">Range</span></span>](range.md)|<span data-ttu-id="32887-119">列のデータ本体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="32887-119">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="32887-120">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="32887-120">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="32887-121">Range</span><span class="sxs-lookup"><span data-stu-id="32887-121">Range</span></span>](range.md)|<span data-ttu-id="32887-122">列のヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="32887-122">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="32887-123">Range</span><span class="sxs-lookup"><span data-stu-id="32887-123">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="32887-124">Range</span><span class="sxs-lookup"><span data-stu-id="32887-124">Range</span></span>](range.md)|<span data-ttu-id="32887-125">列全体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="32887-125">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="32887-126">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="32887-126">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="32887-127">Range</span><span class="sxs-lookup"><span data-stu-id="32887-127">Range</span></span>](range.md)|<span data-ttu-id="32887-128">列の集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="32887-128">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="32887-129">Delete</span><span class="sxs-lookup"><span data-stu-id="32887-129">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="32887-130">なし</span><span class="sxs-lookup"><span data-stu-id="32887-130">None</span></span>|<span data-ttu-id="32887-131">テーブルから列を削除します。</span><span class="sxs-lookup"><span data-stu-id="32887-131">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="32887-132">List</span><span class="sxs-lookup"><span data-stu-id="32887-132">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="32887-133">[TableColumn](tablecolumn.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="32887-133">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="32887-134">tableColumn オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="32887-134">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="32887-135">Itemat</span><span class="sxs-lookup"><span data-stu-id="32887-135">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="32887-136">TableColumn</span><span class="sxs-lookup"><span data-stu-id="32887-136">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="32887-137">コレクション内の位置に基づいて列を取得します。</span><span class="sxs-lookup"><span data-stu-id="32887-137">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="32887-138">Add</span><span class="sxs-lookup"><span data-stu-id="32887-138">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="32887-139">TableColumn</span><span class="sxs-lookup"><span data-stu-id="32887-139">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="32887-140">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="32887-140">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="32887-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32887-141">Properties</span></span>
| <span data-ttu-id="32887-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32887-142">Property</span></span>     | <span data-ttu-id="32887-143">型</span><span class="sxs-lookup"><span data-stu-id="32887-143">Type</span></span>   |<span data-ttu-id="32887-144">説明</span><span class="sxs-lookup"><span data-stu-id="32887-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32887-145">ID</span><span class="sxs-lookup"><span data-stu-id="32887-145">id</span></span>|<span data-ttu-id="32887-146">int</span><span class="sxs-lookup"><span data-stu-id="32887-146">int</span></span>|<span data-ttu-id="32887-p102">テーブル内の列を識別する一意のキーを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32887-p102">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="32887-149">index</span><span class="sxs-lookup"><span data-stu-id="32887-149">index</span></span>|<span data-ttu-id="32887-150">int</span><span class="sxs-lookup"><span data-stu-id="32887-150">int</span></span>|<span data-ttu-id="32887-p103">テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32887-p103">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="32887-154">name</span><span class="sxs-lookup"><span data-stu-id="32887-154">name</span></span>|<span data-ttu-id="32887-155">文字列</span><span class="sxs-lookup"><span data-stu-id="32887-155">string</span></span>|<span data-ttu-id="32887-p104">テーブル列の名前を取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32887-p104">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="32887-158">values</span><span class="sxs-lookup"><span data-stu-id="32887-158">values</span></span>|<span data-ttu-id="32887-159">json</span><span class="sxs-lookup"><span data-stu-id="32887-159">json</span></span>|<span data-ttu-id="32887-p105">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="32887-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32887-163">関係</span><span class="sxs-lookup"><span data-stu-id="32887-163">Relationships</span></span>
| <span data-ttu-id="32887-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32887-164">Relationship</span></span> | <span data-ttu-id="32887-165">型</span><span class="sxs-lookup"><span data-stu-id="32887-165">Type</span></span>   |<span data-ttu-id="32887-166">説明</span><span class="sxs-lookup"><span data-stu-id="32887-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32887-167">filter</span><span class="sxs-lookup"><span data-stu-id="32887-167">filter</span></span>|[<span data-ttu-id="32887-168">Filter</span><span class="sxs-lookup"><span data-stu-id="32887-168">Filter</span></span>](filter.md)|<span data-ttu-id="32887-p106">列に適用されるフィルターを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32887-p106">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32887-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32887-171">JSON representation</span></span>

<span data-ttu-id="32887-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="32887-172">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->