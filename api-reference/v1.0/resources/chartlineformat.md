---
title: ChartLineFormat リソースの種類
description: 直線要素の書式設定オプションをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9da0c29acf49d0e183a2ded4652fe0972f21bf76
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569033"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="a178f-103">ChartLineFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a178f-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="a178f-104">直線要素の書式設定オプションをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="a178f-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="a178f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a178f-105">Methods</span></span>

| <span data-ttu-id="a178f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a178f-106">Method</span></span>           | <span data-ttu-id="a178f-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a178f-107">Return Type</span></span>    |<span data-ttu-id="a178f-108">説明</span><span class="sxs-lookup"><span data-stu-id="a178f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a178f-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a178f-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="a178f-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a178f-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="a178f-111">chartLineFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a178f-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="a178f-112">Update</span><span class="sxs-lookup"><span data-stu-id="a178f-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="a178f-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a178f-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="a178f-114">ChartLineFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a178f-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="a178f-115">Clear</span><span class="sxs-lookup"><span data-stu-id="a178f-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="a178f-116">なし</span><span class="sxs-lookup"><span data-stu-id="a178f-116">None</span></span>|<span data-ttu-id="a178f-117">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="a178f-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="a178f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a178f-118">Properties</span></span>
| <span data-ttu-id="a178f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a178f-119">Property</span></span>     | <span data-ttu-id="a178f-120">型</span><span class="sxs-lookup"><span data-stu-id="a178f-120">Type</span></span>   |<span data-ttu-id="a178f-121">説明</span><span class="sxs-lookup"><span data-stu-id="a178f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a178f-122">color</span><span class="sxs-lookup"><span data-stu-id="a178f-122">color</span></span>|<span data-ttu-id="a178f-123">string</span><span class="sxs-lookup"><span data-stu-id="a178f-123">string</span></span>|<span data-ttu-id="a178f-124">グラフの線の色を表す HTML カラー コード。</span><span class="sxs-lookup"><span data-stu-id="a178f-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a178f-125">関係</span><span class="sxs-lookup"><span data-stu-id="a178f-125">Relationships</span></span>
<span data-ttu-id="a178f-126">なし</span><span class="sxs-lookup"><span data-stu-id="a178f-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a178f-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a178f-127">JSON representation</span></span>

<span data-ttu-id="a178f-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a178f-128">Here is a JSON representation of the resource.</span></span>

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
