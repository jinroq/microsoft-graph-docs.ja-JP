---
title: workbookChartAreaFormat リソースの種類
description: グラフ領域全体の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6554604e2bb4c49d7e14546f1c5079690f99637f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348843"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="f1ff2-103">workbookChartAreaFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1ff2-103">workbookChartAreaFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1ff2-104">グラフ領域全体の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="f1ff2-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="f1ff2-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f1ff2-105">Methods</span></span>
<span data-ttu-id="f1ff2-106">なし</span><span class="sxs-lookup"><span data-stu-id="f1ff2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f1ff2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1ff2-107">Properties</span></span>
<span data-ttu-id="f1ff2-108">なし</span><span class="sxs-lookup"><span data-stu-id="f1ff2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f1ff2-109">関係</span><span class="sxs-lookup"><span data-stu-id="f1ff2-109">Relationships</span></span>
| <span data-ttu-id="f1ff2-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1ff2-110">Relationship</span></span> | <span data-ttu-id="f1ff2-111">型</span><span class="sxs-lookup"><span data-stu-id="f1ff2-111">Type</span></span>   |<span data-ttu-id="f1ff2-112">説明</span><span class="sxs-lookup"><span data-stu-id="f1ff2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1ff2-113">fill</span><span class="sxs-lookup"><span data-stu-id="f1ff2-113">fill</span></span>|[<span data-ttu-id="f1ff2-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="f1ff2-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="f1ff2-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f1ff2-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="f1ff2-117">font</span><span class="sxs-lookup"><span data-stu-id="f1ff2-117">font</span></span>|[<span data-ttu-id="f1ff2-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="f1ff2-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="f1ff2-119">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="f1ff2-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="f1ff2-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f1ff2-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1ff2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1ff2-121">JSON representation</span></span>

<span data-ttu-id="f1ff2-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1ff2-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
