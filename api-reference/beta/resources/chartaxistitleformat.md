---
title: ChartAxisTitleFormat リソースの種類
description: グラフ軸のタイトルの書式設定を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: aeb39c46b349bda9f71385d13ef8e9ab17320823
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575920"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="e5844-103">ChartAxisTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5844-103">ChartAxisTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5844-104">グラフ軸のタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="e5844-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="e5844-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5844-105">Methods</span></span>
<span data-ttu-id="e5844-106">なし</span><span class="sxs-lookup"><span data-stu-id="e5844-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e5844-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5844-107">Properties</span></span>
<span data-ttu-id="e5844-108">なし</span><span class="sxs-lookup"><span data-stu-id="e5844-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e5844-109">関係</span><span class="sxs-lookup"><span data-stu-id="e5844-109">Relationships</span></span>
| <span data-ttu-id="e5844-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5844-110">Relationship</span></span> | <span data-ttu-id="e5844-111">型</span><span class="sxs-lookup"><span data-stu-id="e5844-111">Type</span></span>   |<span data-ttu-id="e5844-112">説明</span><span class="sxs-lookup"><span data-stu-id="e5844-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5844-113">font</span><span class="sxs-lookup"><span data-stu-id="e5844-113">font</span></span>|[<span data-ttu-id="e5844-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e5844-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e5844-p101">グラフの軸タイトルのオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e5844-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5844-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5844-117">JSON representation</span></span>

<span data-ttu-id="e5844-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5844-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxistitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
