---
title: ChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 13c054403eb93afce03775138c151e67bc2f57d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528187"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="c6ee0-103">ChartLegend リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6ee0-103">ChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6ee0-104">グラフに凡例を表します。</span><span class="sxs-lookup"><span data-stu-id="c6ee0-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c6ee0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6ee0-105">Methods</span></span>

| <span data-ttu-id="c6ee0-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6ee0-106">Method</span></span>           | <span data-ttu-id="c6ee0-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c6ee0-107">Return Type</span></span>    |<span data-ttu-id="c6ee0-108">説明</span><span class="sxs-lookup"><span data-stu-id="c6ee0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6ee0-109">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="c6ee0-109">[Get ChartLegend](../api/chartlegend-get.md)</span></span> | [<span data-ttu-id="c6ee0-110">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="c6ee0-110">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="c6ee0-111">chartLegend オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c6ee0-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="c6ee0-112">Update</span><span class="sxs-lookup"><span data-stu-id="c6ee0-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="c6ee0-113">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="c6ee0-113">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="c6ee0-114">ChartLegend オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c6ee0-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6ee0-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6ee0-115">Properties</span></span>
| <span data-ttu-id="c6ee0-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6ee0-116">Property</span></span>     | <span data-ttu-id="c6ee0-117">型</span><span class="sxs-lookup"><span data-stu-id="c6ee0-117">Type</span></span>   |<span data-ttu-id="c6ee0-118">説明</span><span class="sxs-lookup"><span data-stu-id="c6ee0-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6ee0-119">overlay</span><span class="sxs-lookup"><span data-stu-id="c6ee0-119">overlay</span></span>|<span data-ttu-id="c6ee0-120">boolean</span><span class="sxs-lookup"><span data-stu-id="c6ee0-120">boolean</span></span>|<span data-ttu-id="c6ee0-121">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="c6ee0-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="c6ee0-122">position</span><span class="sxs-lookup"><span data-stu-id="c6ee0-122">position</span></span>|<span data-ttu-id="c6ee0-123">文字列</span><span class="sxs-lookup"><span data-stu-id="c6ee0-123">string</span></span>|<span data-ttu-id="c6ee0-p101">グラフの凡例の位置を表します。可能な値は、`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom` です。</span><span class="sxs-lookup"><span data-stu-id="c6ee0-p101">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="c6ee0-126">visible</span><span class="sxs-lookup"><span data-stu-id="c6ee0-126">visible</span></span>|<span data-ttu-id="c6ee0-127">boolean</span><span class="sxs-lookup"><span data-stu-id="c6ee0-127">boolean</span></span>|<span data-ttu-id="c6ee0-128">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="c6ee0-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6ee0-129">関係</span><span class="sxs-lookup"><span data-stu-id="c6ee0-129">Relationships</span></span>
| <span data-ttu-id="c6ee0-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6ee0-130">Relationship</span></span> | <span data-ttu-id="c6ee0-131">型</span><span class="sxs-lookup"><span data-stu-id="c6ee0-131">Type</span></span>   |<span data-ttu-id="c6ee0-132">説明</span><span class="sxs-lookup"><span data-stu-id="c6ee0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6ee0-133">format</span><span class="sxs-lookup"><span data-stu-id="c6ee0-133">format</span></span>|[<span data-ttu-id="c6ee0-134">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="c6ee0-134">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="c6ee0-p102">グラフ の凡例の書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c6ee0-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6ee0-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6ee0-137">JSON representation</span></span>

<span data-ttu-id="c6ee0-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c6ee0-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true
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
