---
title: グラフ リソースの種類
description: ブック内のグラフ オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d274b8ec505d15ea985af22627232dbe11dc3263
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856050"
---
# <a name="chart-resource-type"></a><span data-ttu-id="b8937-103">グラフ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8937-103">Chart resource type</span></span>

> <span data-ttu-id="b8937-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8937-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8937-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8937-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8937-106">ブック内のグラフ オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="b8937-106">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="b8937-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8937-107">Methods</span></span>

| <span data-ttu-id="b8937-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8937-108">Method</span></span>           | <span data-ttu-id="b8937-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8937-109">Return Type</span></span>    |<span data-ttu-id="b8937-110">説明</span><span class="sxs-lookup"><span data-stu-id="b8937-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8937-111">Get Chart</span><span class="sxs-lookup"><span data-stu-id="b8937-111">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="b8937-112">Chart</span><span class="sxs-lookup"><span data-stu-id="b8937-112">Chart</span></span>](chart.md) |<span data-ttu-id="b8937-113">グラフ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b8937-113">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="b8937-114">ChartSeries を作成する</span><span class="sxs-lookup"><span data-stu-id="b8937-114">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="b8937-115">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="b8937-115">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="b8937-116">データ系列のコレクションに投稿して、新しい ChartSeries を作成します。</span><span class="sxs-lookup"><span data-stu-id="b8937-116">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="b8937-117">データ系列を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b8937-117">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="b8937-118">[ChartSeries](chartseries.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8937-118">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="b8937-119">ChartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b8937-119">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="b8937-120">Update</span><span class="sxs-lookup"><span data-stu-id="b8937-120">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="b8937-121">Chart</span><span class="sxs-lookup"><span data-stu-id="b8937-121">Chart</span></span>](chart.md)   |<span data-ttu-id="b8937-122">グラフ オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8937-122">Update Chart object.</span></span> |
|[<span data-ttu-id="b8937-123">Image</span><span class="sxs-lookup"><span data-stu-id="b8937-123">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="b8937-124">Base64 でエンコードされた文字列の画像</span><span class="sxs-lookup"><span data-stu-id="b8937-124">Image base64 encoded string</span></span>|<span data-ttu-id="b8937-125">指定したサイズに合わせてグラフを拡大・縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="b8937-125">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="b8937-126">Delete</span><span class="sxs-lookup"><span data-stu-id="b8937-126">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="b8937-127">なし</span><span class="sxs-lookup"><span data-stu-id="b8937-127">None</span></span>|<span data-ttu-id="b8937-128">グラフ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="b8937-128">Deletes the chart object.</span></span>|
|[<span data-ttu-id="b8937-129">Setdata</span><span class="sxs-lookup"><span data-stu-id="b8937-129">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="b8937-130">なし</span><span class="sxs-lookup"><span data-stu-id="b8937-130">None</span></span>|<span data-ttu-id="b8937-131">グラフの元データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="b8937-131">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="b8937-132">Setposition</span><span class="sxs-lookup"><span data-stu-id="b8937-132">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="b8937-133">なし</span><span class="sxs-lookup"><span data-stu-id="b8937-133">None</span></span>|<span data-ttu-id="b8937-134">ワークシート上のセルを基準にしてグラフを配置します。</span><span class="sxs-lookup"><span data-stu-id="b8937-134">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="b8937-135">List</span><span class="sxs-lookup"><span data-stu-id="b8937-135">List</span></span>](../api/chart-list.md) | <span data-ttu-id="b8937-136">[Chart](chart.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8937-136">[Chart](chart.md) collection</span></span> |<span data-ttu-id="b8937-137">グラフ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b8937-137">Get chart object collection.</span></span> |
|[<span data-ttu-id="b8937-138">Itemat</span><span class="sxs-lookup"><span data-stu-id="b8937-138">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="b8937-139">Chart</span><span class="sxs-lookup"><span data-stu-id="b8937-139">Chart</span></span>](chart.md)|<span data-ttu-id="b8937-140">コレクション内の位置に基づいて、グラフを取得します。</span><span class="sxs-lookup"><span data-stu-id="b8937-140">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="b8937-141">Add</span><span class="sxs-lookup"><span data-stu-id="b8937-141">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="b8937-142">Chart</span><span class="sxs-lookup"><span data-stu-id="b8937-142">Chart</span></span>](chart.md)|<span data-ttu-id="b8937-143">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="b8937-143">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8937-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8937-144">Properties</span></span>
| <span data-ttu-id="b8937-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8937-145">Property</span></span>     | <span data-ttu-id="b8937-146">種類</span><span class="sxs-lookup"><span data-stu-id="b8937-146">Type</span></span>   |<span data-ttu-id="b8937-147">説明</span><span class="sxs-lookup"><span data-stu-id="b8937-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8937-148">height</span><span class="sxs-lookup"><span data-stu-id="b8937-148">height</span></span>|<span data-ttu-id="b8937-149">double</span><span class="sxs-lookup"><span data-stu-id="b8937-149">double</span></span>|<span data-ttu-id="b8937-150">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="b8937-150">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="b8937-151">ID</span><span class="sxs-lookup"><span data-stu-id="b8937-151">id</span></span>|<span data-ttu-id="b8937-152">文字列</span><span class="sxs-lookup"><span data-stu-id="b8937-152">string</span></span>|<span data-ttu-id="b8937-p102">コレクション内での位置を基にグラフを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8937-p102">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="b8937-155">left</span><span class="sxs-lookup"><span data-stu-id="b8937-155">left</span></span>|<span data-ttu-id="b8937-156">double</span><span class="sxs-lookup"><span data-stu-id="b8937-156">double</span></span>|<span data-ttu-id="b8937-157">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="b8937-157">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="b8937-158">name</span><span class="sxs-lookup"><span data-stu-id="b8937-158">name</span></span>|<span data-ttu-id="b8937-159">文字列</span><span class="sxs-lookup"><span data-stu-id="b8937-159">string</span></span>|<span data-ttu-id="b8937-160"> グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="b8937-160">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="b8937-161">top</span><span class="sxs-lookup"><span data-stu-id="b8937-161">top</span></span>|<span data-ttu-id="b8937-162">double</span><span class="sxs-lookup"><span data-stu-id="b8937-162">double</span></span>|<span data-ttu-id="b8937-163">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="b8937-163">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="b8937-164">width</span><span class="sxs-lookup"><span data-stu-id="b8937-164">width</span></span>|<span data-ttu-id="b8937-165">double</span><span class="sxs-lookup"><span data-stu-id="b8937-165">double</span></span>|<span data-ttu-id="b8937-166">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="b8937-166">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8937-167">関係</span><span class="sxs-lookup"><span data-stu-id="b8937-167">Relationships</span></span>
| <span data-ttu-id="b8937-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8937-168">Relationship</span></span> | <span data-ttu-id="b8937-169">型</span><span class="sxs-lookup"><span data-stu-id="b8937-169">Type</span></span>   |<span data-ttu-id="b8937-170">説明</span><span class="sxs-lookup"><span data-stu-id="b8937-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8937-171">axes</span><span class="sxs-lookup"><span data-stu-id="b8937-171">axes</span></span>|[<span data-ttu-id="b8937-172">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="b8937-172">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="b8937-p103">グラフの軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b8937-p103">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="b8937-175">dataLabels</span><span class="sxs-lookup"><span data-stu-id="b8937-175">dataLabels</span></span>|[<span data-ttu-id="b8937-176">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="b8937-176">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="b8937-p104">グラフのデータラベルを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b8937-p104">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="b8937-179">format</span><span class="sxs-lookup"><span data-stu-id="b8937-179">format</span></span>|[<span data-ttu-id="b8937-180">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="b8937-180">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="b8937-p105">グラフ領域の書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b8937-p105">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="b8937-183">legend</span><span class="sxs-lookup"><span data-stu-id="b8937-183">legend</span></span>|[<span data-ttu-id="b8937-184">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="b8937-184">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="b8937-p106">グラフの凡例を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b8937-p106">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="b8937-187">series</span><span class="sxs-lookup"><span data-stu-id="b8937-187">series</span></span>|<span data-ttu-id="b8937-188">[ChartSeries](chartseries.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8937-188">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="b8937-p107">グラフの 1 つのデータ系列またはデータ系列のコレクションを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b8937-p107">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="b8937-191">役職</span><span class="sxs-lookup"><span data-stu-id="b8937-191">title</span></span>|[<span data-ttu-id="b8937-192">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="b8937-192">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="b8937-p108">指定したグラフのタイトル (タイトルのテキスト、表示/非表示、位置、書式設定など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b8937-p108">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="b8937-195">worksheet</span><span class="sxs-lookup"><span data-stu-id="b8937-195">worksheet</span></span>|[<span data-ttu-id="b8937-196">Worksheet</span><span class="sxs-lookup"><span data-stu-id="b8937-196">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="b8937-p109">現在のグラフを含んでいるワークシート。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b8937-p109">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8937-199">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8937-199">JSON representation</span></span>

<span data-ttu-id="b8937-200">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8937-200">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
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
