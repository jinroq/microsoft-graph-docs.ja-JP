---
title: workbookChartAxis リソースの種類
description: グラフの 1 つの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 929fd2569067e67af6770b9281bce1d09cd9eca4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007376"
---
# <a name="workbookchartaxis-resource-type"></a><span data-ttu-id="5afd5-103">workbookChartAxis リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5afd5-103">workbookChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5afd5-104">グラフの 1 つの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="5afd5-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="5afd5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5afd5-105">Methods</span></span>

| <span data-ttu-id="5afd5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5afd5-106">Method</span></span>           | <span data-ttu-id="5afd5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5afd5-107">Return Type</span></span>    |<span data-ttu-id="5afd5-108">説明</span><span class="sxs-lookup"><span data-stu-id="5afd5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5afd5-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="5afd5-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="5afd5-110">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5afd5-110">workbookChartAxis</span></span>](workbookchartaxis.md) |<span data-ttu-id="5afd5-111">chartAxis オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5afd5-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="5afd5-112">Update</span><span class="sxs-lookup"><span data-stu-id="5afd5-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="5afd5-113">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5afd5-113">workbookChartAxis</span></span>](workbookchartaxis.md)   |<span data-ttu-id="5afd5-114">ChartAxis オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5afd5-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5afd5-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5afd5-115">Properties</span></span>
| <span data-ttu-id="5afd5-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5afd5-116">Property</span></span>     | <span data-ttu-id="5afd5-117">型</span><span class="sxs-lookup"><span data-stu-id="5afd5-117">Type</span></span>   |<span data-ttu-id="5afd5-118">説明</span><span class="sxs-lookup"><span data-stu-id="5afd5-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5afd5-119">id</span><span class="sxs-lookup"><span data-stu-id="5afd5-119">id</span></span>       |<span data-ttu-id="5afd5-120">string</span><span class="sxs-lookup"><span data-stu-id="5afd5-120">string</span></span>   | <span data-ttu-id="5afd5-121">一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5afd5-121">Unique identifier.</span></span> <span data-ttu-id="5afd5-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-122">Read-only.</span></span>|
|<span data-ttu-id="5afd5-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="5afd5-123">majorUnit</span></span>|<span data-ttu-id="5afd5-124">Json</span><span class="sxs-lookup"><span data-stu-id="5afd5-124">Json</span></span>|<span data-ttu-id="5afd5-p102">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="5afd5-128">maximum</span><span class="sxs-lookup"><span data-stu-id="5afd5-128">maximum</span></span>|<span data-ttu-id="5afd5-129">Json</span><span class="sxs-lookup"><span data-stu-id="5afd5-129">Json</span></span>|<span data-ttu-id="5afd5-p103">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="5afd5-133">minimum</span><span class="sxs-lookup"><span data-stu-id="5afd5-133">minimum</span></span>|<span data-ttu-id="5afd5-134">Json</span><span class="sxs-lookup"><span data-stu-id="5afd5-134">Json</span></span>|<span data-ttu-id="5afd5-p104">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="5afd5-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="5afd5-138">minorUnit</span></span>|<span data-ttu-id="5afd5-139">Json</span><span class="sxs-lookup"><span data-stu-id="5afd5-139">Json</span></span>|<span data-ttu-id="5afd5-p105">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5afd5-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5afd5-143">Relationships</span></span>
| <span data-ttu-id="5afd5-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5afd5-144">Relationship</span></span> | <span data-ttu-id="5afd5-145">型</span><span class="sxs-lookup"><span data-stu-id="5afd5-145">Type</span></span>   |<span data-ttu-id="5afd5-146">説明</span><span class="sxs-lookup"><span data-stu-id="5afd5-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5afd5-147">format</span><span class="sxs-lookup"><span data-stu-id="5afd5-147">format</span></span>|[<span data-ttu-id="5afd5-148">workbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="5afd5-148">workbookChartAxisFormat</span></span>](workbookchartaxisformat.md)|<span data-ttu-id="5afd5-p106">グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="5afd5-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="5afd5-151">majorGridlines</span></span>|[<span data-ttu-id="5afd5-152">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="5afd5-152">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="5afd5-p107">指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="5afd5-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="5afd5-155">minorGridlines</span></span>|[<span data-ttu-id="5afd5-156">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="5afd5-156">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="5afd5-p108">指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="5afd5-159">title</span><span class="sxs-lookup"><span data-stu-id="5afd5-159">title</span></span>|[<span data-ttu-id="5afd5-160">workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="5afd5-160">workbookChartAxisTitle</span></span>](workbookchartaxistitle.md)|<span data-ttu-id="5afd5-161">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="5afd5-161">Represents the axis title.</span></span> <span data-ttu-id="5afd5-162">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-162">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5afd5-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5afd5-163">JSON representation</span></span>

<span data-ttu-id="5afd5-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5afd5-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "title",
    "minorGridlines",
    "majorGridlines",
    "format"
   ],
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
