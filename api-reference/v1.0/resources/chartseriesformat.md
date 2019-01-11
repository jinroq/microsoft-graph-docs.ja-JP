---
title: ChartSeriesFormat リソースの種類
description: グラフ系列の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f8a4e5fab61da3dba1c02488ff6e3a8bfd0e8fa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815856"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="08a5e-103">ChartSeriesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08a5e-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="08a5e-104">グラフ系列の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="08a5e-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="08a5e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="08a5e-105">Methods</span></span>
<span data-ttu-id="08a5e-106">なし</span><span class="sxs-lookup"><span data-stu-id="08a5e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="08a5e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08a5e-107">Properties</span></span>
<span data-ttu-id="08a5e-108">なし</span><span class="sxs-lookup"><span data-stu-id="08a5e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="08a5e-109">関係</span><span class="sxs-lookup"><span data-stu-id="08a5e-109">Relationships</span></span>
| <span data-ttu-id="08a5e-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="08a5e-110">Relationship</span></span> | <span data-ttu-id="08a5e-111">型</span><span class="sxs-lookup"><span data-stu-id="08a5e-111">Type</span></span>   |<span data-ttu-id="08a5e-112">説明</span><span class="sxs-lookup"><span data-stu-id="08a5e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08a5e-113">fill</span><span class="sxs-lookup"><span data-stu-id="08a5e-113">fill</span></span>|[<span data-ttu-id="08a5e-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="08a5e-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="08a5e-p101">グラフ系列の塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="08a5e-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="08a5e-117">line</span><span class="sxs-lookup"><span data-stu-id="08a5e-117">line</span></span>|[<span data-ttu-id="08a5e-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="08a5e-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="08a5e-p102">線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="08a5e-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="08a5e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08a5e-121">JSON representation</span></span>

<span data-ttu-id="08a5e-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="08a5e-122">Here is a JSON representation of the resource.</span></span>

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
