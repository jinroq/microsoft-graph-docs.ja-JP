---
title: ChartDataLabelFormat リソースの種類
description: グラフのデータ ラベルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a82e88bd8ba083271a821dc86435b0ce55364cec
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572606"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="dc2d2-103">ChartDataLabelFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc2d2-103">ChartDataLabelFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc2d2-104">グラフのデータ ラベルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="dc2d2-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="dc2d2-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc2d2-105">Methods</span></span>
<span data-ttu-id="dc2d2-106">なし</span><span class="sxs-lookup"><span data-stu-id="dc2d2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="dc2d2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc2d2-107">Properties</span></span>
<span data-ttu-id="dc2d2-108">なし</span><span class="sxs-lookup"><span data-stu-id="dc2d2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dc2d2-109">関係</span><span class="sxs-lookup"><span data-stu-id="dc2d2-109">Relationships</span></span>
| <span data-ttu-id="dc2d2-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc2d2-110">Relationship</span></span> | <span data-ttu-id="dc2d2-111">型</span><span class="sxs-lookup"><span data-stu-id="dc2d2-111">Type</span></span>   |<span data-ttu-id="dc2d2-112">説明</span><span class="sxs-lookup"><span data-stu-id="dc2d2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc2d2-113">fill</span><span class="sxs-lookup"><span data-stu-id="dc2d2-113">fill</span></span>|[<span data-ttu-id="dc2d2-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="dc2d2-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="dc2d2-p101">現在のグラフのデータ ラベルの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="dc2d2-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="dc2d2-117">font</span><span class="sxs-lookup"><span data-stu-id="dc2d2-117">font</span></span>|[<span data-ttu-id="dc2d2-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="dc2d2-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="dc2d2-p102">グラフのデータ ラベルのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="dc2d2-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dc2d2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc2d2-121">JSON representation</span></span>

<span data-ttu-id="dc2d2-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dc2d2-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabelformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
