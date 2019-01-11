---
title: ChartDataLabelFormat リソースの種類
description: グラフのデータ ラベルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 586b201b0bcc70765fb68aa7736664f493f5539b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876924"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="66efd-103">ChartDataLabelFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66efd-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="66efd-104">グラフのデータ ラベルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="66efd-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="66efd-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="66efd-105">Methods</span></span>
<span data-ttu-id="66efd-106">なし</span><span class="sxs-lookup"><span data-stu-id="66efd-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="66efd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66efd-107">Properties</span></span>
<span data-ttu-id="66efd-108">なし</span><span class="sxs-lookup"><span data-stu-id="66efd-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="66efd-109">関係</span><span class="sxs-lookup"><span data-stu-id="66efd-109">Relationships</span></span>
| <span data-ttu-id="66efd-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66efd-110">Relationship</span></span> | <span data-ttu-id="66efd-111">型</span><span class="sxs-lookup"><span data-stu-id="66efd-111">Type</span></span>   |<span data-ttu-id="66efd-112">説明</span><span class="sxs-lookup"><span data-stu-id="66efd-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66efd-113">fill</span><span class="sxs-lookup"><span data-stu-id="66efd-113">fill</span></span>|[<span data-ttu-id="66efd-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="66efd-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="66efd-p101">現在のグラフのデータ ラベルの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="66efd-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="66efd-117">font</span><span class="sxs-lookup"><span data-stu-id="66efd-117">font</span></span>|[<span data-ttu-id="66efd-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="66efd-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="66efd-p102">グラフのデータ ラベルのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="66efd-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="66efd-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66efd-121">JSON representation</span></span>

<span data-ttu-id="66efd-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66efd-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
