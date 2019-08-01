---
title: TableSort リソースの種類
description: Table オブジェクトの並べ替え操作を管理します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 14dbd96567510a3aefab4fddbc57a196c7734b5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033916"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="38195-103">TableSort リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38195-103">TableSort resource type</span></span>

<span data-ttu-id="38195-104">Table オブジェクトの並べ替え操作を管理します。</span><span class="sxs-lookup"><span data-stu-id="38195-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="38195-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="38195-105">Methods</span></span>

| <span data-ttu-id="38195-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="38195-106">Method</span></span>           | <span data-ttu-id="38195-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="38195-107">Return Type</span></span>    |<span data-ttu-id="38195-108">説明</span><span class="sxs-lookup"><span data-stu-id="38195-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38195-109">TableSort を取得する</span><span class="sxs-lookup"><span data-stu-id="38195-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="38195-110">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="38195-110">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="38195-111">tableSort オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="38195-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="38195-112">Apply</span><span class="sxs-lookup"><span data-stu-id="38195-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="38195-113">None</span><span class="sxs-lookup"><span data-stu-id="38195-113">None</span></span>|<span data-ttu-id="38195-114">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="38195-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="38195-115">Clear</span><span class="sxs-lookup"><span data-stu-id="38195-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="38195-116">なし</span><span class="sxs-lookup"><span data-stu-id="38195-116">None</span></span>|<span data-ttu-id="38195-p101">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="38195-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="38195-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="38195-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="38195-120">なし</span><span class="sxs-lookup"><span data-stu-id="38195-120">None</span></span>|<span data-ttu-id="38195-121">テーブルに、現在の並べ替えパラメーターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="38195-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="38195-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38195-122">Properties</span></span>
| <span data-ttu-id="38195-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38195-123">Property</span></span>     | <span data-ttu-id="38195-124">型</span><span class="sxs-lookup"><span data-stu-id="38195-124">Type</span></span>   |<span data-ttu-id="38195-125">説明</span><span class="sxs-lookup"><span data-stu-id="38195-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38195-126">fields</span><span class="sxs-lookup"><span data-stu-id="38195-126">fields</span></span>|<span data-ttu-id="38195-127">[WorkbookSortField](sortfield.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="38195-127">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="38195-128">テーブルの最後の並べ替えに使用する現在の条件を表します。</span><span class="sxs-lookup"><span data-stu-id="38195-128">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="38195-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="38195-129">Read-only.</span></span>|
|<span data-ttu-id="38195-130">matchCase</span><span class="sxs-lookup"><span data-stu-id="38195-130">matchCase</span></span>|<span data-ttu-id="38195-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="38195-131">boolean</span></span>|<span data-ttu-id="38195-p103">大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="38195-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="38195-134">method</span><span class="sxs-lookup"><span data-stu-id="38195-134">method</span></span>|<span data-ttu-id="38195-135">string</span><span class="sxs-lookup"><span data-stu-id="38195-135">string</span></span>|<span data-ttu-id="38195-136">テーブルの並べ替えで最後に使用した中国語文字の順序付け方法を表します。</span><span class="sxs-lookup"><span data-stu-id="38195-136">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="38195-137">使用可能な値は`PinYin`、 `StrokeCount`、です。</span><span class="sxs-lookup"><span data-stu-id="38195-137">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="38195-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="38195-138">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38195-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38195-139">JSON representation</span></span>

<span data-ttu-id="38195-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="38195-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
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
