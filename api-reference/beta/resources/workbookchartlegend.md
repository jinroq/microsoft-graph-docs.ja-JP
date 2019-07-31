---
title: workbookChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 42414f0089cf3e33529796ebbeb53b95bc1d4ef2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964040"
---
# <a name="workbookchartlegend-resource-type"></a><span data-ttu-id="3cdad-103">workbookChartLegend リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3cdad-103">workbookChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cdad-104">グラフに凡例を表します。</span><span class="sxs-lookup"><span data-stu-id="3cdad-104">Represents the legend in a chart.</span></span>

## <a name="methods"></a><span data-ttu-id="3cdad-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="3cdad-105">Methods</span></span>

| <span data-ttu-id="3cdad-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3cdad-106">Method</span></span>           | <span data-ttu-id="3cdad-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3cdad-107">Return Type</span></span>    |<span data-ttu-id="3cdad-108">説明</span><span class="sxs-lookup"><span data-stu-id="3cdad-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3cdad-109">WorkbookChartLegend を取得する</span><span class="sxs-lookup"><span data-stu-id="3cdad-109">Get workbookChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="3cdad-110">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="3cdad-110">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="3cdad-111">chartLegend オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3cdad-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="3cdad-112">Update</span><span class="sxs-lookup"><span data-stu-id="3cdad-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="3cdad-113">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="3cdad-113">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="3cdad-114">ChartLegend オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3cdad-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3cdad-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cdad-115">Properties</span></span>
| <span data-ttu-id="3cdad-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cdad-116">Property</span></span>     | <span data-ttu-id="3cdad-117">型</span><span class="sxs-lookup"><span data-stu-id="3cdad-117">Type</span></span>   |<span data-ttu-id="3cdad-118">説明</span><span class="sxs-lookup"><span data-stu-id="3cdad-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cdad-119">overlay</span><span class="sxs-lookup"><span data-stu-id="3cdad-119">overlay</span></span>|<span data-ttu-id="3cdad-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="3cdad-120">boolean</span></span>|<span data-ttu-id="3cdad-121">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="3cdad-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="3cdad-122">position</span><span class="sxs-lookup"><span data-stu-id="3cdad-122">position</span></span>|<span data-ttu-id="3cdad-123">string</span><span class="sxs-lookup"><span data-stu-id="3cdad-123">string</span></span>|<span data-ttu-id="3cdad-124">グラフの凡例の位置を表します。</span><span class="sxs-lookup"><span data-stu-id="3cdad-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="3cdad-125">使用可能な値: `Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="3cdad-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="3cdad-126">visible</span><span class="sxs-lookup"><span data-stu-id="3cdad-126">visible</span></span>|<span data-ttu-id="3cdad-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="3cdad-127">boolean</span></span>|<span data-ttu-id="3cdad-128">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="3cdad-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cdad-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3cdad-129">Relationships</span></span>
| <span data-ttu-id="3cdad-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3cdad-130">Relationship</span></span> | <span data-ttu-id="3cdad-131">型</span><span class="sxs-lookup"><span data-stu-id="3cdad-131">Type</span></span>   |<span data-ttu-id="3cdad-132">説明</span><span class="sxs-lookup"><span data-stu-id="3cdad-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cdad-133">format</span><span class="sxs-lookup"><span data-stu-id="3cdad-133">format</span></span>|[<span data-ttu-id="3cdad-134">workbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="3cdad-134">workbookChartLegendFormat</span></span>](workbookchartlegendformat.md)|<span data-ttu-id="3cdad-135">塗りつぶしとフォントの書式設定を含む、グラフの凡例の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="3cdad-135">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="3cdad-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3cdad-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cdad-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3cdad-137">JSON representation</span></span>

<span data-ttu-id="3cdad-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3cdad-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "format"        
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
