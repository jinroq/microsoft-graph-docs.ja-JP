---
title: ChartAxisFormat リソースの種類
description: グラフ軸の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1d52063e63e179540bcbd5c3b4ec0cd09fb620d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029856"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="eb14f-103">ChartAxisFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb14f-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="eb14f-104">グラフ軸の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="eb14f-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="eb14f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="eb14f-105">Methods</span></span>
<span data-ttu-id="eb14f-106">None</span><span class="sxs-lookup"><span data-stu-id="eb14f-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="eb14f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb14f-107">Properties</span></span>
<span data-ttu-id="eb14f-108">なし</span><span class="sxs-lookup"><span data-stu-id="eb14f-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="eb14f-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eb14f-109">Relationships</span></span>
| <span data-ttu-id="eb14f-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eb14f-110">Relationship</span></span> | <span data-ttu-id="eb14f-111">型</span><span class="sxs-lookup"><span data-stu-id="eb14f-111">Type</span></span>   |<span data-ttu-id="eb14f-112">説明</span><span class="sxs-lookup"><span data-stu-id="eb14f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb14f-113">font</span><span class="sxs-lookup"><span data-stu-id="eb14f-113">font</span></span>|[<span data-ttu-id="eb14f-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="eb14f-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="eb14f-p101">グラフ軸要素のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="eb14f-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="eb14f-117">line</span><span class="sxs-lookup"><span data-stu-id="eb14f-117">line</span></span>|[<span data-ttu-id="eb14f-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="eb14f-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="eb14f-119">グラフの線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="eb14f-119">Represents chart line formatting.</span></span> <span data-ttu-id="eb14f-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb14f-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eb14f-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb14f-121">JSON representation</span></span>

<span data-ttu-id="eb14f-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb14f-122">Here is a JSON representation of the resource.</span></span>

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
