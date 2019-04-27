---
title: workbookChartLegendFormat リソースの種類
description: グラフの凡例の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6bd5fd708574950aea8752396b7fd6495ca6b782
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348872"
---
# <a name="workbookchartlegendformat-resource-type"></a><span data-ttu-id="12d6c-103">workbookChartLegendFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12d6c-103">workbookChartLegendFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12d6c-104">グラフの凡例の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="12d6c-104">Encapsulates the format properties of a chart legend.</span></span>

## <a name="methods"></a><span data-ttu-id="12d6c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="12d6c-105">Methods</span></span>
<span data-ttu-id="12d6c-106">なし</span><span class="sxs-lookup"><span data-stu-id="12d6c-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="12d6c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12d6c-107">Properties</span></span>
<span data-ttu-id="12d6c-108">なし</span><span class="sxs-lookup"><span data-stu-id="12d6c-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="12d6c-109">関係</span><span class="sxs-lookup"><span data-stu-id="12d6c-109">Relationships</span></span>
| <span data-ttu-id="12d6c-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="12d6c-110">Relationship</span></span> | <span data-ttu-id="12d6c-111">型</span><span class="sxs-lookup"><span data-stu-id="12d6c-111">Type</span></span>   |<span data-ttu-id="12d6c-112">説明</span><span class="sxs-lookup"><span data-stu-id="12d6c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12d6c-113">fill</span><span class="sxs-lookup"><span data-stu-id="12d6c-113">fill</span></span>|[<span data-ttu-id="12d6c-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="12d6c-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="12d6c-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="12d6c-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="12d6c-117">font</span><span class="sxs-lookup"><span data-stu-id="12d6c-117">font</span></span>|[<span data-ttu-id="12d6c-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="12d6c-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="12d6c-119">グラフの凡例のフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="12d6c-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="12d6c-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12d6c-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="12d6c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12d6c-121">JSON representation</span></span>

<span data-ttu-id="12d6c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="12d6c-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
