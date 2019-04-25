---
title: ChartAxis リソースの種類
description: グラフの 1 つの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 88066c356306a619ee620a13eefb6592d7b5f100
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569243"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="0f3bc-103">ChartAxis リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f3bc-103">ChartAxis resource type</span></span>

<span data-ttu-id="0f3bc-104">グラフの 1 つの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="0f3bc-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f3bc-105">Methods</span></span>

| <span data-ttu-id="0f3bc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f3bc-106">Method</span></span>           | <span data-ttu-id="0f3bc-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0f3bc-107">Return Type</span></span>    |<span data-ttu-id="0f3bc-108">説明</span><span class="sxs-lookup"><span data-stu-id="0f3bc-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f3bc-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="0f3bc-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="0f3bc-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="0f3bc-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="0f3bc-111">chartAxis オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="0f3bc-112">Update</span><span class="sxs-lookup"><span data-stu-id="0f3bc-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="0f3bc-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="0f3bc-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="0f3bc-114">ChartAxis オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0f3bc-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f3bc-115">Properties</span></span>
| <span data-ttu-id="0f3bc-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f3bc-116">Property</span></span>     | <span data-ttu-id="0f3bc-117">型</span><span class="sxs-lookup"><span data-stu-id="0f3bc-117">Type</span></span>   |<span data-ttu-id="0f3bc-118">説明</span><span class="sxs-lookup"><span data-stu-id="0f3bc-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0f3bc-119">id</span><span class="sxs-lookup"><span data-stu-id="0f3bc-119">id</span></span>       |<span data-ttu-id="0f3bc-120">string</span><span class="sxs-lookup"><span data-stu-id="0f3bc-120">string</span></span>   | <span data-ttu-id="0f3bc-121">一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-121">Unique identifier.</span></span> <span data-ttu-id="0f3bc-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-122">Read-only.</span></span>|
|<span data-ttu-id="0f3bc-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="0f3bc-123">majorUnit</span></span>|<span data-ttu-id="0f3bc-124">Json</span><span class="sxs-lookup"><span data-stu-id="0f3bc-124">Json</span></span>|<span data-ttu-id="0f3bc-p102">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="0f3bc-128">maximum</span><span class="sxs-lookup"><span data-stu-id="0f3bc-128">maximum</span></span>|<span data-ttu-id="0f3bc-129">Json</span><span class="sxs-lookup"><span data-stu-id="0f3bc-129">Json</span></span>|<span data-ttu-id="0f3bc-p103">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="0f3bc-133">minimum</span><span class="sxs-lookup"><span data-stu-id="0f3bc-133">minimum</span></span>|<span data-ttu-id="0f3bc-134">Json</span><span class="sxs-lookup"><span data-stu-id="0f3bc-134">Json</span></span>|<span data-ttu-id="0f3bc-p104">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="0f3bc-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="0f3bc-138">minorUnit</span></span>|<span data-ttu-id="0f3bc-139">Json</span><span class="sxs-lookup"><span data-stu-id="0f3bc-139">Json</span></span>|<span data-ttu-id="0f3bc-p105">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f3bc-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f3bc-143">Relationships</span></span>
| <span data-ttu-id="0f3bc-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f3bc-144">Relationship</span></span> | <span data-ttu-id="0f3bc-145">型</span><span class="sxs-lookup"><span data-stu-id="0f3bc-145">Type</span></span>   |<span data-ttu-id="0f3bc-146">説明</span><span class="sxs-lookup"><span data-stu-id="0f3bc-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f3bc-147">format</span><span class="sxs-lookup"><span data-stu-id="0f3bc-147">format</span></span>|[<span data-ttu-id="0f3bc-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="0f3bc-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="0f3bc-p106">グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="0f3bc-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="0f3bc-151">majorGridlines</span></span>|[<span data-ttu-id="0f3bc-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="0f3bc-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="0f3bc-p107">指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="0f3bc-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="0f3bc-155">minorGridlines</span></span>|[<span data-ttu-id="0f3bc-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="0f3bc-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="0f3bc-p108">指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="0f3bc-159">title</span><span class="sxs-lookup"><span data-stu-id="0f3bc-159">title</span></span>|[<span data-ttu-id="0f3bc-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="0f3bc-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="0f3bc-161">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-161">Represents the axis title.</span></span> <span data-ttu-id="0f3bc-162">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-162">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f3bc-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f3bc-163">JSON representation</span></span>

<span data-ttu-id="0f3bc-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f3bc-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
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
