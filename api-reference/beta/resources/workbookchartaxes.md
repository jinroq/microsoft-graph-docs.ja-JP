---
title: workbookChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 15e63af1e7b648288dba813790302f1dee6536ba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348850"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="2a938-103">workbookChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a938-103">workbookChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a938-104">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="2a938-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="2a938-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a938-105">Methods</span></span>
<span data-ttu-id="2a938-106">なし</span><span class="sxs-lookup"><span data-stu-id="2a938-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="2a938-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a938-107">Properties</span></span>
<span data-ttu-id="2a938-108">なし</span><span class="sxs-lookup"><span data-stu-id="2a938-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="2a938-109">関係</span><span class="sxs-lookup"><span data-stu-id="2a938-109">Relationships</span></span>
| <span data-ttu-id="2a938-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a938-110">Relationship</span></span> | <span data-ttu-id="2a938-111">型</span><span class="sxs-lookup"><span data-stu-id="2a938-111">Type</span></span>   |<span data-ttu-id="2a938-112">説明</span><span class="sxs-lookup"><span data-stu-id="2a938-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a938-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="2a938-113">categoryAxis</span></span>|[<span data-ttu-id="2a938-114">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="2a938-114">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="2a938-p101">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2a938-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="2a938-117">系列軸</span><span class="sxs-lookup"><span data-stu-id="2a938-117">seriesAxis</span></span>|[<span data-ttu-id="2a938-118">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="2a938-118">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="2a938-p102">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2a938-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="2a938-121">数値軸</span><span class="sxs-lookup"><span data-stu-id="2a938-121">valueAxis</span></span>|[<span data-ttu-id="2a938-122">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="2a938-122">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="2a938-123">軸の数値軸を表します。</span><span class="sxs-lookup"><span data-stu-id="2a938-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="2a938-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2a938-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a938-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a938-125">JSON representation</span></span>

<span data-ttu-id="2a938-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a938-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
