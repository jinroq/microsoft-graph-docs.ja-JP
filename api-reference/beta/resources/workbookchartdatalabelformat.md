---
title: workbookChartDataLabelFormat リソースの種類
description: グラフのデータ ラベルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a4bf03bb2c40ce0dc78c24d76e859d040526cf17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348410"
---
# <a name="workbookchartdatalabelformat-resource-type"></a><span data-ttu-id="0cd8e-103">workbookChartDataLabelFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cd8e-103">workbookChartDataLabelFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cd8e-104">グラフのデータ ラベルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="0cd8e-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="0cd8e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cd8e-105">Methods</span></span>
<span data-ttu-id="0cd8e-106">なし</span><span class="sxs-lookup"><span data-stu-id="0cd8e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0cd8e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cd8e-107">Properties</span></span>
<span data-ttu-id="0cd8e-108">なし</span><span class="sxs-lookup"><span data-stu-id="0cd8e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0cd8e-109">関係</span><span class="sxs-lookup"><span data-stu-id="0cd8e-109">Relationships</span></span>
| <span data-ttu-id="0cd8e-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0cd8e-110">Relationship</span></span> | <span data-ttu-id="0cd8e-111">型</span><span class="sxs-lookup"><span data-stu-id="0cd8e-111">Type</span></span>   |<span data-ttu-id="0cd8e-112">説明</span><span class="sxs-lookup"><span data-stu-id="0cd8e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cd8e-113">fill</span><span class="sxs-lookup"><span data-stu-id="0cd8e-113">fill</span></span>|[<span data-ttu-id="0cd8e-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="0cd8e-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="0cd8e-p101">現在のグラフのデータ ラベルの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0cd8e-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="0cd8e-117">font</span><span class="sxs-lookup"><span data-stu-id="0cd8e-117">font</span></span>|[<span data-ttu-id="0cd8e-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="0cd8e-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="0cd8e-119">グラフのデータ ラベルのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="0cd8e-119">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="0cd8e-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0cd8e-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0cd8e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cd8e-121">JSON representation</span></span>

<span data-ttu-id="0cd8e-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0cd8e-122">Here is a JSON representation of the resource.</span></span>

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
