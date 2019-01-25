---
title: グラフ リソースの種類
description: ブック内のグラフ オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529524"
---
# <a name="chart-resource-type"></a><span data-ttu-id="38a15-103">グラフ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38a15-103">Chart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a15-104">ブック内のグラフ オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="38a15-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="38a15-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="38a15-105">Methods</span></span>

| <span data-ttu-id="38a15-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="38a15-106">Method</span></span>           | <span data-ttu-id="38a15-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="38a15-107">Return Type</span></span>    |<span data-ttu-id="38a15-108">説明</span><span class="sxs-lookup"><span data-stu-id="38a15-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38a15-109">Get Chart</span><span class="sxs-lookup"><span data-stu-id="38a15-109">[Get Chart](../api/chart-get.md)</span></span> | [<span data-ttu-id="38a15-110">Chart</span><span class="sxs-lookup"><span data-stu-id="38a15-110">Chart</span></span>](chart.md) |<span data-ttu-id="38a15-111">グラフ オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="38a15-111">Read properties and relationships of chart object.</span></span>|
|<span data-ttu-id="38a15-112">ChartSeries を作成する</span><span class="sxs-lookup"><span data-stu-id="38a15-112">[Create ChartSeries](../api/chart-post-series.md)</span></span> |<span data-ttu-id="38a15-113">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="38a15-113">[ChartSeries](chartseries.md)</span></span>| <span data-ttu-id="38a15-114">データ系列のコレクションに投稿して、新しい ChartSeries を作成します。</span><span class="sxs-lookup"><span data-stu-id="38a15-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|<span data-ttu-id="38a15-115">データ系列を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="38a15-115">[List series](../api/chart-list-series.md)</span></span> |<span data-ttu-id="38a15-116">ChartSeries コレクション</span><span class="sxs-lookup"><span data-stu-id="38a15-116">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="38a15-117">ChartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="38a15-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="38a15-118">Update</span><span class="sxs-lookup"><span data-stu-id="38a15-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="38a15-119">Chart</span><span class="sxs-lookup"><span data-stu-id="38a15-119">Chart</span></span>](chart.md)   |<span data-ttu-id="38a15-120">グラフ オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="38a15-120">Update Chart object.</span></span> |
|[<span data-ttu-id="38a15-121">Image</span><span class="sxs-lookup"><span data-stu-id="38a15-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="38a15-122">Base64 でエンコードされた文字列の画像</span><span class="sxs-lookup"><span data-stu-id="38a15-122">Image base64 encoded string</span></span>|<span data-ttu-id="38a15-123">指定したサイズに合わせてグラフを拡大・縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="38a15-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="38a15-124">Delete</span><span class="sxs-lookup"><span data-stu-id="38a15-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="38a15-125">なし</span><span class="sxs-lookup"><span data-stu-id="38a15-125">None</span></span>|<span data-ttu-id="38a15-126">グラフ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="38a15-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="38a15-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="38a15-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="38a15-128">なし</span><span class="sxs-lookup"><span data-stu-id="38a15-128">None</span></span>|<span data-ttu-id="38a15-129">グラフの元データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="38a15-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="38a15-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="38a15-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="38a15-131">なし</span><span class="sxs-lookup"><span data-stu-id="38a15-131">None</span></span>|<span data-ttu-id="38a15-132">ワークシート上のセルを基準にしてグラフを配置します。</span><span class="sxs-lookup"><span data-stu-id="38a15-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="38a15-133">List</span><span class="sxs-lookup"><span data-stu-id="38a15-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="38a15-134">Chart コレクション</span><span class="sxs-lookup"><span data-stu-id="38a15-134">[Chart](chart.md) collection</span></span> |<span data-ttu-id="38a15-135">グラフ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="38a15-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="38a15-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="38a15-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="38a15-137">Chart</span><span class="sxs-lookup"><span data-stu-id="38a15-137">Chart</span></span>](chart.md)|<span data-ttu-id="38a15-138">コレクション内の位置に基づいて、グラフを取得します。</span><span class="sxs-lookup"><span data-stu-id="38a15-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="38a15-139">Add</span><span class="sxs-lookup"><span data-stu-id="38a15-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="38a15-140">Chart</span><span class="sxs-lookup"><span data-stu-id="38a15-140">Chart</span></span>](chart.md)|<span data-ttu-id="38a15-141">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="38a15-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="38a15-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38a15-142">Properties</span></span>
| <span data-ttu-id="38a15-143">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38a15-143">Property</span></span>     | <span data-ttu-id="38a15-144">型</span><span class="sxs-lookup"><span data-stu-id="38a15-144">Type</span></span>   |<span data-ttu-id="38a15-145">説明</span><span class="sxs-lookup"><span data-stu-id="38a15-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38a15-146">height</span><span class="sxs-lookup"><span data-stu-id="38a15-146">height</span></span>|<span data-ttu-id="38a15-147">double</span><span class="sxs-lookup"><span data-stu-id="38a15-147">double</span></span>|<span data-ttu-id="38a15-148">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="38a15-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="38a15-149">id</span><span class="sxs-lookup"><span data-stu-id="38a15-149">id</span></span>|<span data-ttu-id="38a15-150">文字列</span><span class="sxs-lookup"><span data-stu-id="38a15-150">string</span></span>|<span data-ttu-id="38a15-p101">コレクション内での位置を基にグラフを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="38a15-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="38a15-153">left</span><span class="sxs-lookup"><span data-stu-id="38a15-153">left</span></span>|<span data-ttu-id="38a15-154">double</span><span class="sxs-lookup"><span data-stu-id="38a15-154">double</span></span>|<span data-ttu-id="38a15-155">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="38a15-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="38a15-156">name</span><span class="sxs-lookup"><span data-stu-id="38a15-156">name</span></span>|<span data-ttu-id="38a15-157">文字列</span><span class="sxs-lookup"><span data-stu-id="38a15-157">string</span></span>|<span data-ttu-id="38a15-158"> グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="38a15-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="38a15-159">top</span><span class="sxs-lookup"><span data-stu-id="38a15-159">top</span></span>|<span data-ttu-id="38a15-160">double</span><span class="sxs-lookup"><span data-stu-id="38a15-160">double</span></span>|<span data-ttu-id="38a15-161">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="38a15-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="38a15-162">width</span><span class="sxs-lookup"><span data-stu-id="38a15-162">width</span></span>|<span data-ttu-id="38a15-163">double</span><span class="sxs-lookup"><span data-stu-id="38a15-163">double</span></span>|<span data-ttu-id="38a15-164">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="38a15-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38a15-165">関係</span><span class="sxs-lookup"><span data-stu-id="38a15-165">Relationships</span></span>
| <span data-ttu-id="38a15-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="38a15-166">Relationship</span></span> | <span data-ttu-id="38a15-167">型</span><span class="sxs-lookup"><span data-stu-id="38a15-167">Type</span></span>   |<span data-ttu-id="38a15-168">説明</span><span class="sxs-lookup"><span data-stu-id="38a15-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38a15-169">axes</span><span class="sxs-lookup"><span data-stu-id="38a15-169">axes</span></span>|[<span data-ttu-id="38a15-170">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="38a15-170">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="38a15-p102">グラフの軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="38a15-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="38a15-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="38a15-173">dataLabels</span></span>|[<span data-ttu-id="38a15-174">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="38a15-174">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="38a15-p103">グラフのデータラベルを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="38a15-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="38a15-177">format</span><span class="sxs-lookup"><span data-stu-id="38a15-177">format</span></span>|[<span data-ttu-id="38a15-178">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="38a15-178">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="38a15-p104">グラフ領域の書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="38a15-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="38a15-181">legend</span><span class="sxs-lookup"><span data-stu-id="38a15-181">legend</span></span>|[<span data-ttu-id="38a15-182">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="38a15-182">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="38a15-p105">グラフの凡例を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="38a15-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="38a15-185">series</span><span class="sxs-lookup"><span data-stu-id="38a15-185">series</span></span>|<span data-ttu-id="38a15-186">[ChartSeries](chartseries.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="38a15-186">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="38a15-p106">グラフの 1 つのデータ系列またはデータ系列のコレクションを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="38a15-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="38a15-189">役職</span><span class="sxs-lookup"><span data-stu-id="38a15-189">title</span></span>|[<span data-ttu-id="38a15-190">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="38a15-190">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="38a15-p107">指定したグラフのタイトル (タイトルのテキスト、表示/非表示、位置、書式設定など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="38a15-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="38a15-193">worksheet</span><span class="sxs-lookup"><span data-stu-id="38a15-193">worksheet</span></span>|[<span data-ttu-id="38a15-194">Worksheet</span><span class="sxs-lookup"><span data-stu-id="38a15-194">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="38a15-p108">現在のグラフを含んでいるワークシート。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="38a15-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38a15-197">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38a15-197">JSON representation</span></span>

<span data-ttu-id="38a15-198">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="38a15-198">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
