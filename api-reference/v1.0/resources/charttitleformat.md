---
title: ChartTitleFormat リソースの種類
description: グラフ タイトルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c3632c381dcd29247696c50bc235b9662c8d6366
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032887"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="338b6-103">ChartTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="338b6-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="338b6-104">グラフ タイトルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="338b6-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="338b6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="338b6-105">Methods</span></span>
<span data-ttu-id="338b6-106">None</span><span class="sxs-lookup"><span data-stu-id="338b6-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="338b6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="338b6-107">Properties</span></span>
<span data-ttu-id="338b6-108">なし</span><span class="sxs-lookup"><span data-stu-id="338b6-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="338b6-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="338b6-109">Relationships</span></span>
| <span data-ttu-id="338b6-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="338b6-110">Relationship</span></span> | <span data-ttu-id="338b6-111">型</span><span class="sxs-lookup"><span data-stu-id="338b6-111">Type</span></span>   |<span data-ttu-id="338b6-112">説明</span><span class="sxs-lookup"><span data-stu-id="338b6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="338b6-113">fill</span><span class="sxs-lookup"><span data-stu-id="338b6-113">fill</span></span>|[<span data-ttu-id="338b6-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="338b6-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="338b6-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="338b6-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="338b6-117">font</span><span class="sxs-lookup"><span data-stu-id="338b6-117">font</span></span>|[<span data-ttu-id="338b6-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="338b6-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="338b6-119">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="338b6-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="338b6-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="338b6-120">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="338b6-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="338b6-121">JSON representation</span></span>

<span data-ttu-id="338b6-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="338b6-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
