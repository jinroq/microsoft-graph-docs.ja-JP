---
title: workbookChartAxisTitleFormat リソースの種類
description: グラフ軸のタイトルの書式設定を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c98cfee5c776f761c4e84479bb6a4b3f2814bb06
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348841"
---
# <a name="workbookchartaxistitleformat-resource-type"></a><span data-ttu-id="aba10-103">workbookChartAxisTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aba10-103">workbookChartAxisTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aba10-104">グラフ軸のタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="aba10-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="aba10-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="aba10-105">Methods</span></span>
<span data-ttu-id="aba10-106">なし</span><span class="sxs-lookup"><span data-stu-id="aba10-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="aba10-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aba10-107">Properties</span></span>
<span data-ttu-id="aba10-108">なし</span><span class="sxs-lookup"><span data-stu-id="aba10-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="aba10-109">関係</span><span class="sxs-lookup"><span data-stu-id="aba10-109">Relationships</span></span>
| <span data-ttu-id="aba10-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aba10-110">Relationship</span></span> | <span data-ttu-id="aba10-111">型</span><span class="sxs-lookup"><span data-stu-id="aba10-111">Type</span></span>   |<span data-ttu-id="aba10-112">説明</span><span class="sxs-lookup"><span data-stu-id="aba10-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aba10-113">font</span><span class="sxs-lookup"><span data-stu-id="aba10-113">font</span></span>|[<span data-ttu-id="aba10-114">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="aba10-114">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="aba10-115">グラフの軸タイトルのオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="aba10-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="aba10-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aba10-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aba10-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aba10-117">JSON representation</span></span>

<span data-ttu-id="aba10-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aba10-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
