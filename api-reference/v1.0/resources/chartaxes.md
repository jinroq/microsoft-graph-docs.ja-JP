---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
ms.openlocfilehash: 4fc801ecdba147a26b30f07a2487eabe11acfb3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021120"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="e8300-103">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8300-103">ChartAxes resource type</span></span>

<span data-ttu-id="e8300-104">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="e8300-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="e8300-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8300-105">Methods</span></span>
<span data-ttu-id="e8300-106">なし</span><span class="sxs-lookup"><span data-stu-id="e8300-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e8300-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8300-107">Properties</span></span>
<span data-ttu-id="e8300-108">なし</span><span class="sxs-lookup"><span data-stu-id="e8300-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e8300-109">関係</span><span class="sxs-lookup"><span data-stu-id="e8300-109">Relationships</span></span>
| <span data-ttu-id="e8300-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8300-110">Relationship</span></span> | <span data-ttu-id="e8300-111">型</span><span class="sxs-lookup"><span data-stu-id="e8300-111">Type</span></span>   |<span data-ttu-id="e8300-112">説明</span><span class="sxs-lookup"><span data-stu-id="e8300-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8300-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="e8300-113">categoryAxis</span></span>|[<span data-ttu-id="e8300-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="e8300-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="e8300-p101">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e8300-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="e8300-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="e8300-117">seriesAxis</span></span>|[<span data-ttu-id="e8300-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="e8300-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="e8300-p102">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e8300-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="e8300-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="e8300-121">valueAxis</span></span>|[<span data-ttu-id="e8300-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="e8300-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="e8300-p103">軸の数値軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e8300-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8300-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8300-125">JSON representation</span></span>

<span data-ttu-id="e8300-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8300-126">Here is a JSON representation of the resource.</span></span>

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