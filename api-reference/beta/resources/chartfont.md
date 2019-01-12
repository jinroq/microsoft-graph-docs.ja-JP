---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4187d2837835520864ec3a1ef5c47b578b3d3da4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920948"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="13901-103">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13901-103">ChartFont resource type</span></span>

> <span data-ttu-id="13901-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13901-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13901-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13901-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13901-106">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="13901-106">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="13901-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="13901-107">Methods</span></span>

| <span data-ttu-id="13901-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="13901-108">Method</span></span>           | <span data-ttu-id="13901-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="13901-109">Return Type</span></span>    |<span data-ttu-id="13901-110">説明</span><span class="sxs-lookup"><span data-stu-id="13901-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13901-111">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="13901-111">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="13901-112">ChartFont</span><span class="sxs-lookup"><span data-stu-id="13901-112">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="13901-113">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="13901-113">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="13901-114">Update</span><span class="sxs-lookup"><span data-stu-id="13901-114">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="13901-115">ChartFont</span><span class="sxs-lookup"><span data-stu-id="13901-115">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="13901-116">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="13901-116">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="13901-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13901-117">Properties</span></span>
| <span data-ttu-id="13901-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13901-118">Property</span></span>     | <span data-ttu-id="13901-119">型</span><span class="sxs-lookup"><span data-stu-id="13901-119">Type</span></span>   |<span data-ttu-id="13901-120">説明</span><span class="sxs-lookup"><span data-stu-id="13901-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13901-121">bold</span><span class="sxs-lookup"><span data-stu-id="13901-121">bold</span></span>|<span data-ttu-id="13901-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="13901-122">boolean</span></span>|<span data-ttu-id="13901-123">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="13901-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="13901-124">color</span><span class="sxs-lookup"><span data-stu-id="13901-124">color</span></span>|<span data-ttu-id="13901-125">文字列</span><span class="sxs-lookup"><span data-stu-id="13901-125">string</span></span>|<span data-ttu-id="13901-p102">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="13901-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="13901-129">italic</span><span class="sxs-lookup"><span data-stu-id="13901-129">italic</span></span>|<span data-ttu-id="13901-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="13901-130">boolean</span></span>|<span data-ttu-id="13901-131">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="13901-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="13901-132">name</span><span class="sxs-lookup"><span data-stu-id="13901-132">name</span></span>|<span data-ttu-id="13901-133">文字列</span><span class="sxs-lookup"><span data-stu-id="13901-133">string</span></span>|<span data-ttu-id="13901-134">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="13901-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="13901-135">size</span><span class="sxs-lookup"><span data-stu-id="13901-135">size</span></span>|<span data-ttu-id="13901-136">double</span><span class="sxs-lookup"><span data-stu-id="13901-136">double</span></span>|<span data-ttu-id="13901-137">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="13901-137">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="13901-138">underline</span><span class="sxs-lookup"><span data-stu-id="13901-138">underline</span></span>|<span data-ttu-id="13901-139">文字列</span><span class="sxs-lookup"><span data-stu-id="13901-139">string</span></span>|<span data-ttu-id="13901-p103">フォントに適用する下線の種類。可能な値は、`None`、`Single` です。</span><span class="sxs-lookup"><span data-stu-id="13901-p103">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13901-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13901-142">Relationships</span></span>
<span data-ttu-id="13901-143">なし</span><span class="sxs-lookup"><span data-stu-id="13901-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="13901-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13901-144">JSON representation</span></span>

<span data-ttu-id="13901-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13901-145">Here is a JSON representation of the resource.</span></span>

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
