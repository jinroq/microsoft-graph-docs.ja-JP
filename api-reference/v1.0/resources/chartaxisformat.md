---
title: ChartAxisFormat リソースの種類
description: グラフ軸の書式設定プロパティをカプセル化します。
ms.openlocfilehash: 38679d8f6d70c336f17aa5c17c9a20e80204cfb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024324"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="e0a19-103">ChartAxisFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0a19-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="e0a19-104">グラフ軸の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="e0a19-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="e0a19-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0a19-105">Methods</span></span>
<span data-ttu-id="e0a19-106">なし</span><span class="sxs-lookup"><span data-stu-id="e0a19-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="e0a19-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0a19-107">Properties</span></span>
<span data-ttu-id="e0a19-108">なし</span><span class="sxs-lookup"><span data-stu-id="e0a19-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e0a19-109">関係</span><span class="sxs-lookup"><span data-stu-id="e0a19-109">Relationships</span></span>
| <span data-ttu-id="e0a19-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0a19-110">Relationship</span></span> | <span data-ttu-id="e0a19-111">型</span><span class="sxs-lookup"><span data-stu-id="e0a19-111">Type</span></span>   |<span data-ttu-id="e0a19-112">説明</span><span class="sxs-lookup"><span data-stu-id="e0a19-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a19-113">font</span><span class="sxs-lookup"><span data-stu-id="e0a19-113">font</span></span>|[<span data-ttu-id="e0a19-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e0a19-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e0a19-p101">グラフ軸要素のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e0a19-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="e0a19-117">line</span><span class="sxs-lookup"><span data-stu-id="e0a19-117">line</span></span>|[<span data-ttu-id="e0a19-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e0a19-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="e0a19-p102">グラフの線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e0a19-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e0a19-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0a19-121">JSON representation</span></span>

<span data-ttu-id="e0a19-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0a19-122">Here is a JSON representation of the resource.</span></span>

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