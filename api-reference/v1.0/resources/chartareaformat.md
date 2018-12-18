---
title: ChartAreaFormat リソースの種類
description: グラフ領域全体の書式設定プロパティをカプセル化します。
author: lumine2008
ms.openlocfilehash: d9db44fefeff00ae6f7363126de35d4028964d14
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310004"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="5f283-103">ChartAreaFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f283-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="5f283-104">グラフ領域全体の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="5f283-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="5f283-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5f283-105">Methods</span></span>
<span data-ttu-id="5f283-106">なし</span><span class="sxs-lookup"><span data-stu-id="5f283-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="5f283-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f283-107">Properties</span></span>
<span data-ttu-id="5f283-108">なし</span><span class="sxs-lookup"><span data-stu-id="5f283-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5f283-109">関係</span><span class="sxs-lookup"><span data-stu-id="5f283-109">Relationships</span></span>
| <span data-ttu-id="5f283-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5f283-110">Relationship</span></span> | <span data-ttu-id="5f283-111">型</span><span class="sxs-lookup"><span data-stu-id="5f283-111">Type</span></span>   |<span data-ttu-id="5f283-112">説明</span><span class="sxs-lookup"><span data-stu-id="5f283-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f283-113">fill</span><span class="sxs-lookup"><span data-stu-id="5f283-113">fill</span></span>|[<span data-ttu-id="5f283-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="5f283-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="5f283-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5f283-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="5f283-117">font</span><span class="sxs-lookup"><span data-stu-id="5f283-117">font</span></span>|[<span data-ttu-id="5f283-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="5f283-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="5f283-p102">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5f283-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f283-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f283-121">JSON representation</span></span>

<span data-ttu-id="5f283-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5f283-122">Here is a JSON representation of the resource.</span></span>

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