---
title: ChartDataLabels リソースの種類
description: グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bda2c1849f154435608f311671026e224b0c7e3c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642325"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="0c895-103">ChartDataLabels リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c895-103">ChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c895-104">グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="0c895-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="0c895-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c895-105">Methods</span></span>

| <span data-ttu-id="0c895-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c895-106">Method</span></span>           | <span data-ttu-id="0c895-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0c895-107">Return Type</span></span>    |<span data-ttu-id="0c895-108">説明</span><span class="sxs-lookup"><span data-stu-id="0c895-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c895-109">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0c895-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="0c895-110">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0c895-110">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="0c895-111">chartDataLabels オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0c895-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="0c895-112">更新する</span><span class="sxs-lookup"><span data-stu-id="0c895-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="0c895-113">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0c895-113">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="0c895-114">ChartDataLabels オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="0c895-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c895-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c895-115">Properties</span></span>
| <span data-ttu-id="0c895-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c895-116">Property</span></span>     | <span data-ttu-id="0c895-117">型</span><span class="sxs-lookup"><span data-stu-id="0c895-117">Type</span></span>   |<span data-ttu-id="0c895-118">説明</span><span class="sxs-lookup"><span data-stu-id="0c895-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c895-119">position</span><span class="sxs-lookup"><span data-stu-id="0c895-119">position</span></span>|<span data-ttu-id="0c895-120">文字列</span><span class="sxs-lookup"><span data-stu-id="0c895-120">string</span></span>|<span data-ttu-id="0c895-p101">データ ラベルの位置を表す DataLabelPosition 値。可能な値は、`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout` です。</span><span class="sxs-lookup"><span data-stu-id="0c895-p101">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="0c895-123">separator</span><span class="sxs-lookup"><span data-stu-id="0c895-123">separator</span></span>|<span data-ttu-id="0c895-124">文字列</span><span class="sxs-lookup"><span data-stu-id="0c895-124">string</span></span>|<span data-ttu-id="0c895-125">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="0c895-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="0c895-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="0c895-126">showBubbleSize</span></span>|<span data-ttu-id="0c895-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="0c895-127">boolean</span></span>|<span data-ttu-id="0c895-128">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="0c895-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="0c895-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="0c895-129">showCategoryName</span></span>|<span data-ttu-id="0c895-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="0c895-130">boolean</span></span>|<span data-ttu-id="0c895-131">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="0c895-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="0c895-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="0c895-132">showLegendKey</span></span>|<span data-ttu-id="0c895-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="0c895-133">boolean</span></span>|<span data-ttu-id="0c895-134">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="0c895-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="0c895-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="0c895-135">showPercentage</span></span>|<span data-ttu-id="0c895-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="0c895-136">boolean</span></span>|<span data-ttu-id="0c895-137">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="0c895-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="0c895-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="0c895-138">showSeriesName</span></span>|<span data-ttu-id="0c895-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="0c895-139">boolean</span></span>|<span data-ttu-id="0c895-140">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="0c895-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="0c895-141">showValue</span><span class="sxs-lookup"><span data-stu-id="0c895-141">showValue</span></span>|<span data-ttu-id="0c895-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="0c895-142">boolean</span></span>|<span data-ttu-id="0c895-143">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="0c895-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c895-144">関係</span><span class="sxs-lookup"><span data-stu-id="0c895-144">Relationships</span></span>
| <span data-ttu-id="0c895-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c895-145">Relationship</span></span> | <span data-ttu-id="0c895-146">型</span><span class="sxs-lookup"><span data-stu-id="0c895-146">Type</span></span>   |<span data-ttu-id="0c895-147">説明</span><span class="sxs-lookup"><span data-stu-id="0c895-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c895-148">format</span><span class="sxs-lookup"><span data-stu-id="0c895-148">format</span></span>|[<span data-ttu-id="0c895-149">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="0c895-149">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="0c895-p102">グラフのデータ ラベルの書式 (塗りつぶしとフォントの書式設定を含む) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0c895-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c895-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c895-152">JSON representation</span></span>

<span data-ttu-id="0c895-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c895-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabels.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
