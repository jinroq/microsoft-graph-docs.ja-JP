---
title: workbookFilter リソースの種類
description: テーブルの列のフィルター処理を管理します。
localization_priority: Normal
ms.openlocfilehash: 79ded0bfca0ace3b2d7c1bcdb4cd8dd2696802a4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348906"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="dabe7-103">workbookFilter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dabe7-103">workbookFilter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dabe7-104">テーブルの列のフィルター処理を管理します。</span><span class="sxs-lookup"><span data-stu-id="dabe7-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="dabe7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="dabe7-105">Methods</span></span>

| <span data-ttu-id="dabe7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="dabe7-106">Method</span></span>           | <span data-ttu-id="dabe7-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dabe7-107">Return Type</span></span>    |<span data-ttu-id="dabe7-108">説明</span><span class="sxs-lookup"><span data-stu-id="dabe7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dabe7-109">Apply</span><span class="sxs-lookup"><span data-stu-id="dabe7-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="dabe7-110">なし</span><span class="sxs-lookup"><span data-stu-id="dabe7-110">None</span></span>|<span data-ttu-id="dabe7-111">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="dabe7-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="dabe7-112">Clear</span><span class="sxs-lookup"><span data-stu-id="dabe7-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="dabe7-113">なし</span><span class="sxs-lookup"><span data-stu-id="dabe7-113">None</span></span>|<span data-ttu-id="dabe7-114">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="dabe7-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="dabe7-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dabe7-115">Properties</span></span>
<span data-ttu-id="dabe7-116">なし</span><span class="sxs-lookup"><span data-stu-id="dabe7-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dabe7-117">関係</span><span class="sxs-lookup"><span data-stu-id="dabe7-117">Relationships</span></span>
| <span data-ttu-id="dabe7-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dabe7-118">Relationship</span></span> | <span data-ttu-id="dabe7-119">型</span><span class="sxs-lookup"><span data-stu-id="dabe7-119">Type</span></span>   |<span data-ttu-id="dabe7-120">説明</span><span class="sxs-lookup"><span data-stu-id="dabe7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dabe7-121">criteria</span><span class="sxs-lookup"><span data-stu-id="dabe7-121">criteria</span></span>|[<span data-ttu-id="dabe7-122">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="dabe7-122">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="dabe7-123">指定した列に現在適用されているフィルターです。</span><span class="sxs-lookup"><span data-stu-id="dabe7-123">The currently applied filter on the given column.</span></span> <span data-ttu-id="dabe7-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dabe7-124">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dabe7-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dabe7-125">JSON representation</span></span>

<span data-ttu-id="dabe7-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dabe7-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
    "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
