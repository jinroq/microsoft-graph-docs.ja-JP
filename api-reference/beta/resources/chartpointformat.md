---
title: ChartPointFormat リソースの種類
description: グラフのポイントの書式設定オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3004577a5ca9687b4bef85f59cfcc8eb528c4a66
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573306"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="a4d20-103">ChartPointFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4d20-103">ChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4d20-104">グラフのポイントの書式設定オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="a4d20-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="a4d20-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4d20-105">Methods</span></span>
<span data-ttu-id="a4d20-106">なし</span><span class="sxs-lookup"><span data-stu-id="a4d20-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="a4d20-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4d20-107">Properties</span></span>
<span data-ttu-id="a4d20-108">なし</span><span class="sxs-lookup"><span data-stu-id="a4d20-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a4d20-109">関係</span><span class="sxs-lookup"><span data-stu-id="a4d20-109">Relationships</span></span>
| <span data-ttu-id="a4d20-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4d20-110">Relationship</span></span> | <span data-ttu-id="a4d20-111">型</span><span class="sxs-lookup"><span data-stu-id="a4d20-111">Type</span></span>   |<span data-ttu-id="a4d20-112">説明</span><span class="sxs-lookup"><span data-stu-id="a4d20-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4d20-113">fill</span><span class="sxs-lookup"><span data-stu-id="a4d20-113">fill</span></span>|[<span data-ttu-id="a4d20-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="a4d20-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="a4d20-p101">グラフの塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a4d20-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a4d20-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4d20-117">JSON representation</span></span>

<span data-ttu-id="a4d20-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4d20-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpointformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
