---
title: ChartAreaFormat リソースの種類
description: グラフ領域全体の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a447b604807f3ae223445db953d45928eda9f36b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569390"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="82008-103">ChartAreaFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82008-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="82008-104">グラフ領域全体の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="82008-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="82008-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="82008-105">Methods</span></span>
<span data-ttu-id="82008-106">なし</span><span class="sxs-lookup"><span data-stu-id="82008-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="82008-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82008-107">Properties</span></span>
<span data-ttu-id="82008-108">なし</span><span class="sxs-lookup"><span data-stu-id="82008-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="82008-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82008-109">Relationships</span></span>
| <span data-ttu-id="82008-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82008-110">Relationship</span></span> | <span data-ttu-id="82008-111">型</span><span class="sxs-lookup"><span data-stu-id="82008-111">Type</span></span>   |<span data-ttu-id="82008-112">説明</span><span class="sxs-lookup"><span data-stu-id="82008-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82008-113">fill</span><span class="sxs-lookup"><span data-stu-id="82008-113">fill</span></span>|[<span data-ttu-id="82008-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="82008-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="82008-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="82008-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="82008-117">font</span><span class="sxs-lookup"><span data-stu-id="82008-117">font</span></span>|[<span data-ttu-id="82008-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="82008-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="82008-119">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="82008-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="82008-120">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="82008-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82008-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82008-121">JSON representation</span></span>

<span data-ttu-id="82008-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82008-122">Here is a JSON representation of the resource.</span></span>

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
