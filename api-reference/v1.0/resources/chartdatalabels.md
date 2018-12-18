---
title: ChartDataLabels リソースの種類
description: グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。
author: lumine2008
ms.openlocfilehash: 39c95d0849d398df7d57f676cc392c157e6f43f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339054"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="12e6c-103">ChartDataLabels リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12e6c-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="12e6c-104">グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="12e6c-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="12e6c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="12e6c-105">Methods</span></span>

| <span data-ttu-id="12e6c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="12e6c-106">Method</span></span>           | <span data-ttu-id="12e6c-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="12e6c-107">Return Type</span></span>    |<span data-ttu-id="12e6c-108">説明</span><span class="sxs-lookup"><span data-stu-id="12e6c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12e6c-109">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="12e6c-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="12e6c-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="12e6c-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="12e6c-111">chartDataLabels オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="12e6c-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="12e6c-112">Update</span><span class="sxs-lookup"><span data-stu-id="12e6c-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="12e6c-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="12e6c-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="12e6c-114">ChartDataLabels オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="12e6c-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="12e6c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12e6c-115">Properties</span></span>
| <span data-ttu-id="12e6c-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12e6c-116">Property</span></span>     | <span data-ttu-id="12e6c-117">種類</span><span class="sxs-lookup"><span data-stu-id="12e6c-117">Type</span></span>   |<span data-ttu-id="12e6c-118">説明</span><span class="sxs-lookup"><span data-stu-id="12e6c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12e6c-119">position</span><span class="sxs-lookup"><span data-stu-id="12e6c-119">position</span></span>|<span data-ttu-id="12e6c-120">文字列</span><span class="sxs-lookup"><span data-stu-id="12e6c-120">string</span></span>|<span data-ttu-id="12e6c-121">データ ラベルの位置を表す値を DataLabelPosition。</span><span class="sxs-lookup"><span data-stu-id="12e6c-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="12e6c-122">可能な値: `None`、 `Center`、 `InsideEnd`、 `InsideBase`、 `OutsideEnd`、 `Left`、 `Right`、 `Top`、 `Bottom`、 `BestFit`、 `Callout`。</span><span class="sxs-lookup"><span data-stu-id="12e6c-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="12e6c-123">separator</span><span class="sxs-lookup"><span data-stu-id="12e6c-123">separator</span></span>|<span data-ttu-id="12e6c-124">文字列</span><span class="sxs-lookup"><span data-stu-id="12e6c-124">string</span></span>|<span data-ttu-id="12e6c-125">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="12e6c-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="12e6c-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="12e6c-126">showBubbleSize</span></span>|<span data-ttu-id="12e6c-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="12e6c-127">boolean</span></span>|<span data-ttu-id="12e6c-128">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="12e6c-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="12e6c-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="12e6c-129">showCategoryName</span></span>|<span data-ttu-id="12e6c-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="12e6c-130">boolean</span></span>|<span data-ttu-id="12e6c-131">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="12e6c-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="12e6c-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="12e6c-132">showLegendKey</span></span>|<span data-ttu-id="12e6c-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="12e6c-133">boolean</span></span>|<span data-ttu-id="12e6c-134">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="12e6c-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="12e6c-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="12e6c-135">showPercentage</span></span>|<span data-ttu-id="12e6c-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="12e6c-136">boolean</span></span>|<span data-ttu-id="12e6c-137">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="12e6c-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="12e6c-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="12e6c-138">showSeriesName</span></span>|<span data-ttu-id="12e6c-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="12e6c-139">boolean</span></span>|<span data-ttu-id="12e6c-140">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="12e6c-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="12e6c-141">showValue</span><span class="sxs-lookup"><span data-stu-id="12e6c-141">showValue</span></span>|<span data-ttu-id="12e6c-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="12e6c-142">boolean</span></span>|<span data-ttu-id="12e6c-143">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="12e6c-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12e6c-144">関係</span><span class="sxs-lookup"><span data-stu-id="12e6c-144">Relationships</span></span>
| <span data-ttu-id="12e6c-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="12e6c-145">Relationship</span></span> | <span data-ttu-id="12e6c-146">型</span><span class="sxs-lookup"><span data-stu-id="12e6c-146">Type</span></span>   |<span data-ttu-id="12e6c-147">説明</span><span class="sxs-lookup"><span data-stu-id="12e6c-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12e6c-148">format</span><span class="sxs-lookup"><span data-stu-id="12e6c-148">format</span></span>|[<span data-ttu-id="12e6c-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="12e6c-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="12e6c-p102">グラフのデータ ラベルの書式 (塗りつぶしとフォントの書式設定を含む) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="12e6c-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12e6c-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12e6c-152">JSON representation</span></span>

<span data-ttu-id="12e6c-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="12e6c-153">Here is a JSON representation of the resource.</span></span>

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