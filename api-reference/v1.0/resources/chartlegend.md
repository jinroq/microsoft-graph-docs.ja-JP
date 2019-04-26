---
title: ChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8eea71707d622f0dc28cc8072fa984de64a8427f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569103"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="b9c56-103">ChartLegend リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9c56-103">ChartLegend resource type</span></span>

<span data-ttu-id="b9c56-104">グラフに凡例を表します。</span><span class="sxs-lookup"><span data-stu-id="b9c56-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="b9c56-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b9c56-105">Methods</span></span>

| <span data-ttu-id="b9c56-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b9c56-106">Method</span></span>           | <span data-ttu-id="b9c56-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b9c56-107">Return Type</span></span>    |<span data-ttu-id="b9c56-108">説明</span><span class="sxs-lookup"><span data-stu-id="b9c56-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b9c56-109">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="b9c56-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="b9c56-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="b9c56-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="b9c56-111">chartLegend オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b9c56-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="b9c56-112">Update</span><span class="sxs-lookup"><span data-stu-id="b9c56-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="b9c56-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="b9c56-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="b9c56-114">ChartLegend オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b9c56-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b9c56-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9c56-115">Properties</span></span>
| <span data-ttu-id="b9c56-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9c56-116">Property</span></span>     | <span data-ttu-id="b9c56-117">型</span><span class="sxs-lookup"><span data-stu-id="b9c56-117">Type</span></span>   |<span data-ttu-id="b9c56-118">説明</span><span class="sxs-lookup"><span data-stu-id="b9c56-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9c56-119">overlay</span><span class="sxs-lookup"><span data-stu-id="b9c56-119">overlay</span></span>|<span data-ttu-id="b9c56-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="b9c56-120">boolean</span></span>|<span data-ttu-id="b9c56-121">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="b9c56-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="b9c56-122">position</span><span class="sxs-lookup"><span data-stu-id="b9c56-122">position</span></span>|<span data-ttu-id="b9c56-123">string</span><span class="sxs-lookup"><span data-stu-id="b9c56-123">string</span></span>|<span data-ttu-id="b9c56-124">グラフの凡例の位置を表します。</span><span class="sxs-lookup"><span data-stu-id="b9c56-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="b9c56-125">使用可能な値は`Top`、 `Bottom`、 `Left` `Right` `Corner`、、、 `Custom`、です。</span><span class="sxs-lookup"><span data-stu-id="b9c56-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="b9c56-126">visible</span><span class="sxs-lookup"><span data-stu-id="b9c56-126">visible</span></span>|<span data-ttu-id="b9c56-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="b9c56-127">boolean</span></span>|<span data-ttu-id="b9c56-128">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="b9c56-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9c56-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b9c56-129">Relationships</span></span>
| <span data-ttu-id="b9c56-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b9c56-130">Relationship</span></span> | <span data-ttu-id="b9c56-131">型</span><span class="sxs-lookup"><span data-stu-id="b9c56-131">Type</span></span>   |<span data-ttu-id="b9c56-132">説明</span><span class="sxs-lookup"><span data-stu-id="b9c56-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9c56-133">format</span><span class="sxs-lookup"><span data-stu-id="b9c56-133">format</span></span>|[<span data-ttu-id="b9c56-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="b9c56-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="b9c56-135">塗りつぶしとフォントの書式設定を含む、グラフの凡例の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="b9c56-135">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="b9c56-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b9c56-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9c56-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9c56-137">JSON representation</span></span>

<span data-ttu-id="b9c56-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b9c56-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
