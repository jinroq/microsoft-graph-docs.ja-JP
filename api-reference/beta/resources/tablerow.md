---
title: TableRow リソースの種類
description: 表の行を表します。
ms.openlocfilehash: ca363f8202d61364c609144eaa2fc136ab8b2928
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070552"
---
# <a name="tablerow-resource-type"></a><span data-ttu-id="ba62e-103">TableRow リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba62e-103">TableRow resource type</span></span>

> <span data-ttu-id="ba62e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ba62e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba62e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba62e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba62e-106">表の行を表します。</span><span class="sxs-lookup"><span data-stu-id="ba62e-106">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="ba62e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ba62e-107">Methods</span></span>

| <span data-ttu-id="ba62e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ba62e-108">Method</span></span>           | <span data-ttu-id="ba62e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ba62e-109">Return Type</span></span>    |<span data-ttu-id="ba62e-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba62e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba62e-111">TableRow を取得する</span><span class="sxs-lookup"><span data-stu-id="ba62e-111">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="ba62e-112">TableRow</span><span class="sxs-lookup"><span data-stu-id="ba62e-112">TableRow</span></span>](tablerow.md) |<span data-ttu-id="ba62e-113">tableRow オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ba62e-113">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="ba62e-114">Update</span><span class="sxs-lookup"><span data-stu-id="ba62e-114">Update</span></span>](../api/tablerow-update.md) | [<span data-ttu-id="ba62e-115">TableRow</span><span class="sxs-lookup"><span data-stu-id="ba62e-115">TableRow</span></span>](tablerow.md)  |<span data-ttu-id="ba62e-116">TableRow を更新します。</span><span class="sxs-lookup"><span data-stu-id="ba62e-116">Update TableRow object.</span></span> |
|[<span data-ttu-id="ba62e-117">Range</span><span class="sxs-lookup"><span data-stu-id="ba62e-117">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="ba62e-118">Range</span><span class="sxs-lookup"><span data-stu-id="ba62e-118">Range</span></span>](range.md)|<span data-ttu-id="ba62e-119">行全体に関連付けられた範囲オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ba62e-119">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="ba62e-120">削除</span><span class="sxs-lookup"><span data-stu-id="ba62e-120">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="ba62e-121">なし</span><span class="sxs-lookup"><span data-stu-id="ba62e-121">None</span></span>|<span data-ttu-id="ba62e-122">テーブルから行を削除します。</span><span class="sxs-lookup"><span data-stu-id="ba62e-122">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="ba62e-123">List</span><span class="sxs-lookup"><span data-stu-id="ba62e-123">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="ba62e-124">[TableRow](tablerow.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ba62e-124">[TableRow](tablerow.md) collection</span></span> |<span data-ttu-id="ba62e-125">tableRow オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ba62e-125">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="ba62e-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="ba62e-126">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="ba62e-127">TableRow</span><span class="sxs-lookup"><span data-stu-id="ba62e-127">TableRow</span></span>](tablerow.md)|<span data-ttu-id="ba62e-128">コレクション内の位置を基に行を取得します。</span><span class="sxs-lookup"><span data-stu-id="ba62e-128">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="ba62e-129">追加</span><span class="sxs-lookup"><span data-stu-id="ba62e-129">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="ba62e-130">TableRow</span><span class="sxs-lookup"><span data-stu-id="ba62e-130">TableRow</span></span>](tablerow.md)|<span data-ttu-id="ba62e-131">新しい行をテーブルに追加します。</span><span class="sxs-lookup"><span data-stu-id="ba62e-131">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba62e-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba62e-132">Properties</span></span>
| <span data-ttu-id="ba62e-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba62e-133">Property</span></span>     | <span data-ttu-id="ba62e-134">型</span><span class="sxs-lookup"><span data-stu-id="ba62e-134">Type</span></span>   |<span data-ttu-id="ba62e-135">説明</span><span class="sxs-lookup"><span data-stu-id="ba62e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba62e-136">index</span><span class="sxs-lookup"><span data-stu-id="ba62e-136">index</span></span>|<span data-ttu-id="ba62e-137">int</span><span class="sxs-lookup"><span data-stu-id="ba62e-137">int</span></span>|<span data-ttu-id="ba62e-p102">テーブルの行コレクション内の行のインデックス番号を返します。0 を起点とする番号になります。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ba62e-p102">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="ba62e-141">values</span><span class="sxs-lookup"><span data-stu-id="ba62e-141">values</span></span>|<span data-ttu-id="ba62e-142">json</span><span class="sxs-lookup"><span data-stu-id="ba62e-142">json</span></span>|<span data-ttu-id="ba62e-p103">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="ba62e-p103">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba62e-146">関係</span><span class="sxs-lookup"><span data-stu-id="ba62e-146">Relationships</span></span>
<span data-ttu-id="ba62e-147">なし</span><span class="sxs-lookup"><span data-stu-id="ba62e-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ba62e-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba62e-148">JSON representation</span></span>

<span data-ttu-id="ba62e-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba62e-149">Here is a JSON representation of the resource.</span></span>

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