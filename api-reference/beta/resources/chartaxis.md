---
title: ChartAxis リソースの種類
description: グラフの 1 つの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640932"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="effc4-103">ChartAxis リソースの種類</span><span class="sxs-lookup"><span data-stu-id="effc4-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="effc4-104">グラフの 1 つの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="effc4-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="effc4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="effc4-105">Methods</span></span>

| <span data-ttu-id="effc4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="effc4-106">Method</span></span>           | <span data-ttu-id="effc4-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="effc4-107">Return Type</span></span>    |<span data-ttu-id="effc4-108">説明</span><span class="sxs-lookup"><span data-stu-id="effc4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="effc4-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="effc4-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="effc4-110">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="effc4-110">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="effc4-111">chartAxis オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="effc4-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="effc4-112">更新する</span><span class="sxs-lookup"><span data-stu-id="effc4-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="effc4-113">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="effc4-113">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="effc4-114">ChartAxis オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="effc4-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="effc4-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="effc4-115">Properties</span></span>
| <span data-ttu-id="effc4-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="effc4-116">Property</span></span>     | <span data-ttu-id="effc4-117">型</span><span class="sxs-lookup"><span data-stu-id="effc4-117">Type</span></span>   |<span data-ttu-id="effc4-118">説明</span><span class="sxs-lookup"><span data-stu-id="effc4-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="effc4-119">majorUnit</span><span class="sxs-lookup"><span data-stu-id="effc4-119">majorUnit</span></span>|<span data-ttu-id="effc4-120">object</span><span class="sxs-lookup"><span data-stu-id="effc4-120">object</span></span>|<span data-ttu-id="effc4-p101">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="effc4-p101">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="effc4-124">maximum</span><span class="sxs-lookup"><span data-stu-id="effc4-124">maximum</span></span>|<span data-ttu-id="effc4-125">object</span><span class="sxs-lookup"><span data-stu-id="effc4-125">object</span></span>|<span data-ttu-id="effc4-p102">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="effc4-p102">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="effc4-129">minimum</span><span class="sxs-lookup"><span data-stu-id="effc4-129">minimum</span></span>|<span data-ttu-id="effc4-130">object</span><span class="sxs-lookup"><span data-stu-id="effc4-130">object</span></span>|<span data-ttu-id="effc4-p103">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="effc4-p103">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="effc4-134">minorUnit</span><span class="sxs-lookup"><span data-stu-id="effc4-134">minorUnit</span></span>|<span data-ttu-id="effc4-135">object</span><span class="sxs-lookup"><span data-stu-id="effc4-135">object</span></span>|<span data-ttu-id="effc4-p104">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="effc4-p104">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="effc4-139">関係</span><span class="sxs-lookup"><span data-stu-id="effc4-139">Relationships</span></span>
| <span data-ttu-id="effc4-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="effc4-140">Relationship</span></span> | <span data-ttu-id="effc4-141">型</span><span class="sxs-lookup"><span data-stu-id="effc4-141">Type</span></span>   |<span data-ttu-id="effc4-142">説明</span><span class="sxs-lookup"><span data-stu-id="effc4-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="effc4-143">format</span><span class="sxs-lookup"><span data-stu-id="effc4-143">format</span></span>|[<span data-ttu-id="effc4-144">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="effc4-144">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="effc4-p105">グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="effc4-p105">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="effc4-147">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="effc4-147">majorGridlines</span></span>|[<span data-ttu-id="effc4-148">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="effc4-148">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="effc4-p106">指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="effc4-p106">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="effc4-151">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="effc4-151">minorGridlines</span></span>|[<span data-ttu-id="effc4-152">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="effc4-152">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="effc4-p107">指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="effc4-p107">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="effc4-155">title</span><span class="sxs-lookup"><span data-stu-id="effc4-155">title</span></span>|[<span data-ttu-id="effc4-156">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="effc4-156">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="effc4-p108">軸タイトルを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="effc4-p108">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="effc4-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="effc4-159">JSON representation</span></span>

<span data-ttu-id="effc4-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="effc4-160">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxis.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
