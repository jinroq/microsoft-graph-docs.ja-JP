---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
ms.openlocfilehash: 9b2d6e07f5049449d71be45b41585ed3bd300b7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850786"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="e7fe0-103">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7fe0-103">ChartFont resource type</span></span>

<span data-ttu-id="e7fe0-104">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="e7fe0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7fe0-105">Methods</span></span>

| <span data-ttu-id="e7fe0-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7fe0-106">Method</span></span>           | <span data-ttu-id="e7fe0-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e7fe0-107">Return Type</span></span>    |<span data-ttu-id="e7fe0-108">説明</span><span class="sxs-lookup"><span data-stu-id="e7fe0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7fe0-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="e7fe0-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="e7fe0-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e7fe0-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="e7fe0-111">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="e7fe0-112">Update</span><span class="sxs-lookup"><span data-stu-id="e7fe0-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="e7fe0-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e7fe0-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="e7fe0-114">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7fe0-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7fe0-115">Properties</span></span>
| <span data-ttu-id="e7fe0-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7fe0-116">Property</span></span>     | <span data-ttu-id="e7fe0-117">種類</span><span class="sxs-lookup"><span data-stu-id="e7fe0-117">Type</span></span>   |<span data-ttu-id="e7fe0-118">説明</span><span class="sxs-lookup"><span data-stu-id="e7fe0-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7fe0-119">bold</span><span class="sxs-lookup"><span data-stu-id="e7fe0-119">bold</span></span>|<span data-ttu-id="e7fe0-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="e7fe0-120">boolean</span></span>|<span data-ttu-id="e7fe0-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="e7fe0-122">color</span><span class="sxs-lookup"><span data-stu-id="e7fe0-122">color</span></span>|<span data-ttu-id="e7fe0-123">文字列</span><span class="sxs-lookup"><span data-stu-id="e7fe0-123">string</span></span>|<span data-ttu-id="e7fe0-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="e7fe0-127">italic</span><span class="sxs-lookup"><span data-stu-id="e7fe0-127">italic</span></span>|<span data-ttu-id="e7fe0-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="e7fe0-128">boolean</span></span>|<span data-ttu-id="e7fe0-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="e7fe0-130">name</span><span class="sxs-lookup"><span data-stu-id="e7fe0-130">name</span></span>|<span data-ttu-id="e7fe0-131">文字列</span><span class="sxs-lookup"><span data-stu-id="e7fe0-131">string</span></span>|<span data-ttu-id="e7fe0-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="e7fe0-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="e7fe0-133">size</span><span class="sxs-lookup"><span data-stu-id="e7fe0-133">size</span></span>|<span data-ttu-id="e7fe0-134">double</span><span class="sxs-lookup"><span data-stu-id="e7fe0-134">double</span></span>|<span data-ttu-id="e7fe0-135">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="e7fe0-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="e7fe0-136">underline</span><span class="sxs-lookup"><span data-stu-id="e7fe0-136">underline</span></span>|<span data-ttu-id="e7fe0-137">文字列</span><span class="sxs-lookup"><span data-stu-id="e7fe0-137">string</span></span>|<span data-ttu-id="e7fe0-138">フォントに適用する下線の種類です。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-138">Type of underline applied to the font.</span></span> <span data-ttu-id="e7fe0-139">可能な値: `None`、 `Single`。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7fe0-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7fe0-140">Relationships</span></span>
<span data-ttu-id="e7fe0-141">なし</span><span class="sxs-lookup"><span data-stu-id="e7fe0-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e7fe0-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7fe0-142">JSON representation</span></span>

<span data-ttu-id="e7fe0-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7fe0-143">Here is a JSON representation of the resource.</span></span>

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
