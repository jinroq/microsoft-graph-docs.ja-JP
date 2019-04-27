---
title: workbookChartSeriesFormat リソースの種類
description: グラフ系列の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5d07dbaf17fd715b93dcd039fe3fb9e264bd7f63
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348904"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="3a325-103">workbookChartSeriesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a325-103">workbookChartSeriesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a325-104">グラフ系列の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="3a325-104">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="3a325-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="3a325-105">Methods</span></span>
<span data-ttu-id="3a325-106">なし</span><span class="sxs-lookup"><span data-stu-id="3a325-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="3a325-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a325-107">Properties</span></span>
<span data-ttu-id="3a325-108">なし</span><span class="sxs-lookup"><span data-stu-id="3a325-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3a325-109">関係</span><span class="sxs-lookup"><span data-stu-id="3a325-109">Relationships</span></span>
| <span data-ttu-id="3a325-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a325-110">Relationship</span></span> | <span data-ttu-id="3a325-111">型</span><span class="sxs-lookup"><span data-stu-id="3a325-111">Type</span></span>   |<span data-ttu-id="3a325-112">説明</span><span class="sxs-lookup"><span data-stu-id="3a325-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a325-113">fill</span><span class="sxs-lookup"><span data-stu-id="3a325-113">fill</span></span>|[<span data-ttu-id="3a325-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="3a325-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="3a325-p101">グラフ系列の塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3a325-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="3a325-117">line</span><span class="sxs-lookup"><span data-stu-id="3a325-117">line</span></span>|[<span data-ttu-id="3a325-118">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="3a325-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="3a325-119">線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="3a325-119">Represents line formatting.</span></span> <span data-ttu-id="3a325-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3a325-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3a325-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a325-121">JSON representation</span></span>

<span data-ttu-id="3a325-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a325-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
