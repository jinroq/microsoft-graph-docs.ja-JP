---
title: ChartTitleFormat リソースの種類
description: グラフ タイトルの書式設定プロパティをカプセル化します。
author: lumine2008
ms.openlocfilehash: 16169af251a0764c99ae04c5516ad9d552d1654c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362140"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="45bc3-103">ChartTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45bc3-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="45bc3-104">グラフ タイトルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="45bc3-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="45bc3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="45bc3-105">Methods</span></span>
<span data-ttu-id="45bc3-106">なし</span><span class="sxs-lookup"><span data-stu-id="45bc3-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="45bc3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45bc3-107">Properties</span></span>
<span data-ttu-id="45bc3-108">なし</span><span class="sxs-lookup"><span data-stu-id="45bc3-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="45bc3-109">関係</span><span class="sxs-lookup"><span data-stu-id="45bc3-109">Relationships</span></span>
| <span data-ttu-id="45bc3-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="45bc3-110">Relationship</span></span> | <span data-ttu-id="45bc3-111">型</span><span class="sxs-lookup"><span data-stu-id="45bc3-111">Type</span></span>   |<span data-ttu-id="45bc3-112">説明</span><span class="sxs-lookup"><span data-stu-id="45bc3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45bc3-113">fill</span><span class="sxs-lookup"><span data-stu-id="45bc3-113">fill</span></span>|[<span data-ttu-id="45bc3-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="45bc3-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="45bc3-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="45bc3-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="45bc3-117">font</span><span class="sxs-lookup"><span data-stu-id="45bc3-117">font</span></span>|[<span data-ttu-id="45bc3-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="45bc3-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="45bc3-p102">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="45bc3-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="45bc3-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45bc3-121">JSON representation</span></span>

<span data-ttu-id="45bc3-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="45bc3-122">Here is a JSON representation of the resource.</span></span>

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
