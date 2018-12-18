---
title: ChartSeriesFormat リソースの種類
description: グラフ系列の書式設定プロパティをカプセル化します。
author: lumine2008
ms.openlocfilehash: 9c27a20c6be6987c31579ca88d546ee80c86d3ea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354062"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="8e33b-103">ChartSeriesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8e33b-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="8e33b-104">グラフ系列の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="8e33b-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="8e33b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8e33b-105">Methods</span></span>
<span data-ttu-id="8e33b-106">なし</span><span class="sxs-lookup"><span data-stu-id="8e33b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="8e33b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e33b-107">Properties</span></span>
<span data-ttu-id="8e33b-108">なし</span><span class="sxs-lookup"><span data-stu-id="8e33b-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8e33b-109">関係</span><span class="sxs-lookup"><span data-stu-id="8e33b-109">Relationships</span></span>
| <span data-ttu-id="8e33b-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8e33b-110">Relationship</span></span> | <span data-ttu-id="8e33b-111">型</span><span class="sxs-lookup"><span data-stu-id="8e33b-111">Type</span></span>   |<span data-ttu-id="8e33b-112">説明</span><span class="sxs-lookup"><span data-stu-id="8e33b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e33b-113">fill</span><span class="sxs-lookup"><span data-stu-id="8e33b-113">fill</span></span>|[<span data-ttu-id="8e33b-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="8e33b-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="8e33b-p101">グラフ系列の塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8e33b-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="8e33b-117">line</span><span class="sxs-lookup"><span data-stu-id="8e33b-117">line</span></span>|[<span data-ttu-id="8e33b-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8e33b-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="8e33b-p102">線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8e33b-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8e33b-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8e33b-121">JSON representation</span></span>

<span data-ttu-id="8e33b-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8e33b-122">Here is a JSON representation of the resource.</span></span>

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