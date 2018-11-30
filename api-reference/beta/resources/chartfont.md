---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
ms.openlocfilehash: a0aa3150cb6ad31b4ad635253fd6ae35647b5ff7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070394"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="ecc6d-103">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecc6d-103">ChartFont resource type</span></span>

> <span data-ttu-id="ecc6d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecc6d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecc6d-106">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-106">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="ecc6d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ecc6d-107">Methods</span></span>

| <span data-ttu-id="ecc6d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ecc6d-108">Method</span></span>           | <span data-ttu-id="ecc6d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ecc6d-109">Return Type</span></span>    |<span data-ttu-id="ecc6d-110">説明</span><span class="sxs-lookup"><span data-stu-id="ecc6d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ecc6d-111">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="ecc6d-111">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="ecc6d-112">ChartFont</span><span class="sxs-lookup"><span data-stu-id="ecc6d-112">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="ecc6d-113">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-113">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="ecc6d-114">Update</span><span class="sxs-lookup"><span data-stu-id="ecc6d-114">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="ecc6d-115">ChartFont</span><span class="sxs-lookup"><span data-stu-id="ecc6d-115">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="ecc6d-116">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-116">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ecc6d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecc6d-117">Properties</span></span>
| <span data-ttu-id="ecc6d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecc6d-118">Property</span></span>     | <span data-ttu-id="ecc6d-119">型</span><span class="sxs-lookup"><span data-stu-id="ecc6d-119">Type</span></span>   |<span data-ttu-id="ecc6d-120">説明</span><span class="sxs-lookup"><span data-stu-id="ecc6d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecc6d-121">bold</span><span class="sxs-lookup"><span data-stu-id="ecc6d-121">bold</span></span>|<span data-ttu-id="ecc6d-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="ecc6d-122">boolean</span></span>|<span data-ttu-id="ecc6d-123">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="ecc6d-124">color</span><span class="sxs-lookup"><span data-stu-id="ecc6d-124">color</span></span>|<span data-ttu-id="ecc6d-125">文字列</span><span class="sxs-lookup"><span data-stu-id="ecc6d-125">string</span></span>|<span data-ttu-id="ecc6d-p102">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="ecc6d-129">italic</span><span class="sxs-lookup"><span data-stu-id="ecc6d-129">italic</span></span>|<span data-ttu-id="ecc6d-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="ecc6d-130">boolean</span></span>|<span data-ttu-id="ecc6d-131">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="ecc6d-132">name</span><span class="sxs-lookup"><span data-stu-id="ecc6d-132">name</span></span>|<span data-ttu-id="ecc6d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ecc6d-133">string</span></span>|<span data-ttu-id="ecc6d-134">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="ecc6d-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="ecc6d-135">size</span><span class="sxs-lookup"><span data-stu-id="ecc6d-135">size</span></span>|<span data-ttu-id="ecc6d-136">double</span><span class="sxs-lookup"><span data-stu-id="ecc6d-136">double</span></span>|<span data-ttu-id="ecc6d-137">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="ecc6d-137">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="ecc6d-138">underline</span><span class="sxs-lookup"><span data-stu-id="ecc6d-138">underline</span></span>|<span data-ttu-id="ecc6d-139">文字列</span><span class="sxs-lookup"><span data-stu-id="ecc6d-139">string</span></span>|<span data-ttu-id="ecc6d-p103">フォントに適用する下線の種類。可能な値は、`None`、`Single` です。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-p103">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecc6d-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ecc6d-142">Relationships</span></span>
<span data-ttu-id="ecc6d-143">なし</span><span class="sxs-lookup"><span data-stu-id="ecc6d-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ecc6d-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecc6d-144">JSON representation</span></span>

<span data-ttu-id="ecc6d-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ecc6d-145">Here is a JSON representation of the resource.</span></span>

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