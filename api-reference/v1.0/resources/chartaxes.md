---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
ms.openlocfilehash: 23a9a5cc1f9eaa9a4ff222cf18f00953d829f88a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352977"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="59917-103">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59917-103">ChartAxes resource type</span></span>

<span data-ttu-id="59917-104">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="59917-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="59917-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="59917-105">Methods</span></span>
<span data-ttu-id="59917-106">なし</span><span class="sxs-lookup"><span data-stu-id="59917-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="59917-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59917-107">Properties</span></span>
<span data-ttu-id="59917-108">なし</span><span class="sxs-lookup"><span data-stu-id="59917-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="59917-109">関係</span><span class="sxs-lookup"><span data-stu-id="59917-109">Relationships</span></span>
| <span data-ttu-id="59917-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59917-110">Relationship</span></span> | <span data-ttu-id="59917-111">型</span><span class="sxs-lookup"><span data-stu-id="59917-111">Type</span></span>   |<span data-ttu-id="59917-112">説明</span><span class="sxs-lookup"><span data-stu-id="59917-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59917-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="59917-113">categoryAxis</span></span>|[<span data-ttu-id="59917-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="59917-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="59917-p101">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="59917-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="59917-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="59917-117">seriesAxis</span></span>|[<span data-ttu-id="59917-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="59917-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="59917-p102">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="59917-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="59917-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="59917-121">valueAxis</span></span>|[<span data-ttu-id="59917-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="59917-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="59917-p103">軸の数値軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="59917-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59917-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59917-125">JSON representation</span></span>

<span data-ttu-id="59917-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59917-126">Here is a JSON representation of the resource.</span></span>

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