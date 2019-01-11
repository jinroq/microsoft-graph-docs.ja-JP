---
title: ChartAxisFormat リソースの種類
description: グラフ軸の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a219122141da1f384279d0ff4c612f62226612c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821267"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="76dfc-103">ChartAxisFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76dfc-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="76dfc-104">グラフ軸の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="76dfc-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="76dfc-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="76dfc-105">Methods</span></span>
<span data-ttu-id="76dfc-106">なし</span><span class="sxs-lookup"><span data-stu-id="76dfc-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="76dfc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76dfc-107">Properties</span></span>
<span data-ttu-id="76dfc-108">なし</span><span class="sxs-lookup"><span data-stu-id="76dfc-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="76dfc-109">関係</span><span class="sxs-lookup"><span data-stu-id="76dfc-109">Relationships</span></span>
| <span data-ttu-id="76dfc-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="76dfc-110">Relationship</span></span> | <span data-ttu-id="76dfc-111">型</span><span class="sxs-lookup"><span data-stu-id="76dfc-111">Type</span></span>   |<span data-ttu-id="76dfc-112">説明</span><span class="sxs-lookup"><span data-stu-id="76dfc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76dfc-113">font</span><span class="sxs-lookup"><span data-stu-id="76dfc-113">font</span></span>|[<span data-ttu-id="76dfc-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="76dfc-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="76dfc-p101">グラフ軸要素のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="76dfc-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="76dfc-117">line</span><span class="sxs-lookup"><span data-stu-id="76dfc-117">line</span></span>|[<span data-ttu-id="76dfc-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="76dfc-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="76dfc-p102">グラフの線の書式設定を表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="76dfc-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="76dfc-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76dfc-121">JSON representation</span></span>

<span data-ttu-id="76dfc-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76dfc-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
