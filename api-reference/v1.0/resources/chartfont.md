---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9241691296b93eb21e19e10b81f36e692fea0692
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032999"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="a37fc-103">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a37fc-103">ChartFont resource type</span></span>

<span data-ttu-id="a37fc-104">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="a37fc-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="a37fc-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a37fc-105">Methods</span></span>

| <span data-ttu-id="a37fc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a37fc-106">Method</span></span>           | <span data-ttu-id="a37fc-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a37fc-107">Return Type</span></span>    |<span data-ttu-id="a37fc-108">説明</span><span class="sxs-lookup"><span data-stu-id="a37fc-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a37fc-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="a37fc-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="a37fc-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="a37fc-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="a37fc-111">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a37fc-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="a37fc-112">Update</span><span class="sxs-lookup"><span data-stu-id="a37fc-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="a37fc-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="a37fc-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="a37fc-114">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a37fc-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a37fc-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a37fc-115">Properties</span></span>
| <span data-ttu-id="a37fc-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a37fc-116">Property</span></span>     | <span data-ttu-id="a37fc-117">型</span><span class="sxs-lookup"><span data-stu-id="a37fc-117">Type</span></span>   |<span data-ttu-id="a37fc-118">説明</span><span class="sxs-lookup"><span data-stu-id="a37fc-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a37fc-119">bold</span><span class="sxs-lookup"><span data-stu-id="a37fc-119">bold</span></span>|<span data-ttu-id="a37fc-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="a37fc-120">boolean</span></span>|<span data-ttu-id="a37fc-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="a37fc-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="a37fc-122">color</span><span class="sxs-lookup"><span data-stu-id="a37fc-122">color</span></span>|<span data-ttu-id="a37fc-123">string</span><span class="sxs-lookup"><span data-stu-id="a37fc-123">string</span></span>|<span data-ttu-id="a37fc-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="a37fc-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="a37fc-127">italic</span><span class="sxs-lookup"><span data-stu-id="a37fc-127">italic</span></span>|<span data-ttu-id="a37fc-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="a37fc-128">boolean</span></span>|<span data-ttu-id="a37fc-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="a37fc-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="a37fc-130">name</span><span class="sxs-lookup"><span data-stu-id="a37fc-130">name</span></span>|<span data-ttu-id="a37fc-131">string</span><span class="sxs-lookup"><span data-stu-id="a37fc-131">string</span></span>|<span data-ttu-id="a37fc-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="a37fc-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="a37fc-133">size</span><span class="sxs-lookup"><span data-stu-id="a37fc-133">size</span></span>|<span data-ttu-id="a37fc-134">double</span><span class="sxs-lookup"><span data-stu-id="a37fc-134">double</span></span>|<span data-ttu-id="a37fc-135">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="a37fc-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="a37fc-136">underline</span><span class="sxs-lookup"><span data-stu-id="a37fc-136">underline</span></span>|<span data-ttu-id="a37fc-137">文字列</span><span class="sxs-lookup"><span data-stu-id="a37fc-137">string</span></span>|<span data-ttu-id="a37fc-138">フォントに適用する下線の種類。</span><span class="sxs-lookup"><span data-stu-id="a37fc-138">Type of underline applied to the font.</span></span> <span data-ttu-id="a37fc-139">使用可能な値は`None`、 `Single`、です。</span><span class="sxs-lookup"><span data-stu-id="a37fc-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a37fc-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a37fc-140">Relationships</span></span>
<span data-ttu-id="a37fc-141">なし</span><span class="sxs-lookup"><span data-stu-id="a37fc-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a37fc-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a37fc-142">JSON representation</span></span>

<span data-ttu-id="a37fc-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a37fc-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
