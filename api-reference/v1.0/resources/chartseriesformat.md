---
title: ChartSeriesFormat リソースの種類
description: グラフ系列の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ce9a777936b25ed77b130dc2b2219eba0f72c183
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029751"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="0e728-103">ChartSeriesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e728-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="0e728-104">グラフ系列の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="0e728-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="0e728-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e728-105">Methods</span></span>
<span data-ttu-id="0e728-106">None</span><span class="sxs-lookup"><span data-stu-id="0e728-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0e728-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e728-107">Properties</span></span>
<span data-ttu-id="0e728-108">なし</span><span class="sxs-lookup"><span data-stu-id="0e728-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0e728-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e728-109">Relationships</span></span>
| <span data-ttu-id="0e728-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e728-110">Relationship</span></span> | <span data-ttu-id="0e728-111">型</span><span class="sxs-lookup"><span data-stu-id="0e728-111">Type</span></span>   |<span data-ttu-id="0e728-112">説明</span><span class="sxs-lookup"><span data-stu-id="0e728-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e728-113">fill</span><span class="sxs-lookup"><span data-stu-id="0e728-113">fill</span></span>|[<span data-ttu-id="0e728-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="0e728-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="0e728-p101">グラフ系列の塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0e728-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="0e728-117">line</span><span class="sxs-lookup"><span data-stu-id="0e728-117">line</span></span>|[<span data-ttu-id="0e728-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="0e728-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="0e728-119">線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="0e728-119">Represents line formatting.</span></span> <span data-ttu-id="0e728-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e728-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0e728-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e728-121">JSON representation</span></span>

<span data-ttu-id="0e728-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e728-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
