---
title: ChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
ms.openlocfilehash: 27dc0ea751cff47adaa077f824f619630341cdc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326090"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="06033-103">ChartLegend リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06033-103">ChartLegend resource type</span></span>

<span data-ttu-id="06033-104">グラフに凡例を表します。</span><span class="sxs-lookup"><span data-stu-id="06033-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="06033-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="06033-105">Methods</span></span>

| <span data-ttu-id="06033-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="06033-106">Method</span></span>           | <span data-ttu-id="06033-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06033-107">Return Type</span></span>    |<span data-ttu-id="06033-108">説明</span><span class="sxs-lookup"><span data-stu-id="06033-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06033-109">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="06033-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="06033-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="06033-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="06033-111">chartLegend オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="06033-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="06033-112">Update</span><span class="sxs-lookup"><span data-stu-id="06033-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="06033-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="06033-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="06033-114">ChartLegend オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="06033-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="06033-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06033-115">Properties</span></span>
| <span data-ttu-id="06033-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06033-116">Property</span></span>     | <span data-ttu-id="06033-117">種類</span><span class="sxs-lookup"><span data-stu-id="06033-117">Type</span></span>   |<span data-ttu-id="06033-118">説明</span><span class="sxs-lookup"><span data-stu-id="06033-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06033-119">overlay</span><span class="sxs-lookup"><span data-stu-id="06033-119">overlay</span></span>|<span data-ttu-id="06033-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="06033-120">boolean</span></span>|<span data-ttu-id="06033-121">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="06033-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="06033-122">position</span><span class="sxs-lookup"><span data-stu-id="06033-122">position</span></span>|<span data-ttu-id="06033-123">文字列</span><span class="sxs-lookup"><span data-stu-id="06033-123">string</span></span>|<span data-ttu-id="06033-124">グラフの凡例の位置を表します。</span><span class="sxs-lookup"><span data-stu-id="06033-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="06033-125">可能な値: `Top`、 `Bottom`、 `Left`、 `Right`、 `Corner`、 `Custom`。</span><span class="sxs-lookup"><span data-stu-id="06033-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="06033-126">visible</span><span class="sxs-lookup"><span data-stu-id="06033-126">visible</span></span>|<span data-ttu-id="06033-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="06033-127">boolean</span></span>|<span data-ttu-id="06033-128">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="06033-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06033-129">関係</span><span class="sxs-lookup"><span data-stu-id="06033-129">Relationships</span></span>
| <span data-ttu-id="06033-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06033-130">Relationship</span></span> | <span data-ttu-id="06033-131">型</span><span class="sxs-lookup"><span data-stu-id="06033-131">Type</span></span>   |<span data-ttu-id="06033-132">説明</span><span class="sxs-lookup"><span data-stu-id="06033-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06033-133">format</span><span class="sxs-lookup"><span data-stu-id="06033-133">format</span></span>|[<span data-ttu-id="06033-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="06033-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="06033-p102">グラフ の凡例の書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="06033-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06033-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06033-137">JSON representation</span></span>

<span data-ttu-id="06033-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06033-138">Here is a JSON representation of the resource.</span></span>

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