---
title: ChartLegendFormat リソースの種類
description: グラフの凡例の書式設定プロパティをカプセル化します。
author: lumine2008
ms.openlocfilehash: 6ef6f2d26ade1d8d93489fbc560d4e0eb511bc86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334378"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="1ea22-103">ChartLegendFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1ea22-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="1ea22-104">グラフの凡例の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="1ea22-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="1ea22-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1ea22-105">Methods</span></span>
<span data-ttu-id="1ea22-106">なし</span><span class="sxs-lookup"><span data-stu-id="1ea22-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="1ea22-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ea22-107">Properties</span></span>
<span data-ttu-id="1ea22-108">なし</span><span class="sxs-lookup"><span data-stu-id="1ea22-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1ea22-109">関係</span><span class="sxs-lookup"><span data-stu-id="1ea22-109">Relationships</span></span>
| <span data-ttu-id="1ea22-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ea22-110">Relationship</span></span> | <span data-ttu-id="1ea22-111">型</span><span class="sxs-lookup"><span data-stu-id="1ea22-111">Type</span></span>   |<span data-ttu-id="1ea22-112">説明</span><span class="sxs-lookup"><span data-stu-id="1ea22-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ea22-113">fill</span><span class="sxs-lookup"><span data-stu-id="1ea22-113">fill</span></span>|[<span data-ttu-id="1ea22-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="1ea22-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="1ea22-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1ea22-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="1ea22-117">font</span><span class="sxs-lookup"><span data-stu-id="1ea22-117">font</span></span>|[<span data-ttu-id="1ea22-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="1ea22-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="1ea22-p102">グラフの凡例のフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1ea22-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1ea22-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ea22-121">JSON representation</span></span>

<span data-ttu-id="1ea22-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1ea22-122">Here is a JSON representation of the resource.</span></span>

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