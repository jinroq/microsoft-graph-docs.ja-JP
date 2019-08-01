---
title: ChartLegendFormat リソースの種類
description: グラフの凡例の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2148b6b5baf8bb680f85954d000da097bcf8f0b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032957"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="0d377-103">ChartLegendFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d377-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="0d377-104">グラフの凡例の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="0d377-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="0d377-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d377-105">Methods</span></span>
<span data-ttu-id="0d377-106">None</span><span class="sxs-lookup"><span data-stu-id="0d377-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0d377-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d377-107">Properties</span></span>
<span data-ttu-id="0d377-108">なし</span><span class="sxs-lookup"><span data-stu-id="0d377-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0d377-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0d377-109">Relationships</span></span>
| <span data-ttu-id="0d377-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0d377-110">Relationship</span></span> | <span data-ttu-id="0d377-111">型</span><span class="sxs-lookup"><span data-stu-id="0d377-111">Type</span></span>   |<span data-ttu-id="0d377-112">説明</span><span class="sxs-lookup"><span data-stu-id="0d377-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d377-113">fill</span><span class="sxs-lookup"><span data-stu-id="0d377-113">fill</span></span>|[<span data-ttu-id="0d377-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="0d377-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="0d377-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0d377-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="0d377-117">font</span><span class="sxs-lookup"><span data-stu-id="0d377-117">font</span></span>|[<span data-ttu-id="0d377-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="0d377-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="0d377-119">グラフの凡例のフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="0d377-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="0d377-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0d377-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0d377-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d377-121">JSON representation</span></span>

<span data-ttu-id="0d377-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0d377-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
