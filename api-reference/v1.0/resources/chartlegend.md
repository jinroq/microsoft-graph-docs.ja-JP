---
title: ChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 9bb81eef7c78d952a71b60cec787413308b10833
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813413"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="de420-103">ChartLegend リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de420-103">ChartLegend resource type</span></span>

<span data-ttu-id="de420-104">グラフに凡例を表します。</span><span class="sxs-lookup"><span data-stu-id="de420-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="de420-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="de420-105">Methods</span></span>

| <span data-ttu-id="de420-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="de420-106">Method</span></span>           | <span data-ttu-id="de420-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="de420-107">Return Type</span></span>    |<span data-ttu-id="de420-108">説明</span><span class="sxs-lookup"><span data-stu-id="de420-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de420-109">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="de420-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="de420-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="de420-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="de420-111">chartLegend オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="de420-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="de420-112">Update</span><span class="sxs-lookup"><span data-stu-id="de420-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="de420-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="de420-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="de420-114">ChartLegend オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="de420-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="de420-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de420-115">Properties</span></span>
| <span data-ttu-id="de420-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de420-116">Property</span></span>     | <span data-ttu-id="de420-117">種類</span><span class="sxs-lookup"><span data-stu-id="de420-117">Type</span></span>   |<span data-ttu-id="de420-118">説明</span><span class="sxs-lookup"><span data-stu-id="de420-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de420-119">overlay</span><span class="sxs-lookup"><span data-stu-id="de420-119">overlay</span></span>|<span data-ttu-id="de420-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="de420-120">boolean</span></span>|<span data-ttu-id="de420-121">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="de420-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="de420-122">position</span><span class="sxs-lookup"><span data-stu-id="de420-122">position</span></span>|<span data-ttu-id="de420-123">文字列</span><span class="sxs-lookup"><span data-stu-id="de420-123">string</span></span>|<span data-ttu-id="de420-124">グラフの凡例の位置を表します。</span><span class="sxs-lookup"><span data-stu-id="de420-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="de420-125">可能な値: `Top`、 `Bottom`、 `Left`、 `Right`、 `Corner`、 `Custom`。</span><span class="sxs-lookup"><span data-stu-id="de420-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="de420-126">visible</span><span class="sxs-lookup"><span data-stu-id="de420-126">visible</span></span>|<span data-ttu-id="de420-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="de420-127">boolean</span></span>|<span data-ttu-id="de420-128">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="de420-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de420-129">関係</span><span class="sxs-lookup"><span data-stu-id="de420-129">Relationships</span></span>
| <span data-ttu-id="de420-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de420-130">Relationship</span></span> | <span data-ttu-id="de420-131">型</span><span class="sxs-lookup"><span data-stu-id="de420-131">Type</span></span>   |<span data-ttu-id="de420-132">説明</span><span class="sxs-lookup"><span data-stu-id="de420-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de420-133">format</span><span class="sxs-lookup"><span data-stu-id="de420-133">format</span></span>|[<span data-ttu-id="de420-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="de420-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="de420-p102">グラフ の凡例の書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="de420-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de420-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de420-137">JSON representation</span></span>

<span data-ttu-id="de420-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de420-138">Here is a JSON representation of the resource.</span></span>

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
