---
title: RangeFormat リソースの種類
description: 範囲のフォント、塗りつぶし、境界線、配置などのプロパティをカプセル化する、書式設定オブジェクトです。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b4018995e37ff40ae014b54d08b77bbed73d6fe2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937349"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="4de7c-103">RangeFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4de7c-103">RangeFormat resource type</span></span>

> <span data-ttu-id="4de7c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4de7c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4de7c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4de7c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4de7c-106">範囲のフォント、塗りつぶし、境界線、配置などのプロパティをカプセル化する、書式設定オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4de7c-106">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="4de7c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4de7c-107">Methods</span></span>

| <span data-ttu-id="4de7c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4de7c-108">Method</span></span>           | <span data-ttu-id="4de7c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4de7c-109">Return Type</span></span>    |<span data-ttu-id="4de7c-110">説明</span><span class="sxs-lookup"><span data-stu-id="4de7c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4de7c-111">RangeFormat を取得する</span><span class="sxs-lookup"><span data-stu-id="4de7c-111">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="4de7c-112">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="4de7c-112">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="4de7c-113">rangeFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4de7c-113">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="4de7c-114">RangeBorder を作成する</span><span class="sxs-lookup"><span data-stu-id="4de7c-114">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="4de7c-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="4de7c-115">RangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="4de7c-116">境界線コレクションに投稿して、新しい RangeBorder を作成します。</span><span class="sxs-lookup"><span data-stu-id="4de7c-116">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="4de7c-117">境界線を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4de7c-117">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="4de7c-118">[RangeBorder](rangeborder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4de7c-118">[RangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="4de7c-119">RangeBorder オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4de7c-119">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="4de7c-120">Update</span><span class="sxs-lookup"><span data-stu-id="4de7c-120">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="4de7c-121">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="4de7c-121">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="4de7c-122">RangeFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4de7c-122">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="4de7c-123">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="4de7c-123">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="4de7c-124">なし</span><span class="sxs-lookup"><span data-stu-id="4de7c-124">None</span></span>|<span data-ttu-id="4de7c-125">現在の列のデータに基づいて、現在の範囲の列の幅を最適な幅に変更します。</span><span class="sxs-lookup"><span data-stu-id="4de7c-125">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="4de7c-126">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="4de7c-126">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="4de7c-127">なし</span><span class="sxs-lookup"><span data-stu-id="4de7c-127">None</span></span>|<span data-ttu-id="4de7c-128">現在の行のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。</span><span class="sxs-lookup"><span data-stu-id="4de7c-128">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="4de7c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4de7c-129">Properties</span></span>
| <span data-ttu-id="4de7c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4de7c-130">Property</span></span>     | <span data-ttu-id="4de7c-131">型</span><span class="sxs-lookup"><span data-stu-id="4de7c-131">Type</span></span>   |<span data-ttu-id="4de7c-132">説明</span><span class="sxs-lookup"><span data-stu-id="4de7c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4de7c-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="4de7c-133">columnWidth</span></span>|<span data-ttu-id="4de7c-134">double</span><span class="sxs-lookup"><span data-stu-id="4de7c-134">double</span></span>|<span data-ttu-id="4de7c-p102">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="4de7c-p102">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="4de7c-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="4de7c-137">horizontalAlignment</span></span>|<span data-ttu-id="4de7c-138">文字列</span><span class="sxs-lookup"><span data-stu-id="4de7c-138">string</span></span>|<span data-ttu-id="4de7c-p103">指定したオブジェクトの水平方向の配置を表します。可能な値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="4de7c-p103">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="4de7c-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="4de7c-141">rowHeight</span></span>|<span data-ttu-id="4de7c-142">double</span><span class="sxs-lookup"><span data-stu-id="4de7c-142">double</span></span>|<span data-ttu-id="4de7c-p104">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="4de7c-p104">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="4de7c-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="4de7c-145">verticalAlignment</span></span>|<span data-ttu-id="4de7c-146">文字列</span><span class="sxs-lookup"><span data-stu-id="4de7c-146">string</span></span>|<span data-ttu-id="4de7c-p105">指定したオブジェクトの垂直方向の配置を表します。可能な値は、`Top`、`Center`、`Bottom`、`Justify`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="4de7c-p105">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="4de7c-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="4de7c-149">wrapText</span></span>|<span data-ttu-id="4de7c-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="4de7c-150">boolean</span></span>|<span data-ttu-id="4de7c-p106">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="4de7c-p106">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="4de7c-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4de7c-153">Relationships</span></span>
| <span data-ttu-id="4de7c-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4de7c-154">Relationship</span></span> | <span data-ttu-id="4de7c-155">型</span><span class="sxs-lookup"><span data-stu-id="4de7c-155">Type</span></span>   |<span data-ttu-id="4de7c-156">説明</span><span class="sxs-lookup"><span data-stu-id="4de7c-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4de7c-157">borders</span><span class="sxs-lookup"><span data-stu-id="4de7c-157">borders</span></span>|<span data-ttu-id="4de7c-158">[RangeBorder](rangeborder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4de7c-158">[RangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="4de7c-159">選択した範囲全体に適用する境界線オブジェクトのコレクションです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4de7c-159">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="4de7c-160">fill</span><span class="sxs-lookup"><span data-stu-id="4de7c-160">fill</span></span>|[<span data-ttu-id="4de7c-161">RangeFill</span><span class="sxs-lookup"><span data-stu-id="4de7c-161">RangeFill</span></span>](rangefill.md)|<span data-ttu-id="4de7c-p107">範囲全体に定義された塗りつぶしオブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4de7c-p107">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="4de7c-164">font</span><span class="sxs-lookup"><span data-stu-id="4de7c-164">font</span></span>|[<span data-ttu-id="4de7c-165">RangeFont</span><span class="sxs-lookup"><span data-stu-id="4de7c-165">RangeFont</span></span>](rangefont.md)|<span data-ttu-id="4de7c-166">選択した範囲全体に定義されているフォント オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4de7c-166">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="4de7c-167">protection</span><span class="sxs-lookup"><span data-stu-id="4de7c-167">protection</span></span>|[<span data-ttu-id="4de7c-168">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="4de7c-168">FormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="4de7c-p108">範囲に対する書式保護オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4de7c-p108">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4de7c-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4de7c-171">JSON representation</span></span>

<span data-ttu-id="4de7c-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4de7c-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
