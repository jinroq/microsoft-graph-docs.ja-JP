---
title: TableRow リソースの種類
description: 表の行を表します。
author: lumine2008
ms.openlocfilehash: de83ec8cae87f159c6f1f9687bd093873558c150
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309885"
---
# <a name="tablerow-resource-type"></a><span data-ttu-id="35292-103">TableRow リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35292-103">TableRow resource type</span></span>

> <span data-ttu-id="35292-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35292-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35292-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35292-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35292-106">表の行を表します。</span><span class="sxs-lookup"><span data-stu-id="35292-106">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="35292-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="35292-107">Methods</span></span>

| <span data-ttu-id="35292-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="35292-108">Method</span></span>           | <span data-ttu-id="35292-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="35292-109">Return Type</span></span>    |<span data-ttu-id="35292-110">説明</span><span class="sxs-lookup"><span data-stu-id="35292-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35292-111">TableRow を取得する</span><span class="sxs-lookup"><span data-stu-id="35292-111">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="35292-112">TableRow</span><span class="sxs-lookup"><span data-stu-id="35292-112">TableRow</span></span>](tablerow.md) |<span data-ttu-id="35292-113">tableRow オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="35292-113">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="35292-114">Update</span><span class="sxs-lookup"><span data-stu-id="35292-114">Update</span></span>](../api/tablerow-update.md) | [<span data-ttu-id="35292-115">TableRow</span><span class="sxs-lookup"><span data-stu-id="35292-115">TableRow</span></span>](tablerow.md)  |<span data-ttu-id="35292-116">TableRow を更新します。</span><span class="sxs-lookup"><span data-stu-id="35292-116">Update TableRow object.</span></span> |
|[<span data-ttu-id="35292-117">Range</span><span class="sxs-lookup"><span data-stu-id="35292-117">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="35292-118">Range</span><span class="sxs-lookup"><span data-stu-id="35292-118">Range</span></span>](range.md)|<span data-ttu-id="35292-119">行全体に関連付けられた範囲オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="35292-119">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="35292-120">Delete</span><span class="sxs-lookup"><span data-stu-id="35292-120">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="35292-121">なし</span><span class="sxs-lookup"><span data-stu-id="35292-121">None</span></span>|<span data-ttu-id="35292-122">テーブルから行を削除します。</span><span class="sxs-lookup"><span data-stu-id="35292-122">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="35292-123">List</span><span class="sxs-lookup"><span data-stu-id="35292-123">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="35292-124">[TableRow](tablerow.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35292-124">[TableRow](tablerow.md) collection</span></span> |<span data-ttu-id="35292-125">tableRow オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="35292-125">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="35292-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="35292-126">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="35292-127">TableRow</span><span class="sxs-lookup"><span data-stu-id="35292-127">TableRow</span></span>](tablerow.md)|<span data-ttu-id="35292-128">コレクション内の位置を基に行を取得します。</span><span class="sxs-lookup"><span data-stu-id="35292-128">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="35292-129">Add</span><span class="sxs-lookup"><span data-stu-id="35292-129">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="35292-130">TableRow</span><span class="sxs-lookup"><span data-stu-id="35292-130">TableRow</span></span>](tablerow.md)|<span data-ttu-id="35292-131">新しい行をテーブルに追加します。</span><span class="sxs-lookup"><span data-stu-id="35292-131">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="35292-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35292-132">Properties</span></span>
| <span data-ttu-id="35292-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35292-133">Property</span></span>     | <span data-ttu-id="35292-134">種類</span><span class="sxs-lookup"><span data-stu-id="35292-134">Type</span></span>   |<span data-ttu-id="35292-135">説明</span><span class="sxs-lookup"><span data-stu-id="35292-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35292-136">index</span><span class="sxs-lookup"><span data-stu-id="35292-136">index</span></span>|<span data-ttu-id="35292-137">int</span><span class="sxs-lookup"><span data-stu-id="35292-137">int</span></span>|<span data-ttu-id="35292-p102">テーブルの行コレクション内の行のインデックス番号を返します。0 を起点とする番号になります。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="35292-p102">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="35292-141">values</span><span class="sxs-lookup"><span data-stu-id="35292-141">values</span></span>|<span data-ttu-id="35292-142">json</span><span class="sxs-lookup"><span data-stu-id="35292-142">json</span></span>|<span data-ttu-id="35292-p103">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="35292-p103">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35292-146">関係</span><span class="sxs-lookup"><span data-stu-id="35292-146">Relationships</span></span>
<span data-ttu-id="35292-147">なし</span><span class="sxs-lookup"><span data-stu-id="35292-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="35292-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35292-148">JSON representation</span></span>

<span data-ttu-id="35292-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35292-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->