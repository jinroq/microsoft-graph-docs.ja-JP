---
title: ChartLegend リソースの種類
description: グラフに凡例を表します。
author: lumine2008
ms.openlocfilehash: 67a55f0286bcf57157cd9912bb03ba0bd6506517
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326405"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="35c6b-103">ChartLegend リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35c6b-103">ChartLegend resource type</span></span>

> <span data-ttu-id="35c6b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35c6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35c6b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35c6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35c6b-106">グラフに凡例を表します。</span><span class="sxs-lookup"><span data-stu-id="35c6b-106">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="35c6b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="35c6b-107">Methods</span></span>

| <span data-ttu-id="35c6b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="35c6b-108">Method</span></span>           | <span data-ttu-id="35c6b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="35c6b-109">Return Type</span></span>    |<span data-ttu-id="35c6b-110">説明</span><span class="sxs-lookup"><span data-stu-id="35c6b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35c6b-111">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="35c6b-111">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="35c6b-112">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="35c6b-112">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="35c6b-113">chartLegend オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="35c6b-113">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="35c6b-114">Update</span><span class="sxs-lookup"><span data-stu-id="35c6b-114">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="35c6b-115">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="35c6b-115">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="35c6b-116">ChartLegend オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="35c6b-116">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="35c6b-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35c6b-117">Properties</span></span>
| <span data-ttu-id="35c6b-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35c6b-118">Property</span></span>     | <span data-ttu-id="35c6b-119">種類</span><span class="sxs-lookup"><span data-stu-id="35c6b-119">Type</span></span>   |<span data-ttu-id="35c6b-120">説明</span><span class="sxs-lookup"><span data-stu-id="35c6b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35c6b-121">overlay</span><span class="sxs-lookup"><span data-stu-id="35c6b-121">overlay</span></span>|<span data-ttu-id="35c6b-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="35c6b-122">boolean</span></span>|<span data-ttu-id="35c6b-123">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="35c6b-123">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="35c6b-124">position</span><span class="sxs-lookup"><span data-stu-id="35c6b-124">position</span></span>|<span data-ttu-id="35c6b-125">文字列</span><span class="sxs-lookup"><span data-stu-id="35c6b-125">string</span></span>|<span data-ttu-id="35c6b-p102">グラフの凡例の位置を表します。可能な値は、`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom` です。</span><span class="sxs-lookup"><span data-stu-id="35c6b-p102">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="35c6b-128">visible</span><span class="sxs-lookup"><span data-stu-id="35c6b-128">visible</span></span>|<span data-ttu-id="35c6b-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="35c6b-129">boolean</span></span>|<span data-ttu-id="35c6b-130">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="35c6b-130">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35c6b-131">関係</span><span class="sxs-lookup"><span data-stu-id="35c6b-131">Relationships</span></span>
| <span data-ttu-id="35c6b-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35c6b-132">Relationship</span></span> | <span data-ttu-id="35c6b-133">型</span><span class="sxs-lookup"><span data-stu-id="35c6b-133">Type</span></span>   |<span data-ttu-id="35c6b-134">説明</span><span class="sxs-lookup"><span data-stu-id="35c6b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35c6b-135">format</span><span class="sxs-lookup"><span data-stu-id="35c6b-135">format</span></span>|[<span data-ttu-id="35c6b-136">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="35c6b-136">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="35c6b-p103">グラフ の凡例の書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="35c6b-p103">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35c6b-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35c6b-139">JSON representation</span></span>

<span data-ttu-id="35c6b-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35c6b-140">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->