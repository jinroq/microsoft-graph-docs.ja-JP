---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 483a69f11425f3b8991305e6acdf6b970d0e2db1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976388"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="3aee0-103">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3aee0-103">ChartAxes resource type</span></span>

<span data-ttu-id="3aee0-104">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="3aee0-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="3aee0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="3aee0-105">Methods</span></span>
<span data-ttu-id="3aee0-106">なし</span><span class="sxs-lookup"><span data-stu-id="3aee0-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="3aee0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3aee0-107">Properties</span></span>
<span data-ttu-id="3aee0-108">なし</span><span class="sxs-lookup"><span data-stu-id="3aee0-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3aee0-109">関係</span><span class="sxs-lookup"><span data-stu-id="3aee0-109">Relationships</span></span>
| <span data-ttu-id="3aee0-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3aee0-110">Relationship</span></span> | <span data-ttu-id="3aee0-111">型</span><span class="sxs-lookup"><span data-stu-id="3aee0-111">Type</span></span>   |<span data-ttu-id="3aee0-112">説明</span><span class="sxs-lookup"><span data-stu-id="3aee0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3aee0-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="3aee0-113">categoryAxis</span></span>|[<span data-ttu-id="3aee0-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="3aee0-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="3aee0-p101">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3aee0-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="3aee0-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="3aee0-117">seriesAxis</span></span>|[<span data-ttu-id="3aee0-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="3aee0-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="3aee0-p102">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3aee0-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="3aee0-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="3aee0-121">valueAxis</span></span>|[<span data-ttu-id="3aee0-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="3aee0-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="3aee0-p103">軸の数値軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3aee0-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3aee0-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3aee0-125">JSON representation</span></span>

<span data-ttu-id="3aee0-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3aee0-126">Here is a JSON representation of the resource.</span></span>

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
