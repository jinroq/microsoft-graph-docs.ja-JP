---
title: rangeFormat リソースの種類
description: 範囲のフォント、塗りつぶし、境界線、配置などのプロパティをカプセル化する、書式設定オブジェクトです。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 1394153a09a30c273280dab5469a40e2e0c2c4ad
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572424"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="29f75-103">RangeFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29f75-103">RangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f75-104">範囲のフォント、塗りつぶし、境界線、配置などのプロパティをカプセル化する、書式設定オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="29f75-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="29f75-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="29f75-105">Methods</span></span>

| <span data-ttu-id="29f75-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="29f75-106">Method</span></span>           | <span data-ttu-id="29f75-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="29f75-107">Return Type</span></span>    |<span data-ttu-id="29f75-108">説明</span><span class="sxs-lookup"><span data-stu-id="29f75-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29f75-109">RangeFormat を取得する</span><span class="sxs-lookup"><span data-stu-id="29f75-109">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="29f75-110">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="29f75-110">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="29f75-111">rangeFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="29f75-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="29f75-112">RangeBorder を作成する</span><span class="sxs-lookup"><span data-stu-id="29f75-112">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="29f75-113">rangeBorder</span><span class="sxs-lookup"><span data-stu-id="29f75-113">rangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="29f75-114">境界線コレクションに投稿して、新しい RangeBorder を作成します。</span><span class="sxs-lookup"><span data-stu-id="29f75-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="29f75-115">境界線を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="29f75-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="29f75-116">[rangeBorder](rangeborder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29f75-116">[rangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="29f75-117">RangeBorder オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="29f75-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="29f75-118">Update</span><span class="sxs-lookup"><span data-stu-id="29f75-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="29f75-119">rangeFormat</span><span class="sxs-lookup"><span data-stu-id="29f75-119">rangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="29f75-120">RangeFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="29f75-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="29f75-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="29f75-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="29f75-122">なし</span><span class="sxs-lookup"><span data-stu-id="29f75-122">None</span></span>|<span data-ttu-id="29f75-123">現在の列のデータに基づいて、現在の範囲の列の幅を最適な幅に変更します。</span><span class="sxs-lookup"><span data-stu-id="29f75-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="29f75-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="29f75-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="29f75-125">なし</span><span class="sxs-lookup"><span data-stu-id="29f75-125">None</span></span>|<span data-ttu-id="29f75-126">現在の行のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。</span><span class="sxs-lookup"><span data-stu-id="29f75-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="29f75-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29f75-127">Properties</span></span>
| <span data-ttu-id="29f75-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29f75-128">Property</span></span>     | <span data-ttu-id="29f75-129">型</span><span class="sxs-lookup"><span data-stu-id="29f75-129">Type</span></span>   |<span data-ttu-id="29f75-130">説明</span><span class="sxs-lookup"><span data-stu-id="29f75-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f75-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="29f75-131">columnWidth</span></span>|<span data-ttu-id="29f75-132">double</span><span class="sxs-lookup"><span data-stu-id="29f75-132">double</span></span>|<span data-ttu-id="29f75-p101">範囲内のすべての列の幅を取得または設定します。列の幅が均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="29f75-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="29f75-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="29f75-135">horizontalAlignment</span></span>|<span data-ttu-id="29f75-136">文字列</span><span class="sxs-lookup"><span data-stu-id="29f75-136">string</span></span>|<span data-ttu-id="29f75-p102">指定したオブジェクトの水平方向の配置を表します。可能な値は、`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="29f75-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="29f75-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="29f75-139">rowHeight</span></span>|<span data-ttu-id="29f75-140">double</span><span class="sxs-lookup"><span data-stu-id="29f75-140">double</span></span>|<span data-ttu-id="29f75-p103">範囲内のすべての行の高さを取得または設定します。行の高さが均一でない場合は、null が返されます。</span><span class="sxs-lookup"><span data-stu-id="29f75-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="29f75-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="29f75-143">verticalAlignment</span></span>|<span data-ttu-id="29f75-144">文字列</span><span class="sxs-lookup"><span data-stu-id="29f75-144">string</span></span>|<span data-ttu-id="29f75-p104">指定したオブジェクトの垂直方向の配置を表します。可能な値は、`Top`、`Center`、`Bottom`、`Justify`、`Distributed` です。</span><span class="sxs-lookup"><span data-stu-id="29f75-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="29f75-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="29f75-147">wrapText</span></span>|<span data-ttu-id="29f75-148">boolean</span><span class="sxs-lookup"><span data-stu-id="29f75-148">boolean</span></span>|<span data-ttu-id="29f75-p105">オブジェクト内のテキストを Excel でラップするかどうかを表します。null 値は、範囲全体に一様なラップ設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="29f75-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="29f75-151">関係</span><span class="sxs-lookup"><span data-stu-id="29f75-151">Relationships</span></span>
| <span data-ttu-id="29f75-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29f75-152">Relationship</span></span> | <span data-ttu-id="29f75-153">型</span><span class="sxs-lookup"><span data-stu-id="29f75-153">Type</span></span>   |<span data-ttu-id="29f75-154">説明</span><span class="sxs-lookup"><span data-stu-id="29f75-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f75-155">borders</span><span class="sxs-lookup"><span data-stu-id="29f75-155">borders</span></span>|<span data-ttu-id="29f75-156">[rangeBorder](rangeborder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29f75-156">[rangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="29f75-157">選択した範囲全体に適用する境界線オブジェクトのコレクションです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29f75-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="29f75-158">fill</span><span class="sxs-lookup"><span data-stu-id="29f75-158">fill</span></span>|[<span data-ttu-id="29f75-159">rangeFill</span><span class="sxs-lookup"><span data-stu-id="29f75-159">rangeFill</span></span>](rangefill.md)|<span data-ttu-id="29f75-p106">範囲全体に定義された塗りつぶしオブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29f75-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="29f75-162">font</span><span class="sxs-lookup"><span data-stu-id="29f75-162">font</span></span>|[<span data-ttu-id="29f75-163">rangeFont</span><span class="sxs-lookup"><span data-stu-id="29f75-163">rangeFont</span></span>](rangefont.md)|<span data-ttu-id="29f75-164">選択した範囲全体に定義されているフォント オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29f75-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="29f75-165">protection</span><span class="sxs-lookup"><span data-stu-id="29f75-165">protection</span></span>|[<span data-ttu-id="29f75-166">formatProtection</span><span class="sxs-lookup"><span data-stu-id="29f75-166">formatProtection</span></span>](formatprotection.md)|<span data-ttu-id="29f75-p107">範囲に対する書式保護オブジェクトを返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29f75-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29f75-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29f75-169">JSON representation</span></span>

<span data-ttu-id="29f75-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29f75-170">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangeformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
