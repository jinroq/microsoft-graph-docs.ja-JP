---
title: workbookChartDataLabelFormat リソースの種類
description: グラフのデータ ラベルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd60187d5bc62675b53b4a0a254afa3632e9c1d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964003"
---
# <a name="workbookchartdatalabelformat-resource-type"></a><span data-ttu-id="e8ec4-103">workbookChartDataLabelFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8ec4-103">workbookChartDataLabelFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8ec4-104">グラフのデータ ラベルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="e8ec4-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="e8ec4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8ec4-105">Methods</span></span>
<span data-ttu-id="e8ec4-106">None</span><span class="sxs-lookup"><span data-stu-id="e8ec4-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e8ec4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8ec4-107">Properties</span></span>
<span data-ttu-id="e8ec4-108">なし</span><span class="sxs-lookup"><span data-stu-id="e8ec4-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e8ec4-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8ec4-109">Relationships</span></span>
| <span data-ttu-id="e8ec4-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8ec4-110">Relationship</span></span> | <span data-ttu-id="e8ec4-111">型</span><span class="sxs-lookup"><span data-stu-id="e8ec4-111">Type</span></span>   |<span data-ttu-id="e8ec4-112">説明</span><span class="sxs-lookup"><span data-stu-id="e8ec4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8ec4-113">fill</span><span class="sxs-lookup"><span data-stu-id="e8ec4-113">fill</span></span>|[<span data-ttu-id="e8ec4-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="e8ec4-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="e8ec4-p101">現在のグラフのデータ ラベルの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e8ec4-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="e8ec4-117">font</span><span class="sxs-lookup"><span data-stu-id="e8ec4-117">font</span></span>|[<span data-ttu-id="e8ec4-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e8ec4-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="e8ec4-119">グラフのデータ ラベルのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="e8ec4-119">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="e8ec4-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e8ec4-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e8ec4-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8ec4-121">JSON representation</span></span>

<span data-ttu-id="e8ec4-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8ec4-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
  "suppressions": []
}
-->
