---
title: ChartTitleFormat リソースの種類
description: グラフ タイトルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3a2c16d37d2ca86d7cafbb4047ee0bcea1ee4bde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977116"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="6a9e1-103">ChartTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a9e1-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="6a9e1-104">グラフ タイトルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="6a9e1-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="6a9e1-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a9e1-105">Methods</span></span>
<span data-ttu-id="6a9e1-106">なし</span><span class="sxs-lookup"><span data-stu-id="6a9e1-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="6a9e1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a9e1-107">Properties</span></span>
<span data-ttu-id="6a9e1-108">なし</span><span class="sxs-lookup"><span data-stu-id="6a9e1-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6a9e1-109">関係</span><span class="sxs-lookup"><span data-stu-id="6a9e1-109">Relationships</span></span>
| <span data-ttu-id="6a9e1-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a9e1-110">Relationship</span></span> | <span data-ttu-id="6a9e1-111">型</span><span class="sxs-lookup"><span data-stu-id="6a9e1-111">Type</span></span>   |<span data-ttu-id="6a9e1-112">説明</span><span class="sxs-lookup"><span data-stu-id="6a9e1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a9e1-113">fill</span><span class="sxs-lookup"><span data-stu-id="6a9e1-113">fill</span></span>|[<span data-ttu-id="6a9e1-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="6a9e1-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="6a9e1-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6a9e1-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="6a9e1-117">font</span><span class="sxs-lookup"><span data-stu-id="6a9e1-117">font</span></span>|[<span data-ttu-id="6a9e1-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="6a9e1-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="6a9e1-p102">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6a9e1-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="6a9e1-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a9e1-121">JSON representation</span></span>

<span data-ttu-id="6a9e1-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a9e1-122">Here is a JSON representation of the resource.</span></span>

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
