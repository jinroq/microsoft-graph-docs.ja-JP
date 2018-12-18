---
title: TableSort リソースの種類
description: テーブル オブジェクトの並べ替え操作を管理します。
author: lumine2008
ms.openlocfilehash: 52ee5288698b236f7ee4d29eb75fdac5ad14fa0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339824"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="e5bc3-103">TableSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5bc3-103">TableSort resource type</span></span>

> <span data-ttu-id="e5bc3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5bc3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5bc3-106">テーブル オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-106">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="e5bc3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5bc3-107">Methods</span></span>

| <span data-ttu-id="e5bc3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5bc3-108">Method</span></span>           | <span data-ttu-id="e5bc3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e5bc3-109">Return Type</span></span>    |<span data-ttu-id="e5bc3-110">説明</span><span class="sxs-lookup"><span data-stu-id="e5bc3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5bc3-111">TableSort を取得する</span><span class="sxs-lookup"><span data-stu-id="e5bc3-111">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="e5bc3-112">TableSort</span><span class="sxs-lookup"><span data-stu-id="e5bc3-112">TableSort</span></span>](tablesort.md) |<span data-ttu-id="e5bc3-113">tableSort オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-113">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="e5bc3-114">Apply</span><span class="sxs-lookup"><span data-stu-id="e5bc3-114">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="e5bc3-115">なし</span><span class="sxs-lookup"><span data-stu-id="e5bc3-115">None</span></span>|<span data-ttu-id="e5bc3-116">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-116">Perform a sort operation.</span></span>|
|[<span data-ttu-id="e5bc3-117">Clear</span><span class="sxs-lookup"><span data-stu-id="e5bc3-117">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="e5bc3-118">なし</span><span class="sxs-lookup"><span data-stu-id="e5bc3-118">None</span></span>|<span data-ttu-id="e5bc3-p102">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="e5bc3-121">Reapply</span><span class="sxs-lookup"><span data-stu-id="e5bc3-121">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="e5bc3-122">なし</span><span class="sxs-lookup"><span data-stu-id="e5bc3-122">None</span></span>|<span data-ttu-id="e5bc3-123">テーブルに、現在の並べ替えパラメーターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-123">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5bc3-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5bc3-124">Properties</span></span>
| <span data-ttu-id="e5bc3-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5bc3-125">Property</span></span>     | <span data-ttu-id="e5bc3-126">種類</span><span class="sxs-lookup"><span data-stu-id="e5bc3-126">Type</span></span>   |<span data-ttu-id="e5bc3-127">説明</span><span class="sxs-lookup"><span data-stu-id="e5bc3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5bc3-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="e5bc3-128">matchCase</span></span>|<span data-ttu-id="e5bc3-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="e5bc3-129">boolean</span></span>|<span data-ttu-id="e5bc3-p103">大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="e5bc3-132">method</span><span class="sxs-lookup"><span data-stu-id="e5bc3-132">method</span></span>|<span data-ttu-id="e5bc3-133">string</span><span class="sxs-lookup"><span data-stu-id="e5bc3-133">string</span></span>|<span data-ttu-id="e5bc3-p104">テーブルの並べ替えで最後に使用した中国語文字の順序付け方法を表します。可能な値は、`PinYin`、`StrokeCount` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-p104">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5bc3-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5bc3-137">Relationships</span></span>
| <span data-ttu-id="e5bc3-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5bc3-138">Relationship</span></span> | <span data-ttu-id="e5bc3-139">型</span><span class="sxs-lookup"><span data-stu-id="e5bc3-139">Type</span></span>   |<span data-ttu-id="e5bc3-140">説明</span><span class="sxs-lookup"><span data-stu-id="e5bc3-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5bc3-141">fields</span><span class="sxs-lookup"><span data-stu-id="e5bc3-141">fields</span></span>|[<span data-ttu-id="e5bc3-142">SortField</span><span class="sxs-lookup"><span data-stu-id="e5bc3-142">SortField</span></span>](sortfield.md)|<span data-ttu-id="e5bc3-p105">テーブルの最後の並べ替えに使用する現在の条件を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-p105">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5bc3-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5bc3-145">JSON representation</span></span>

<span data-ttu-id="e5bc3-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5bc3-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->