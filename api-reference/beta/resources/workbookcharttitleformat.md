---
title: workbookChartTitleFormat リソースの種類
description: グラフ タイトルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3827b44ae24a63f8fe048575633cc3b5508ac300
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348902"
---
# <a name="workbookcharttitleformat-resource-type"></a><span data-ttu-id="f1356-103">workbookChartTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1356-103">workbookChartTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1356-104">グラフ タイトルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="f1356-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="f1356-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f1356-105">Methods</span></span>
<span data-ttu-id="f1356-106">なし</span><span class="sxs-lookup"><span data-stu-id="f1356-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f1356-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1356-107">Properties</span></span>
<span data-ttu-id="f1356-108">なし</span><span class="sxs-lookup"><span data-stu-id="f1356-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f1356-109">関係</span><span class="sxs-lookup"><span data-stu-id="f1356-109">Relationships</span></span>
| <span data-ttu-id="f1356-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1356-110">Relationship</span></span> | <span data-ttu-id="f1356-111">型</span><span class="sxs-lookup"><span data-stu-id="f1356-111">Type</span></span>   |<span data-ttu-id="f1356-112">説明</span><span class="sxs-lookup"><span data-stu-id="f1356-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1356-113">fill</span><span class="sxs-lookup"><span data-stu-id="f1356-113">fill</span></span>|[<span data-ttu-id="f1356-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="f1356-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="f1356-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f1356-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="f1356-117">font</span><span class="sxs-lookup"><span data-stu-id="f1356-117">font</span></span>|[<span data-ttu-id="f1356-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="f1356-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="f1356-119">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="f1356-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="f1356-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f1356-120">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="f1356-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1356-121">JSON representation</span></span>

<span data-ttu-id="f1356-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1356-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
