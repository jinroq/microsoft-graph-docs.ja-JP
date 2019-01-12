---
title: ChartAxisFormat リソースの種類
description: グラフ軸の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 92258887c9646890ee63d14aebcd32ada7a8aaa6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952112"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="d1a08-103">ChartAxisFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1a08-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="d1a08-104">グラフ軸の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="d1a08-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="d1a08-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1a08-105">Methods</span></span>
<span data-ttu-id="d1a08-106">なし</span><span class="sxs-lookup"><span data-stu-id="d1a08-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="d1a08-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1a08-107">Properties</span></span>
<span data-ttu-id="d1a08-108">なし</span><span class="sxs-lookup"><span data-stu-id="d1a08-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d1a08-109">関係</span><span class="sxs-lookup"><span data-stu-id="d1a08-109">Relationships</span></span>
| <span data-ttu-id="d1a08-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1a08-110">Relationship</span></span> | <span data-ttu-id="d1a08-111">型</span><span class="sxs-lookup"><span data-stu-id="d1a08-111">Type</span></span>   |<span data-ttu-id="d1a08-112">説明</span><span class="sxs-lookup"><span data-stu-id="d1a08-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1a08-113">font</span><span class="sxs-lookup"><span data-stu-id="d1a08-113">font</span></span>|[<span data-ttu-id="d1a08-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d1a08-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="d1a08-p101">グラフ軸要素のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d1a08-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="d1a08-117">line</span><span class="sxs-lookup"><span data-stu-id="d1a08-117">line</span></span>|[<span data-ttu-id="d1a08-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d1a08-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="d1a08-p102">グラフの線の書式設定を表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d1a08-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d1a08-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1a08-121">JSON representation</span></span>

<span data-ttu-id="d1a08-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1a08-122">Here is a JSON representation of the resource.</span></span>

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
