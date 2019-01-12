---
title: ChartDataLabels リソースの種類
description: グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 16e2e3acafc98a4066b8620f41f15c7cae1667cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954681"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="5848a-103">ChartDataLabels リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5848a-103">ChartDataLabels resource type</span></span>

> <span data-ttu-id="5848a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5848a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5848a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5848a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5848a-106">グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5848a-106">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="5848a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5848a-107">Methods</span></span>

| <span data-ttu-id="5848a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5848a-108">Method</span></span>           | <span data-ttu-id="5848a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5848a-109">Return Type</span></span>    |<span data-ttu-id="5848a-110">説明</span><span class="sxs-lookup"><span data-stu-id="5848a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5848a-111">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5848a-111">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="5848a-112">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5848a-112">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5848a-113">chartDataLabels オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5848a-113">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="5848a-114">Update</span><span class="sxs-lookup"><span data-stu-id="5848a-114">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="5848a-115">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5848a-115">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5848a-116">ChartDataLabels オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5848a-116">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5848a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5848a-117">Properties</span></span>
| <span data-ttu-id="5848a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5848a-118">Property</span></span>     | <span data-ttu-id="5848a-119">種類</span><span class="sxs-lookup"><span data-stu-id="5848a-119">Type</span></span>   |<span data-ttu-id="5848a-120">説明</span><span class="sxs-lookup"><span data-stu-id="5848a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5848a-121">position</span><span class="sxs-lookup"><span data-stu-id="5848a-121">position</span></span>|<span data-ttu-id="5848a-122">文字列</span><span class="sxs-lookup"><span data-stu-id="5848a-122">string</span></span>|<span data-ttu-id="5848a-p102">データ ラベルの位置を表す DataLabelPosition 値。可能な値は、`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout` です。</span><span class="sxs-lookup"><span data-stu-id="5848a-p102">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="5848a-125">separator</span><span class="sxs-lookup"><span data-stu-id="5848a-125">separator</span></span>|<span data-ttu-id="5848a-126">文字列</span><span class="sxs-lookup"><span data-stu-id="5848a-126">string</span></span>|<span data-ttu-id="5848a-127">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="5848a-127">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="5848a-128">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="5848a-128">showBubbleSize</span></span>|<span data-ttu-id="5848a-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="5848a-129">boolean</span></span>|<span data-ttu-id="5848a-130">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="5848a-130">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="5848a-131">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="5848a-131">showCategoryName</span></span>|<span data-ttu-id="5848a-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="5848a-132">boolean</span></span>|<span data-ttu-id="5848a-133">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="5848a-133">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="5848a-134">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="5848a-134">showLegendKey</span></span>|<span data-ttu-id="5848a-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="5848a-135">boolean</span></span>|<span data-ttu-id="5848a-136">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="5848a-136">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="5848a-137">showPercentage</span><span class="sxs-lookup"><span data-stu-id="5848a-137">showPercentage</span></span>|<span data-ttu-id="5848a-138">ブール値</span><span class="sxs-lookup"><span data-stu-id="5848a-138">boolean</span></span>|<span data-ttu-id="5848a-139">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="5848a-139">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="5848a-140">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="5848a-140">showSeriesName</span></span>|<span data-ttu-id="5848a-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="5848a-141">boolean</span></span>|<span data-ttu-id="5848a-142">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="5848a-142">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="5848a-143">showValue</span><span class="sxs-lookup"><span data-stu-id="5848a-143">showValue</span></span>|<span data-ttu-id="5848a-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="5848a-144">boolean</span></span>|<span data-ttu-id="5848a-145">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="5848a-145">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5848a-146">関係</span><span class="sxs-lookup"><span data-stu-id="5848a-146">Relationships</span></span>
| <span data-ttu-id="5848a-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5848a-147">Relationship</span></span> | <span data-ttu-id="5848a-148">型</span><span class="sxs-lookup"><span data-stu-id="5848a-148">Type</span></span>   |<span data-ttu-id="5848a-149">説明</span><span class="sxs-lookup"><span data-stu-id="5848a-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5848a-150">format</span><span class="sxs-lookup"><span data-stu-id="5848a-150">format</span></span>|[<span data-ttu-id="5848a-151">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="5848a-151">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="5848a-p103">グラフのデータ ラベルの書式 (塗りつぶしとフォントの書式設定を含む) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5848a-p103">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5848a-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5848a-154">JSON representation</span></span>

<span data-ttu-id="5848a-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5848a-155">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
