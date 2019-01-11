---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
ms.openlocfilehash: 0df14f98993c33b6b3eb3c0b2ea9fbdf211a8124
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824165"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="55f8a-103">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55f8a-103">ChartFont resource type</span></span>

> <span data-ttu-id="55f8a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="55f8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55f8a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55f8a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55f8a-106">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="55f8a-106">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="55f8a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="55f8a-107">Methods</span></span>

| <span data-ttu-id="55f8a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="55f8a-108">Method</span></span>           | <span data-ttu-id="55f8a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="55f8a-109">Return Type</span></span>    |<span data-ttu-id="55f8a-110">説明</span><span class="sxs-lookup"><span data-stu-id="55f8a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55f8a-111">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="55f8a-111">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="55f8a-112">ChartFont</span><span class="sxs-lookup"><span data-stu-id="55f8a-112">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="55f8a-113">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="55f8a-113">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="55f8a-114">Update</span><span class="sxs-lookup"><span data-stu-id="55f8a-114">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="55f8a-115">ChartFont</span><span class="sxs-lookup"><span data-stu-id="55f8a-115">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="55f8a-116">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="55f8a-116">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="55f8a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55f8a-117">Properties</span></span>
| <span data-ttu-id="55f8a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55f8a-118">Property</span></span>     | <span data-ttu-id="55f8a-119">種類</span><span class="sxs-lookup"><span data-stu-id="55f8a-119">Type</span></span>   |<span data-ttu-id="55f8a-120">説明</span><span class="sxs-lookup"><span data-stu-id="55f8a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55f8a-121">bold</span><span class="sxs-lookup"><span data-stu-id="55f8a-121">bold</span></span>|<span data-ttu-id="55f8a-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="55f8a-122">boolean</span></span>|<span data-ttu-id="55f8a-123">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="55f8a-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="55f8a-124">color</span><span class="sxs-lookup"><span data-stu-id="55f8a-124">color</span></span>|<span data-ttu-id="55f8a-125">文字列</span><span class="sxs-lookup"><span data-stu-id="55f8a-125">string</span></span>|<span data-ttu-id="55f8a-p102">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="55f8a-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="55f8a-129">italic</span><span class="sxs-lookup"><span data-stu-id="55f8a-129">italic</span></span>|<span data-ttu-id="55f8a-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="55f8a-130">boolean</span></span>|<span data-ttu-id="55f8a-131">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="55f8a-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="55f8a-132">name</span><span class="sxs-lookup"><span data-stu-id="55f8a-132">name</span></span>|<span data-ttu-id="55f8a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="55f8a-133">string</span></span>|<span data-ttu-id="55f8a-134">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="55f8a-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="55f8a-135">size</span><span class="sxs-lookup"><span data-stu-id="55f8a-135">size</span></span>|<span data-ttu-id="55f8a-136">double</span><span class="sxs-lookup"><span data-stu-id="55f8a-136">double</span></span>|<span data-ttu-id="55f8a-137">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="55f8a-137">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="55f8a-138">underline</span><span class="sxs-lookup"><span data-stu-id="55f8a-138">underline</span></span>|<span data-ttu-id="55f8a-139">文字列</span><span class="sxs-lookup"><span data-stu-id="55f8a-139">string</span></span>|<span data-ttu-id="55f8a-p103">フォントに適用する下線の種類。可能な値は、`None`、`Single` です。</span><span class="sxs-lookup"><span data-stu-id="55f8a-p103">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55f8a-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="55f8a-142">Relationships</span></span>
<span data-ttu-id="55f8a-143">なし</span><span class="sxs-lookup"><span data-stu-id="55f8a-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="55f8a-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55f8a-144">JSON representation</span></span>

<span data-ttu-id="55f8a-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="55f8a-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
