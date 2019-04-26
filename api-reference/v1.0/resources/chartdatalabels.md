---
title: ChartDataLabels リソースの種類
description: グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 48d6cb0d35e82fc0117a24aad1c5e171bc869870
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569005"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="704de-103">ChartDataLabels リソースの種類</span><span class="sxs-lookup"><span data-stu-id="704de-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="704de-104">グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="704de-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="704de-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="704de-105">Methods</span></span>

| <span data-ttu-id="704de-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="704de-106">Method</span></span>           | <span data-ttu-id="704de-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="704de-107">Return Type</span></span>    |<span data-ttu-id="704de-108">説明</span><span class="sxs-lookup"><span data-stu-id="704de-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="704de-109">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="704de-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="704de-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="704de-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="704de-111">chartDataLabels オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="704de-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="704de-112">Update</span><span class="sxs-lookup"><span data-stu-id="704de-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="704de-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="704de-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="704de-114">ChartDataLabels オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="704de-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="704de-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="704de-115">Properties</span></span>
| <span data-ttu-id="704de-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="704de-116">Property</span></span>     | <span data-ttu-id="704de-117">型</span><span class="sxs-lookup"><span data-stu-id="704de-117">Type</span></span>   |<span data-ttu-id="704de-118">説明</span><span class="sxs-lookup"><span data-stu-id="704de-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="704de-119">position</span><span class="sxs-lookup"><span data-stu-id="704de-119">position</span></span>|<span data-ttu-id="704de-120">string</span><span class="sxs-lookup"><span data-stu-id="704de-120">string</span></span>|<span data-ttu-id="704de-121">データ ラベルの位置を表す DataLabelPosition 値。</span><span class="sxs-lookup"><span data-stu-id="704de-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="704de-122">使用可能な値は`None`、 `Center`、 `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom`、、、、、、、、、 `Callout` `BestFit`です。</span><span class="sxs-lookup"><span data-stu-id="704de-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="704de-123">separator</span><span class="sxs-lookup"><span data-stu-id="704de-123">separator</span></span>|<span data-ttu-id="704de-124">string</span><span class="sxs-lookup"><span data-stu-id="704de-124">string</span></span>|<span data-ttu-id="704de-125">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="704de-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="704de-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="704de-126">showBubbleSize</span></span>|<span data-ttu-id="704de-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="704de-127">boolean</span></span>|<span data-ttu-id="704de-128">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="704de-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="704de-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="704de-129">showCategoryName</span></span>|<span data-ttu-id="704de-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="704de-130">boolean</span></span>|<span data-ttu-id="704de-131">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="704de-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="704de-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="704de-132">showLegendKey</span></span>|<span data-ttu-id="704de-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="704de-133">boolean</span></span>|<span data-ttu-id="704de-134">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="704de-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="704de-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="704de-135">showPercentage</span></span>|<span data-ttu-id="704de-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="704de-136">boolean</span></span>|<span data-ttu-id="704de-137">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="704de-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="704de-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="704de-138">showSeriesName</span></span>|<span data-ttu-id="704de-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="704de-139">boolean</span></span>|<span data-ttu-id="704de-140">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="704de-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="704de-141">showValue</span><span class="sxs-lookup"><span data-stu-id="704de-141">showValue</span></span>|<span data-ttu-id="704de-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="704de-142">boolean</span></span>|<span data-ttu-id="704de-143">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="704de-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="704de-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="704de-144">Relationships</span></span>
| <span data-ttu-id="704de-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="704de-145">Relationship</span></span> | <span data-ttu-id="704de-146">型</span><span class="sxs-lookup"><span data-stu-id="704de-146">Type</span></span>   |<span data-ttu-id="704de-147">説明</span><span class="sxs-lookup"><span data-stu-id="704de-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="704de-148">format</span><span class="sxs-lookup"><span data-stu-id="704de-148">format</span></span>|[<span data-ttu-id="704de-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="704de-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="704de-150">グラフのデータ ラベルの書式 (塗りつぶしとフォントの書式設定を含む) を表します。</span><span class="sxs-lookup"><span data-stu-id="704de-150">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="704de-151">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="704de-151">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="704de-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="704de-152">JSON representation</span></span>

<span data-ttu-id="704de-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="704de-153">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
