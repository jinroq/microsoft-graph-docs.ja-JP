---
title: ChartAxisTitleFormat リソースの種類
description: グラフ軸のタイトルの書式設定を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3ae74b7353a0b4198b42a04fdd420eb3447d4c11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029849"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="b656d-103">ChartAxisTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b656d-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="b656d-104">グラフ軸のタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="b656d-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="b656d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b656d-105">Methods</span></span>
<span data-ttu-id="b656d-106">None</span><span class="sxs-lookup"><span data-stu-id="b656d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="b656d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b656d-107">Properties</span></span>
<span data-ttu-id="b656d-108">なし</span><span class="sxs-lookup"><span data-stu-id="b656d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b656d-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b656d-109">Relationships</span></span>
| <span data-ttu-id="b656d-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b656d-110">Relationship</span></span> | <span data-ttu-id="b656d-111">型</span><span class="sxs-lookup"><span data-stu-id="b656d-111">Type</span></span>   |<span data-ttu-id="b656d-112">説明</span><span class="sxs-lookup"><span data-stu-id="b656d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b656d-113">font</span><span class="sxs-lookup"><span data-stu-id="b656d-113">font</span></span>|[<span data-ttu-id="b656d-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b656d-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="b656d-115">グラフの軸タイトルのオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="b656d-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="b656d-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b656d-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b656d-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b656d-117">JSON representation</span></span>

<span data-ttu-id="b656d-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b656d-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
