---
title: フィルター リソースの種類
description: テーブルの列のフィルター処理を管理します。
ms.openlocfilehash: 272b4ea0ee91c25ea845217512a12e33b08ed7b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021852"
---
# <a name="filter-resource-type"></a><span data-ttu-id="1260b-103">フィルター リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1260b-103">Filter resource type</span></span>

<span data-ttu-id="1260b-104">テーブルの列のフィルター処理を管理します。</span><span class="sxs-lookup"><span data-stu-id="1260b-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="1260b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1260b-105">Methods</span></span>

| <span data-ttu-id="1260b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1260b-106">Method</span></span>           | <span data-ttu-id="1260b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1260b-107">Return Type</span></span>    |<span data-ttu-id="1260b-108">説明</span><span class="sxs-lookup"><span data-stu-id="1260b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1260b-109">適用</span><span class="sxs-lookup"><span data-stu-id="1260b-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="1260b-110">なし</span><span class="sxs-lookup"><span data-stu-id="1260b-110">None</span></span>|<span data-ttu-id="1260b-111">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="1260b-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="1260b-112">クリア</span><span class="sxs-lookup"><span data-stu-id="1260b-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="1260b-113">なし</span><span class="sxs-lookup"><span data-stu-id="1260b-113">None</span></span>|<span data-ttu-id="1260b-114">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="1260b-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="1260b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1260b-115">Properties</span></span>

| <span data-ttu-id="1260b-116">名前</span><span class="sxs-lookup"><span data-stu-id="1260b-116">Name</span></span> | <span data-ttu-id="1260b-117">型</span><span class="sxs-lookup"><span data-stu-id="1260b-117">Type</span></span>   |<span data-ttu-id="1260b-118">説明</span><span class="sxs-lookup"><span data-stu-id="1260b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1260b-119">criteria</span><span class="sxs-lookup"><span data-stu-id="1260b-119">criteria</span></span>|[<span data-ttu-id="1260b-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="1260b-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="1260b-p101">指定した列に現在適用されているフィルターです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1260b-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1260b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1260b-123">JSON representation</span></span>

<span data-ttu-id="1260b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1260b-124">Here is a JSON representation of the resource.</span></span>

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