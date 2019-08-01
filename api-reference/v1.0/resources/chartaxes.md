---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7e8ee5eac8face4d16418799d627d3aa168c48c2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029877"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="657c4-103">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="657c4-103">ChartAxes resource type</span></span>

<span data-ttu-id="657c4-104">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="657c4-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="657c4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="657c4-105">Methods</span></span>
<span data-ttu-id="657c4-106">None</span><span class="sxs-lookup"><span data-stu-id="657c4-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="657c4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="657c4-107">Properties</span></span>
<span data-ttu-id="657c4-108">なし</span><span class="sxs-lookup"><span data-stu-id="657c4-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="657c4-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="657c4-109">Relationships</span></span>
| <span data-ttu-id="657c4-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="657c4-110">Relationship</span></span> | <span data-ttu-id="657c4-111">型</span><span class="sxs-lookup"><span data-stu-id="657c4-111">Type</span></span>   |<span data-ttu-id="657c4-112">説明</span><span class="sxs-lookup"><span data-stu-id="657c4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="657c4-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="657c4-113">categoryAxis</span></span>|[<span data-ttu-id="657c4-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="657c4-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="657c4-p101">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="657c4-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="657c4-117">系列軸</span><span class="sxs-lookup"><span data-stu-id="657c4-117">seriesAxis</span></span>|[<span data-ttu-id="657c4-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="657c4-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="657c4-p102">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="657c4-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="657c4-121">数値軸</span><span class="sxs-lookup"><span data-stu-id="657c4-121">valueAxis</span></span>|[<span data-ttu-id="657c4-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="657c4-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="657c4-123">軸の数値軸を表します。</span><span class="sxs-lookup"><span data-stu-id="657c4-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="657c4-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="657c4-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="657c4-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="657c4-125">JSON representation</span></span>

<span data-ttu-id="657c4-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="657c4-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
