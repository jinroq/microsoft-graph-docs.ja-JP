---
title: ChartAreaFormat リソースの種類
description: グラフ領域全体の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ee39e1fc58fe604ff24433dcb540b44e22bb3ee9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033006"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="e3ab3-103">ChartAreaFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e3ab3-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="e3ab3-104">グラフ領域全体の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="e3ab3-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="e3ab3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3ab3-105">Methods</span></span>
<span data-ttu-id="e3ab3-106">None</span><span class="sxs-lookup"><span data-stu-id="e3ab3-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e3ab3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3ab3-107">Properties</span></span>
<span data-ttu-id="e3ab3-108">なし</span><span class="sxs-lookup"><span data-stu-id="e3ab3-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e3ab3-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3ab3-109">Relationships</span></span>
| <span data-ttu-id="e3ab3-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3ab3-110">Relationship</span></span> | <span data-ttu-id="e3ab3-111">型</span><span class="sxs-lookup"><span data-stu-id="e3ab3-111">Type</span></span>   |<span data-ttu-id="e3ab3-112">説明</span><span class="sxs-lookup"><span data-stu-id="e3ab3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3ab3-113">fill</span><span class="sxs-lookup"><span data-stu-id="e3ab3-113">fill</span></span>|[<span data-ttu-id="e3ab3-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="e3ab3-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="e3ab3-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e3ab3-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="e3ab3-117">font</span><span class="sxs-lookup"><span data-stu-id="e3ab3-117">font</span></span>|[<span data-ttu-id="e3ab3-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e3ab3-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e3ab3-119">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="e3ab3-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="e3ab3-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e3ab3-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3ab3-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e3ab3-121">JSON representation</span></span>

<span data-ttu-id="e3ab3-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e3ab3-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
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
