---
title: ChartAxis リソースの種類
description: グラフの 1 つの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524724"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="16c15-103">ChartAxis リソースの種類</span><span class="sxs-lookup"><span data-stu-id="16c15-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16c15-104">グラフの 1 つの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="16c15-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="16c15-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="16c15-105">Methods</span></span>

| <span data-ttu-id="16c15-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="16c15-106">Method</span></span>           | <span data-ttu-id="16c15-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="16c15-107">Return Type</span></span>    |<span data-ttu-id="16c15-108">説明</span><span class="sxs-lookup"><span data-stu-id="16c15-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16c15-109">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="16c15-109">[Get ChartAxis](../api/chartaxis-get.md)</span></span> | [<span data-ttu-id="16c15-110">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="16c15-110">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="16c15-111">chartAxis オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="16c15-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="16c15-112">Update</span><span class="sxs-lookup"><span data-stu-id="16c15-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="16c15-113">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="16c15-113">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="16c15-114">ChartAxis オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="16c15-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="16c15-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16c15-115">Properties</span></span>
| <span data-ttu-id="16c15-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16c15-116">Property</span></span>     | <span data-ttu-id="16c15-117">型</span><span class="sxs-lookup"><span data-stu-id="16c15-117">Type</span></span>   |<span data-ttu-id="16c15-118">説明</span><span class="sxs-lookup"><span data-stu-id="16c15-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16c15-119">majorUnit</span><span class="sxs-lookup"><span data-stu-id="16c15-119">majorUnit</span></span>|<span data-ttu-id="16c15-120">object</span><span class="sxs-lookup"><span data-stu-id="16c15-120">object</span></span>|<span data-ttu-id="16c15-p101">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="16c15-p101">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="16c15-124">maximum</span><span class="sxs-lookup"><span data-stu-id="16c15-124">maximum</span></span>|<span data-ttu-id="16c15-125">object</span><span class="sxs-lookup"><span data-stu-id="16c15-125">object</span></span>|<span data-ttu-id="16c15-p102">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="16c15-p102">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="16c15-129">minimum</span><span class="sxs-lookup"><span data-stu-id="16c15-129">minimum</span></span>|<span data-ttu-id="16c15-130">object</span><span class="sxs-lookup"><span data-stu-id="16c15-130">object</span></span>|<span data-ttu-id="16c15-p103">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="16c15-p103">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="16c15-134">minorUnit</span><span class="sxs-lookup"><span data-stu-id="16c15-134">minorUnit</span></span>|<span data-ttu-id="16c15-135">object</span><span class="sxs-lookup"><span data-stu-id="16c15-135">object</span></span>|<span data-ttu-id="16c15-p104">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="16c15-p104">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16c15-139">関係</span><span class="sxs-lookup"><span data-stu-id="16c15-139">Relationships</span></span>
| <span data-ttu-id="16c15-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="16c15-140">Relationship</span></span> | <span data-ttu-id="16c15-141">型</span><span class="sxs-lookup"><span data-stu-id="16c15-141">Type</span></span>   |<span data-ttu-id="16c15-142">説明</span><span class="sxs-lookup"><span data-stu-id="16c15-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16c15-143">format</span><span class="sxs-lookup"><span data-stu-id="16c15-143">format</span></span>|[<span data-ttu-id="16c15-144">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="16c15-144">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="16c15-p105">グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="16c15-p105">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="16c15-147">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="16c15-147">majorGridlines</span></span>|<span data-ttu-id="16c15-148">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="16c15-148">[ChartGridlines](chartgridlines.md)</span></span>|<span data-ttu-id="16c15-p106">指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="16c15-p106">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="16c15-151">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="16c15-151">minorGridlines</span></span>|[<span data-ttu-id="16c15-152">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="16c15-152">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="16c15-p107">指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="16c15-p107">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="16c15-155">title</span><span class="sxs-lookup"><span data-stu-id="16c15-155">title</span></span>|[<span data-ttu-id="16c15-156">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="16c15-156">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="16c15-p108">軸タイトルを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="16c15-p108">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16c15-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16c15-159">JSON representation</span></span>

<span data-ttu-id="16c15-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="16c15-160">Here is a JSON representation of the resource.</span></span>

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
