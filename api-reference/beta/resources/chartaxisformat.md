---
title: ChartAxisFormat リソースの種類
description: グラフ軸の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 587c35f0bf28d695f67e61a8eefa1593317a8d5d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577110"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="692e4-103">ChartAxisFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="692e4-103">ChartAxisFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="692e4-104">グラフ軸の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="692e4-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="692e4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="692e4-105">Methods</span></span>
<span data-ttu-id="692e4-106">なし</span><span class="sxs-lookup"><span data-stu-id="692e4-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="692e4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="692e4-107">Properties</span></span>
<span data-ttu-id="692e4-108">なし</span><span class="sxs-lookup"><span data-stu-id="692e4-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="692e4-109">関係</span><span class="sxs-lookup"><span data-stu-id="692e4-109">Relationships</span></span>
| <span data-ttu-id="692e4-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="692e4-110">Relationship</span></span> | <span data-ttu-id="692e4-111">型</span><span class="sxs-lookup"><span data-stu-id="692e4-111">Type</span></span>   |<span data-ttu-id="692e4-112">説明</span><span class="sxs-lookup"><span data-stu-id="692e4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="692e4-113">font</span><span class="sxs-lookup"><span data-stu-id="692e4-113">font</span></span>|[<span data-ttu-id="692e4-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="692e4-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="692e4-p101">グラフ軸要素のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="692e4-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="692e4-117">line</span><span class="sxs-lookup"><span data-stu-id="692e4-117">line</span></span>|[<span data-ttu-id="692e4-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="692e4-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="692e4-p102">グラフの線の書式設定を表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="692e4-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="692e4-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="692e4-121">JSON representation</span></span>

<span data-ttu-id="692e4-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="692e4-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxisformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
