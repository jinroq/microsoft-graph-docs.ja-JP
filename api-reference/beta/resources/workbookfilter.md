---
title: workbookFilter リソースの種類
description: テーブルの列のフィルター処理を管理します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: f3622a2efd952907214add4343bb5958adebe606
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007124"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="ddb75-103">workbookFilter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ddb75-103">workbookFilter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb75-104">テーブルの列のフィルター処理を管理します。</span><span class="sxs-lookup"><span data-stu-id="ddb75-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="ddb75-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddb75-105">Methods</span></span>

| <span data-ttu-id="ddb75-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddb75-106">Method</span></span>           | <span data-ttu-id="ddb75-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ddb75-107">Return Type</span></span>    |<span data-ttu-id="ddb75-108">説明</span><span class="sxs-lookup"><span data-stu-id="ddb75-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ddb75-109">Apply</span><span class="sxs-lookup"><span data-stu-id="ddb75-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="ddb75-110">None</span><span class="sxs-lookup"><span data-stu-id="ddb75-110">None</span></span>|<span data-ttu-id="ddb75-111">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="ddb75-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="ddb75-112">Clear</span><span class="sxs-lookup"><span data-stu-id="ddb75-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="ddb75-113">なし</span><span class="sxs-lookup"><span data-stu-id="ddb75-113">None</span></span>|<span data-ttu-id="ddb75-114">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="ddb75-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddb75-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddb75-115">Properties</span></span>
<span data-ttu-id="ddb75-116">なし</span><span class="sxs-lookup"><span data-stu-id="ddb75-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ddb75-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddb75-117">Relationships</span></span>
| <span data-ttu-id="ddb75-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddb75-118">Relationship</span></span> | <span data-ttu-id="ddb75-119">型</span><span class="sxs-lookup"><span data-stu-id="ddb75-119">Type</span></span>   |<span data-ttu-id="ddb75-120">説明</span><span class="sxs-lookup"><span data-stu-id="ddb75-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddb75-121">criteria</span><span class="sxs-lookup"><span data-stu-id="ddb75-121">criteria</span></span>|[<span data-ttu-id="ddb75-122">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="ddb75-122">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="ddb75-123">指定した列に現在適用されているフィルターです。</span><span class="sxs-lookup"><span data-stu-id="ddb75-123">The currently applied filter on the given column.</span></span> <span data-ttu-id="ddb75-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddb75-124">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ddb75-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddb75-125">JSON representation</span></span>

<span data-ttu-id="ddb75-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ddb75-126">Here is a JSON representation of the resource.</span></span>

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
