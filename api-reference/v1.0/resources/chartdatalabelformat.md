---
title: ChartDataLabelFormat リソースの種類
description: グラフのデータ ラベルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 645267fd595a4b8e83090d9d6b2179e8c6112a78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569075"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="462b6-103">ChartDataLabelFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="462b6-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="462b6-104">グラフのデータ ラベルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="462b6-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="462b6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="462b6-105">Methods</span></span>
<span data-ttu-id="462b6-106">なし</span><span class="sxs-lookup"><span data-stu-id="462b6-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="462b6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="462b6-107">Properties</span></span>
<span data-ttu-id="462b6-108">なし</span><span class="sxs-lookup"><span data-stu-id="462b6-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="462b6-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="462b6-109">Relationships</span></span>
| <span data-ttu-id="462b6-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="462b6-110">Relationship</span></span> | <span data-ttu-id="462b6-111">型</span><span class="sxs-lookup"><span data-stu-id="462b6-111">Type</span></span>   |<span data-ttu-id="462b6-112">説明</span><span class="sxs-lookup"><span data-stu-id="462b6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="462b6-113">fill</span><span class="sxs-lookup"><span data-stu-id="462b6-113">fill</span></span>|[<span data-ttu-id="462b6-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="462b6-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="462b6-p101">現在のグラフのデータ ラベルの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="462b6-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="462b6-117">font</span><span class="sxs-lookup"><span data-stu-id="462b6-117">font</span></span>|[<span data-ttu-id="462b6-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="462b6-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="462b6-119">グラフのデータ ラベルのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="462b6-119">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="462b6-120">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="462b6-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="462b6-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="462b6-121">JSON representation</span></span>

<span data-ttu-id="462b6-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="462b6-122">Here is a JSON representation of the resource.</span></span>

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
