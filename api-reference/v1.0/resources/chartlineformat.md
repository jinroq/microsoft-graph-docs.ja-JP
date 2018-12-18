---
title: ChartLineFormat リソースの種類
description: 直線要素の書式設定オプションをカプセル化します。
author: lumine2008
ms.openlocfilehash: 1940b5dfe09c2895fbf1b8eb6bf4e5227194367c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357303"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="960af-103">ChartLineFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="960af-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="960af-104">直線要素の書式設定オプションをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="960af-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="960af-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="960af-105">Methods</span></span>

| <span data-ttu-id="960af-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="960af-106">Method</span></span>           | <span data-ttu-id="960af-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="960af-107">Return Type</span></span>    |<span data-ttu-id="960af-108">説明</span><span class="sxs-lookup"><span data-stu-id="960af-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="960af-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="960af-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="960af-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="960af-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="960af-111">chartLineFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="960af-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="960af-112">Update</span><span class="sxs-lookup"><span data-stu-id="960af-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="960af-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="960af-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="960af-114">ChartLineFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="960af-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="960af-115">Clear</span><span class="sxs-lookup"><span data-stu-id="960af-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="960af-116">なし</span><span class="sxs-lookup"><span data-stu-id="960af-116">None</span></span>|<span data-ttu-id="960af-117">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="960af-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="960af-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="960af-118">Properties</span></span>
| <span data-ttu-id="960af-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="960af-119">Property</span></span>     | <span data-ttu-id="960af-120">種類</span><span class="sxs-lookup"><span data-stu-id="960af-120">Type</span></span>   |<span data-ttu-id="960af-121">説明</span><span class="sxs-lookup"><span data-stu-id="960af-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="960af-122">color</span><span class="sxs-lookup"><span data-stu-id="960af-122">color</span></span>|<span data-ttu-id="960af-123">文字列</span><span class="sxs-lookup"><span data-stu-id="960af-123">string</span></span>|<span data-ttu-id="960af-124">グラフの線の色を表す HTML カラー コード。</span><span class="sxs-lookup"><span data-stu-id="960af-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="960af-125">関係</span><span class="sxs-lookup"><span data-stu-id="960af-125">Relationships</span></span>
<span data-ttu-id="960af-126">なし</span><span class="sxs-lookup"><span data-stu-id="960af-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="960af-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="960af-127">JSON representation</span></span>

<span data-ttu-id="960af-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="960af-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->