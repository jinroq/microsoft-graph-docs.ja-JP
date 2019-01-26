---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2a3744e38ffebef0c28784c0fd4be8f35b8af23
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570863"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="8b303-103">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b303-103">ChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b303-104">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="8b303-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="8b303-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8b303-105">Methods</span></span>
<span data-ttu-id="8b303-106">なし</span><span class="sxs-lookup"><span data-stu-id="8b303-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="8b303-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b303-107">Properties</span></span>
<span data-ttu-id="8b303-108">なし</span><span class="sxs-lookup"><span data-stu-id="8b303-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8b303-109">関係</span><span class="sxs-lookup"><span data-stu-id="8b303-109">Relationships</span></span>
| <span data-ttu-id="8b303-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8b303-110">Relationship</span></span> | <span data-ttu-id="8b303-111">型</span><span class="sxs-lookup"><span data-stu-id="8b303-111">Type</span></span>   |<span data-ttu-id="8b303-112">説明</span><span class="sxs-lookup"><span data-stu-id="8b303-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b303-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="8b303-113">categoryAxis</span></span>|[<span data-ttu-id="8b303-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="8b303-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="8b303-p101">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8b303-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="8b303-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="8b303-117">seriesAxis</span></span>|[<span data-ttu-id="8b303-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="8b303-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="8b303-p102">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8b303-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="8b303-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="8b303-121">valueAxis</span></span>|[<span data-ttu-id="8b303-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="8b303-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="8b303-p103">軸の数値軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8b303-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b303-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b303-125">JSON representation</span></span>

<span data-ttu-id="8b303-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b303-126">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
