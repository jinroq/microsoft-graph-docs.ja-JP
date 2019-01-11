---
title: ChartAxis リソースの種類
description: グラフの 1 つの軸を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 077afe6a384b77c9b4bb3b1bab6a0e257a9175a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842722"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="b6911-103">ChartAxis リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b6911-103">ChartAxis resource type</span></span>

> <span data-ttu-id="b6911-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b6911-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6911-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6911-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6911-106">グラフの 1 つの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="b6911-106">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="b6911-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b6911-107">Methods</span></span>

| <span data-ttu-id="b6911-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b6911-108">Method</span></span>           | <span data-ttu-id="b6911-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b6911-109">Return Type</span></span>    |<span data-ttu-id="b6911-110">説明</span><span class="sxs-lookup"><span data-stu-id="b6911-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6911-111">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="b6911-111">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="b6911-112">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="b6911-112">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="b6911-113">chartAxis オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b6911-113">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="b6911-114">Update</span><span class="sxs-lookup"><span data-stu-id="b6911-114">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="b6911-115">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="b6911-115">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="b6911-116">ChartAxis オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b6911-116">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6911-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6911-117">Properties</span></span>
| <span data-ttu-id="b6911-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6911-118">Property</span></span>     | <span data-ttu-id="b6911-119">種類</span><span class="sxs-lookup"><span data-stu-id="b6911-119">Type</span></span>   |<span data-ttu-id="b6911-120">説明</span><span class="sxs-lookup"><span data-stu-id="b6911-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6911-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="b6911-121">majorUnit</span></span>|<span data-ttu-id="b6911-122">object</span><span class="sxs-lookup"><span data-stu-id="b6911-122">object</span></span>|<span data-ttu-id="b6911-p102">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="b6911-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="b6911-126">maximum</span><span class="sxs-lookup"><span data-stu-id="b6911-126">maximum</span></span>|<span data-ttu-id="b6911-127">object</span><span class="sxs-lookup"><span data-stu-id="b6911-127">object</span></span>|<span data-ttu-id="b6911-p103">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="b6911-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="b6911-131">minimum</span><span class="sxs-lookup"><span data-stu-id="b6911-131">minimum</span></span>|<span data-ttu-id="b6911-132">object</span><span class="sxs-lookup"><span data-stu-id="b6911-132">object</span></span>|<span data-ttu-id="b6911-p104">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="b6911-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="b6911-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="b6911-136">minorUnit</span></span>|<span data-ttu-id="b6911-137">object</span><span class="sxs-lookup"><span data-stu-id="b6911-137">object</span></span>|<span data-ttu-id="b6911-p105">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="b6911-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6911-141">関係</span><span class="sxs-lookup"><span data-stu-id="b6911-141">Relationships</span></span>
| <span data-ttu-id="b6911-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b6911-142">Relationship</span></span> | <span data-ttu-id="b6911-143">型</span><span class="sxs-lookup"><span data-stu-id="b6911-143">Type</span></span>   |<span data-ttu-id="b6911-144">説明</span><span class="sxs-lookup"><span data-stu-id="b6911-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6911-145">format</span><span class="sxs-lookup"><span data-stu-id="b6911-145">format</span></span>|[<span data-ttu-id="b6911-146">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="b6911-146">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="b6911-p106">グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b6911-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="b6911-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="b6911-149">majorGridlines</span></span>|[<span data-ttu-id="b6911-150">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="b6911-150">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="b6911-p107">指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b6911-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="b6911-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="b6911-153">minorGridlines</span></span>|[<span data-ttu-id="b6911-154">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="b6911-154">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="b6911-p108">指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b6911-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="b6911-157">title</span><span class="sxs-lookup"><span data-stu-id="b6911-157">title</span></span>|[<span data-ttu-id="b6911-158">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="b6911-158">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="b6911-p109">軸タイトルを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="b6911-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6911-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b6911-161">JSON representation</span></span>

<span data-ttu-id="b6911-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b6911-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
