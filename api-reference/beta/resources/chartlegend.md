---
title: ChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 88330f98b2d652d347aae703ec91fd4de8678c9d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576396"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="4c132-103">ChartLegend リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c132-103">ChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c132-104">グラフに凡例を表します。</span><span class="sxs-lookup"><span data-stu-id="4c132-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="4c132-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c132-105">Methods</span></span>

| <span data-ttu-id="4c132-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c132-106">Method</span></span>           | <span data-ttu-id="4c132-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4c132-107">Return Type</span></span>    |<span data-ttu-id="4c132-108">説明</span><span class="sxs-lookup"><span data-stu-id="4c132-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c132-109">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="4c132-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="4c132-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="4c132-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="4c132-111">chartLegend オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4c132-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="4c132-112">Update</span><span class="sxs-lookup"><span data-stu-id="4c132-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="4c132-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="4c132-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="4c132-114">ChartLegend オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c132-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4c132-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c132-115">Properties</span></span>
| <span data-ttu-id="4c132-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c132-116">Property</span></span>     | <span data-ttu-id="4c132-117">型</span><span class="sxs-lookup"><span data-stu-id="4c132-117">Type</span></span>   |<span data-ttu-id="4c132-118">説明</span><span class="sxs-lookup"><span data-stu-id="4c132-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c132-119">overlay</span><span class="sxs-lookup"><span data-stu-id="4c132-119">overlay</span></span>|<span data-ttu-id="4c132-120">boolean</span><span class="sxs-lookup"><span data-stu-id="4c132-120">boolean</span></span>|<span data-ttu-id="4c132-121">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="4c132-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="4c132-122">position</span><span class="sxs-lookup"><span data-stu-id="4c132-122">position</span></span>|<span data-ttu-id="4c132-123">文字列</span><span class="sxs-lookup"><span data-stu-id="4c132-123">string</span></span>|<span data-ttu-id="4c132-124">グラフの凡例の位置を表します。</span><span class="sxs-lookup"><span data-stu-id="4c132-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="4c132-125">可能な値: `Top`、 `Bottom`、 `Left`、 `Right`、 `Corner`、 `Custom`。</span><span class="sxs-lookup"><span data-stu-id="4c132-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="4c132-126">visible</span><span class="sxs-lookup"><span data-stu-id="4c132-126">visible</span></span>|<span data-ttu-id="4c132-127">boolean</span><span class="sxs-lookup"><span data-stu-id="4c132-127">boolean</span></span>|<span data-ttu-id="4c132-128">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="4c132-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c132-129">関係</span><span class="sxs-lookup"><span data-stu-id="4c132-129">Relationships</span></span>
| <span data-ttu-id="4c132-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c132-130">Relationship</span></span> | <span data-ttu-id="4c132-131">型</span><span class="sxs-lookup"><span data-stu-id="4c132-131">Type</span></span>   |<span data-ttu-id="4c132-132">説明</span><span class="sxs-lookup"><span data-stu-id="4c132-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c132-133">format</span><span class="sxs-lookup"><span data-stu-id="4c132-133">format</span></span>|[<span data-ttu-id="4c132-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="4c132-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="4c132-p102">グラフ の凡例の書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="4c132-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c132-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c132-137">JSON representation</span></span>

<span data-ttu-id="4c132-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c132-138">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlegend.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
