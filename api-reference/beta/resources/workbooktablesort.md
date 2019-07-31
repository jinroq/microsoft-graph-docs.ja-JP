---
title: workbookTableSort リソースの種類
description: Table オブジェクトの並べ替え操作を管理します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ea0332f1ad00029cf511f2bc55aca80836e5ef2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007033"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="40c16-103">workbookTableSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40c16-103">workbookTableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40c16-104">Table オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="40c16-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="40c16-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="40c16-105">Methods</span></span>

| <span data-ttu-id="40c16-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="40c16-106">Method</span></span>           | <span data-ttu-id="40c16-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="40c16-107">Return Type</span></span>    |<span data-ttu-id="40c16-108">説明</span><span class="sxs-lookup"><span data-stu-id="40c16-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40c16-109">TableSort を取得する</span><span class="sxs-lookup"><span data-stu-id="40c16-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="40c16-110">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="40c16-110">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="40c16-111">tableSort オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="40c16-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="40c16-112">Apply</span><span class="sxs-lookup"><span data-stu-id="40c16-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="40c16-113">None</span><span class="sxs-lookup"><span data-stu-id="40c16-113">None</span></span>|<span data-ttu-id="40c16-114">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="40c16-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="40c16-115">Clear</span><span class="sxs-lookup"><span data-stu-id="40c16-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="40c16-116">なし</span><span class="sxs-lookup"><span data-stu-id="40c16-116">None</span></span>|<span data-ttu-id="40c16-p101">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="40c16-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="40c16-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="40c16-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="40c16-120">なし</span><span class="sxs-lookup"><span data-stu-id="40c16-120">None</span></span>|<span data-ttu-id="40c16-121">テーブルに、現在の並べ替えパラメーターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="40c16-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="40c16-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40c16-122">Properties</span></span>
| <span data-ttu-id="40c16-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40c16-123">Property</span></span>     | <span data-ttu-id="40c16-124">型</span><span class="sxs-lookup"><span data-stu-id="40c16-124">Type</span></span>   |<span data-ttu-id="40c16-125">説明</span><span class="sxs-lookup"><span data-stu-id="40c16-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40c16-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="40c16-126">matchCase</span></span>|<span data-ttu-id="40c16-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="40c16-127">boolean</span></span>|<span data-ttu-id="40c16-p102">大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="40c16-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="40c16-130">method</span><span class="sxs-lookup"><span data-stu-id="40c16-130">method</span></span>|<span data-ttu-id="40c16-131">string</span><span class="sxs-lookup"><span data-stu-id="40c16-131">string</span></span>|<span data-ttu-id="40c16-p103">テーブルの並べ替えで最後に使用した中国語文字の順序付け方法を表します。可能な値は、`PinYin`、`StrokeCount` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="40c16-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40c16-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="40c16-135">Relationships</span></span>
| <span data-ttu-id="40c16-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="40c16-136">Relationship</span></span> | <span data-ttu-id="40c16-137">型</span><span class="sxs-lookup"><span data-stu-id="40c16-137">Type</span></span>   |<span data-ttu-id="40c16-138">説明</span><span class="sxs-lookup"><span data-stu-id="40c16-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40c16-139">fields</span><span class="sxs-lookup"><span data-stu-id="40c16-139">fields</span></span>|[<span data-ttu-id="40c16-140">workbookSortField</span><span class="sxs-lookup"><span data-stu-id="40c16-140">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="40c16-141">テーブルの最後の並べ替えに使用する現在の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="40c16-141">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="40c16-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="40c16-142">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40c16-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40c16-143">JSON representation</span></span>

<span data-ttu-id="40c16-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40c16-144">Here is a JSON representation of the resource.</span></span>

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
