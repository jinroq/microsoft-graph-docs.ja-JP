---
title: グラフ リソースの種類
description: ブック内のグラフ オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 831cea99e2eefaf87db814b149798506950bf407
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986594"
---
# <a name="chart-resource-type"></a><span data-ttu-id="db818-103">グラフ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="db818-103">Chart resource type</span></span>

<span data-ttu-id="db818-104">ブック内のグラフ オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="db818-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="db818-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="db818-105">Methods</span></span>

| <span data-ttu-id="db818-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="db818-106">Method</span></span>           | <span data-ttu-id="db818-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="db818-107">Return Type</span></span>    |<span data-ttu-id="db818-108">説明</span><span class="sxs-lookup"><span data-stu-id="db818-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db818-109">Get Chart</span><span class="sxs-lookup"><span data-stu-id="db818-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="db818-110">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="db818-110">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="db818-111">グラフ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="db818-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="db818-112">ChartSeries を作成する</span><span class="sxs-lookup"><span data-stu-id="db818-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="db818-113">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="db818-113">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="db818-114">データ系列のコレクションに投稿して、新しい ChartSeries を作成します。</span><span class="sxs-lookup"><span data-stu-id="db818-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="db818-115">データ系列を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="db818-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="db818-116">[WorkbookChartSeries](chartseries.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="db818-116">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="db818-117">ChartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="db818-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="db818-118">Update</span><span class="sxs-lookup"><span data-stu-id="db818-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="db818-119">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="db818-119">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="db818-120">グラフ オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="db818-120">Update Chart object.</span></span> |
|[<span data-ttu-id="db818-121">Image</span><span class="sxs-lookup"><span data-stu-id="db818-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="db818-122">Base64 でエンコードされた文字列の画像</span><span class="sxs-lookup"><span data-stu-id="db818-122">Image base64 encoded string</span></span>|<span data-ttu-id="db818-123">指定したサイズに合わせてグラフを拡大・縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="db818-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="db818-124">Delete</span><span class="sxs-lookup"><span data-stu-id="db818-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="db818-125">なし</span><span class="sxs-lookup"><span data-stu-id="db818-125">None</span></span>|<span data-ttu-id="db818-126">グラフ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="db818-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="db818-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="db818-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="db818-128">なし</span><span class="sxs-lookup"><span data-stu-id="db818-128">None</span></span>|<span data-ttu-id="db818-129">グラフの元データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="db818-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="db818-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="db818-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="db818-131">なし</span><span class="sxs-lookup"><span data-stu-id="db818-131">None</span></span>|<span data-ttu-id="db818-132">ワークシート上のセルを基準にしてグラフを配置します。</span><span class="sxs-lookup"><span data-stu-id="db818-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="db818-133">List</span><span class="sxs-lookup"><span data-stu-id="db818-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="db818-134">[WorkbookChart](chart.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="db818-134">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="db818-135">グラフ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="db818-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="db818-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="db818-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="db818-137">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="db818-137">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="db818-138">コレクション内での位置を基にグラフを取得します。</span><span class="sxs-lookup"><span data-stu-id="db818-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="db818-139">Add</span><span class="sxs-lookup"><span data-stu-id="db818-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="db818-140">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="db818-140">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="db818-141">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="db818-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="db818-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db818-142">Properties</span></span>
| <span data-ttu-id="db818-143">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db818-143">Property</span></span>     | <span data-ttu-id="db818-144">種類</span><span class="sxs-lookup"><span data-stu-id="db818-144">Type</span></span>   |<span data-ttu-id="db818-145">説明</span><span class="sxs-lookup"><span data-stu-id="db818-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db818-146">height</span><span class="sxs-lookup"><span data-stu-id="db818-146">height</span></span>|<span data-ttu-id="db818-147">double</span><span class="sxs-lookup"><span data-stu-id="db818-147">double</span></span>|<span data-ttu-id="db818-148">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="db818-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="db818-149">ID</span><span class="sxs-lookup"><span data-stu-id="db818-149">id</span></span>|<span data-ttu-id="db818-150">文字列</span><span class="sxs-lookup"><span data-stu-id="db818-150">string</span></span>|<span data-ttu-id="db818-p101">コレクション内での位置を基にグラフを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db818-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="db818-153">left</span><span class="sxs-lookup"><span data-stu-id="db818-153">left</span></span>|<span data-ttu-id="db818-154">double</span><span class="sxs-lookup"><span data-stu-id="db818-154">double</span></span>|<span data-ttu-id="db818-155">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="db818-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="db818-156">name</span><span class="sxs-lookup"><span data-stu-id="db818-156">name</span></span>|<span data-ttu-id="db818-157">文字列</span><span class="sxs-lookup"><span data-stu-id="db818-157">string</span></span>|<span data-ttu-id="db818-158"> グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="db818-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="db818-159">top</span><span class="sxs-lookup"><span data-stu-id="db818-159">top</span></span>|<span data-ttu-id="db818-160">double</span><span class="sxs-lookup"><span data-stu-id="db818-160">double</span></span>|<span data-ttu-id="db818-161">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="db818-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="db818-162">width</span><span class="sxs-lookup"><span data-stu-id="db818-162">width</span></span>|<span data-ttu-id="db818-163">double</span><span class="sxs-lookup"><span data-stu-id="db818-163">double</span></span>|<span data-ttu-id="db818-164">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="db818-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db818-165">関係</span><span class="sxs-lookup"><span data-stu-id="db818-165">Relationships</span></span>
| <span data-ttu-id="db818-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="db818-166">Relationship</span></span> | <span data-ttu-id="db818-167">型</span><span class="sxs-lookup"><span data-stu-id="db818-167">Type</span></span>   |<span data-ttu-id="db818-168">説明</span><span class="sxs-lookup"><span data-stu-id="db818-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db818-169">axes</span><span class="sxs-lookup"><span data-stu-id="db818-169">axes</span></span>|[<span data-ttu-id="db818-170">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="db818-170">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="db818-p102">グラフの軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="db818-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="db818-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="db818-173">dataLabels</span></span>|[<span data-ttu-id="db818-174">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="db818-174">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="db818-p103">グラフのデータラベルを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="db818-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="db818-177">format</span><span class="sxs-lookup"><span data-stu-id="db818-177">format</span></span>|[<span data-ttu-id="db818-178">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="db818-178">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="db818-p104">グラフ領域の書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="db818-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="db818-181">legend</span><span class="sxs-lookup"><span data-stu-id="db818-181">legend</span></span>|[<span data-ttu-id="db818-182">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="db818-182">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="db818-p105">グラフの凡例を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="db818-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="db818-185">series</span><span class="sxs-lookup"><span data-stu-id="db818-185">series</span></span>|<span data-ttu-id="db818-186">[WorkbookChartSeries](chartseries.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="db818-186">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="db818-p106">グラフの 1 つのデータ系列またはデータ系列のコレクションを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="db818-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="db818-189">役職</span><span class="sxs-lookup"><span data-stu-id="db818-189">title</span></span>|[<span data-ttu-id="db818-190">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="db818-190">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="db818-p107">指定したグラフのタイトル (タイトルのテキスト、表示/非表示、位置、書式設定など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="db818-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="db818-193">worksheet</span><span class="sxs-lookup"><span data-stu-id="db818-193">worksheet</span></span>|[<span data-ttu-id="db818-194">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="db818-194">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="db818-p108">現在のグラフを含んでいるワークシート。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="db818-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db818-197">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db818-197">JSON representation</span></span>

<span data-ttu-id="db818-198">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="db818-198">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
