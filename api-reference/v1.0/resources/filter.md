---
title: フィルター リソースの種類
description: テーブルの列のフィルター処理を管理します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3f58e1f5207fc3b4aebe2fdfb780735c0c5d209d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032481"
---
# <a name="filter-resource-type"></a><span data-ttu-id="0d7b3-103">フィルター リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d7b3-103">Filter resource type</span></span>

<span data-ttu-id="0d7b3-104">テーブルの列のフィルター処理を管理します。</span><span class="sxs-lookup"><span data-stu-id="0d7b3-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="0d7b3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d7b3-105">Methods</span></span>

| <span data-ttu-id="0d7b3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d7b3-106">Method</span></span>           | <span data-ttu-id="0d7b3-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0d7b3-107">Return Type</span></span>    |<span data-ttu-id="0d7b3-108">説明</span><span class="sxs-lookup"><span data-stu-id="0d7b3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d7b3-109">Apply</span><span class="sxs-lookup"><span data-stu-id="0d7b3-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="0d7b3-110">なし</span><span class="sxs-lookup"><span data-stu-id="0d7b3-110">None</span></span>|<span data-ttu-id="0d7b3-111">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="0d7b3-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="0d7b3-112">Clear</span><span class="sxs-lookup"><span data-stu-id="0d7b3-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="0d7b3-113">なし</span><span class="sxs-lookup"><span data-stu-id="0d7b3-113">None</span></span>|<span data-ttu-id="0d7b3-114">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="0d7b3-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d7b3-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d7b3-115">Properties</span></span>

| <span data-ttu-id="0d7b3-116">名前</span><span class="sxs-lookup"><span data-stu-id="0d7b3-116">Name</span></span> | <span data-ttu-id="0d7b3-117">型</span><span class="sxs-lookup"><span data-stu-id="0d7b3-117">Type</span></span>   |<span data-ttu-id="0d7b3-118">説明</span><span class="sxs-lookup"><span data-stu-id="0d7b3-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d7b3-119">criteria</span><span class="sxs-lookup"><span data-stu-id="0d7b3-119">criteria</span></span>|[<span data-ttu-id="0d7b3-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="0d7b3-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="0d7b3-121">指定した列に現在適用されているフィルターです。</span><span class="sxs-lookup"><span data-stu-id="0d7b3-121">The currently applied filter on the given column.</span></span> <span data-ttu-id="0d7b3-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0d7b3-122">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d7b3-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d7b3-123">JSON representation</span></span>

<span data-ttu-id="0d7b3-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0d7b3-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
