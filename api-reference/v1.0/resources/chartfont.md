---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
ms.openlocfilehash: dc4b1f8cd0653d89c3486a61604dd09c0e23cb2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021362"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="2f696-103">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f696-103">ChartFont resource type</span></span>

<span data-ttu-id="2f696-104">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="2f696-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="2f696-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2f696-105">Methods</span></span>

| <span data-ttu-id="2f696-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2f696-106">Method</span></span>           | <span data-ttu-id="2f696-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2f696-107">Return Type</span></span>    |<span data-ttu-id="2f696-108">説明</span><span class="sxs-lookup"><span data-stu-id="2f696-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f696-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="2f696-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="2f696-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="2f696-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="2f696-111">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2f696-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="2f696-112">Update</span><span class="sxs-lookup"><span data-stu-id="2f696-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="2f696-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="2f696-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="2f696-114">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2f696-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2f696-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f696-115">Properties</span></span>
| <span data-ttu-id="2f696-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f696-116">Property</span></span>     | <span data-ttu-id="2f696-117">型</span><span class="sxs-lookup"><span data-stu-id="2f696-117">Type</span></span>   |<span data-ttu-id="2f696-118">説明</span><span class="sxs-lookup"><span data-stu-id="2f696-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f696-119">bold</span><span class="sxs-lookup"><span data-stu-id="2f696-119">bold</span></span>|<span data-ttu-id="2f696-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="2f696-120">boolean</span></span>|<span data-ttu-id="2f696-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2f696-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="2f696-122">color</span><span class="sxs-lookup"><span data-stu-id="2f696-122">color</span></span>|<span data-ttu-id="2f696-123">文字列</span><span class="sxs-lookup"><span data-stu-id="2f696-123">string</span></span>|<span data-ttu-id="2f696-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="2f696-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="2f696-127">italic</span><span class="sxs-lookup"><span data-stu-id="2f696-127">italic</span></span>|<span data-ttu-id="2f696-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="2f696-128">boolean</span></span>|<span data-ttu-id="2f696-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2f696-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="2f696-130">name</span><span class="sxs-lookup"><span data-stu-id="2f696-130">name</span></span>|<span data-ttu-id="2f696-131">文字列</span><span class="sxs-lookup"><span data-stu-id="2f696-131">string</span></span>|<span data-ttu-id="2f696-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="2f696-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="2f696-133">size</span><span class="sxs-lookup"><span data-stu-id="2f696-133">size</span></span>|<span data-ttu-id="2f696-134">double</span><span class="sxs-lookup"><span data-stu-id="2f696-134">double</span></span>|<span data-ttu-id="2f696-135">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="2f696-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="2f696-136">underline</span><span class="sxs-lookup"><span data-stu-id="2f696-136">underline</span></span>|<span data-ttu-id="2f696-137">文字列</span><span class="sxs-lookup"><span data-stu-id="2f696-137">string</span></span>|<span data-ttu-id="2f696-138">フォントに適用する下線の種類です。</span><span class="sxs-lookup"><span data-stu-id="2f696-138">Type of underline applied to the font.</span></span> <span data-ttu-id="2f696-139">可能な値: `None`、 `Single`。</span><span class="sxs-lookup"><span data-stu-id="2f696-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f696-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2f696-140">Relationships</span></span>
<span data-ttu-id="2f696-141">なし</span><span class="sxs-lookup"><span data-stu-id="2f696-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2f696-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f696-142">JSON representation</span></span>

<span data-ttu-id="2f696-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2f696-143">Here is a JSON representation of the resource.</span></span>

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