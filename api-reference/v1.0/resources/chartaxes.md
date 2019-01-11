---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 53f0e4a7344ddfab89330203f90032266e0c622d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885905"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="6c626-103">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c626-103">ChartAxes resource type</span></span>

<span data-ttu-id="6c626-104">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="6c626-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="6c626-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c626-105">Methods</span></span>
<span data-ttu-id="6c626-106">なし</span><span class="sxs-lookup"><span data-stu-id="6c626-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="6c626-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c626-107">Properties</span></span>
<span data-ttu-id="6c626-108">なし</span><span class="sxs-lookup"><span data-stu-id="6c626-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6c626-109">関係</span><span class="sxs-lookup"><span data-stu-id="6c626-109">Relationships</span></span>
| <span data-ttu-id="6c626-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c626-110">Relationship</span></span> | <span data-ttu-id="6c626-111">型</span><span class="sxs-lookup"><span data-stu-id="6c626-111">Type</span></span>   |<span data-ttu-id="6c626-112">説明</span><span class="sxs-lookup"><span data-stu-id="6c626-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c626-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="6c626-113">categoryAxis</span></span>|[<span data-ttu-id="6c626-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="6c626-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="6c626-p101">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6c626-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="6c626-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="6c626-117">seriesAxis</span></span>|[<span data-ttu-id="6c626-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="6c626-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="6c626-p102">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6c626-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="6c626-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="6c626-121">valueAxis</span></span>|[<span data-ttu-id="6c626-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="6c626-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="6c626-p103">軸の数値軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6c626-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c626-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c626-125">JSON representation</span></span>

<span data-ttu-id="6c626-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c626-126">Here is a JSON representation of the resource.</span></span>

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
