---
title: workbookTableSort リソースの種類
description: Table オブジェクトの並べ替え操作を管理します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6ba1e7cdcf48a3ac5cf8262be2174481016aad2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348864"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="067ff-103">workbookTableSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="067ff-103">workbookTableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="067ff-104">Table オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="067ff-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="067ff-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="067ff-105">Methods</span></span>

| <span data-ttu-id="067ff-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="067ff-106">Method</span></span>           | <span data-ttu-id="067ff-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="067ff-107">Return Type</span></span>    |<span data-ttu-id="067ff-108">説明</span><span class="sxs-lookup"><span data-stu-id="067ff-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="067ff-109">TableSort を取得する</span><span class="sxs-lookup"><span data-stu-id="067ff-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="067ff-110">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="067ff-110">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="067ff-111">tableSort オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="067ff-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="067ff-112">Apply</span><span class="sxs-lookup"><span data-stu-id="067ff-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="067ff-113">なし</span><span class="sxs-lookup"><span data-stu-id="067ff-113">None</span></span>|<span data-ttu-id="067ff-114">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="067ff-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="067ff-115">Clear</span><span class="sxs-lookup"><span data-stu-id="067ff-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="067ff-116">なし</span><span class="sxs-lookup"><span data-stu-id="067ff-116">None</span></span>|<span data-ttu-id="067ff-p101">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="067ff-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="067ff-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="067ff-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="067ff-120">なし</span><span class="sxs-lookup"><span data-stu-id="067ff-120">None</span></span>|<span data-ttu-id="067ff-121">テーブルに、現在の並べ替えパラメーターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="067ff-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="067ff-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="067ff-122">Properties</span></span>
| <span data-ttu-id="067ff-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="067ff-123">Property</span></span>     | <span data-ttu-id="067ff-124">種類</span><span class="sxs-lookup"><span data-stu-id="067ff-124">Type</span></span>   |<span data-ttu-id="067ff-125">説明</span><span class="sxs-lookup"><span data-stu-id="067ff-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="067ff-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="067ff-126">matchCase</span></span>|<span data-ttu-id="067ff-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="067ff-127">boolean</span></span>|<span data-ttu-id="067ff-p102">大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="067ff-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="067ff-130">method</span><span class="sxs-lookup"><span data-stu-id="067ff-130">method</span></span>|<span data-ttu-id="067ff-131">string</span><span class="sxs-lookup"><span data-stu-id="067ff-131">string</span></span>|<span data-ttu-id="067ff-p103">テーブルの並べ替えで最後に使用した中国語文字の順序付け方法を表します。可能な値は、`PinYin`、`StrokeCount` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="067ff-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="067ff-135">関係</span><span class="sxs-lookup"><span data-stu-id="067ff-135">Relationships</span></span>
| <span data-ttu-id="067ff-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="067ff-136">Relationship</span></span> | <span data-ttu-id="067ff-137">型</span><span class="sxs-lookup"><span data-stu-id="067ff-137">Type</span></span>   |<span data-ttu-id="067ff-138">説明</span><span class="sxs-lookup"><span data-stu-id="067ff-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="067ff-139">fields</span><span class="sxs-lookup"><span data-stu-id="067ff-139">fields</span></span>|[<span data-ttu-id="067ff-140">workbookSortField</span><span class="sxs-lookup"><span data-stu-id="067ff-140">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="067ff-141">テーブルの最後の並べ替えに使用する現在の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="067ff-141">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="067ff-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="067ff-142">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="067ff-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="067ff-143">JSON representation</span></span>

<span data-ttu-id="067ff-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="067ff-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
 
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "id": "string",
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
