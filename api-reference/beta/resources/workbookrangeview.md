---
title: rangeView リソースの種類
description: RangeView は、親の範囲の表示されているセルのセットを表します。
author: lumine2008
ms.openlocfilehash: a5157d3917f9f4ed51437d9ae9854194b85ae4d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359487"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="77ebd-103">rangeView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77ebd-103">rangeView resource type</span></span>

> <span data-ttu-id="77ebd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77ebd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77ebd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77ebd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77ebd-106">RangeView は、親の範囲の表示されているセルのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="77ebd-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="77ebd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="77ebd-107">Methods</span></span>

| <span data-ttu-id="77ebd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="77ebd-108">Method</span></span>           | <span data-ttu-id="77ebd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="77ebd-109">Return Type</span></span>    |<span data-ttu-id="77ebd-110">説明</span><span class="sxs-lookup"><span data-stu-id="77ebd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77ebd-111">行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="77ebd-111">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="77ebd-112">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="77ebd-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="77ebd-113">workbookRangeView オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="77ebd-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="77ebd-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="77ebd-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="77ebd-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="77ebd-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="77ebd-116">インデックスに基づいて範囲ビューの項目を取得します。</span><span class="sxs-lookup"><span data-stu-id="77ebd-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="77ebd-117">Range</span><span class="sxs-lookup"><span data-stu-id="77ebd-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="77ebd-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="77ebd-118">workbookRange</span></span>](range.md)|<span data-ttu-id="77ebd-119">範囲ビューに関連付けられた範囲オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77ebd-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="77ebd-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77ebd-120">Properties</span></span>
| <span data-ttu-id="77ebd-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77ebd-121">Property</span></span>     | <span data-ttu-id="77ebd-122">種類</span><span class="sxs-lookup"><span data-stu-id="77ebd-122">Type</span></span>   |<span data-ttu-id="77ebd-123">説明</span><span class="sxs-lookup"><span data-stu-id="77ebd-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77ebd-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="77ebd-124">columnCount</span></span>|<span data-ttu-id="77ebd-125">Int32</span><span class="sxs-lookup"><span data-stu-id="77ebd-125">Int32</span></span>|<span data-ttu-id="77ebd-p102">表示されている列の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="77ebd-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="77ebd-128">formulas</span><span class="sxs-lookup"><span data-stu-id="77ebd-128">formulas</span></span>|<span data-ttu-id="77ebd-129">Json</span><span class="sxs-lookup"><span data-stu-id="77ebd-129">Json</span></span>|<span data-ttu-id="77ebd-130">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="77ebd-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="77ebd-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="77ebd-131">formulasLocal</span></span>|<span data-ttu-id="77ebd-132">Json</span><span class="sxs-lookup"><span data-stu-id="77ebd-132">Json</span></span>|<span data-ttu-id="77ebd-p103">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="77ebd-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="77ebd-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="77ebd-135">formulasR1C1</span></span>|<span data-ttu-id="77ebd-136">Json</span><span class="sxs-lookup"><span data-stu-id="77ebd-136">Json</span></span>|<span data-ttu-id="77ebd-137">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="77ebd-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="77ebd-138">index</span><span class="sxs-lookup"><span data-stu-id="77ebd-138">index</span></span>|<span data-ttu-id="77ebd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="77ebd-139">Int32</span></span>|<span data-ttu-id="77ebd-140">範囲のインデックス。</span><span class="sxs-lookup"><span data-stu-id="77ebd-140">Index of the range.</span></span>|
|<span data-ttu-id="77ebd-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="77ebd-141">numberFormat</span></span>|<span data-ttu-id="77ebd-142">Json</span><span class="sxs-lookup"><span data-stu-id="77ebd-142">Json</span></span>|<span data-ttu-id="77ebd-p104">指定したセルの Excel の数値書式コードを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="77ebd-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="77ebd-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="77ebd-145">rowCount</span></span>|<span data-ttu-id="77ebd-146">Int32</span><span class="sxs-lookup"><span data-stu-id="77ebd-146">Int32</span></span>|<span data-ttu-id="77ebd-p105">表示されている行の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="77ebd-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="77ebd-149">text</span><span class="sxs-lookup"><span data-stu-id="77ebd-149">text</span></span>|<span data-ttu-id="77ebd-150">Json</span><span class="sxs-lookup"><span data-stu-id="77ebd-150">Json</span></span>|<span data-ttu-id="77ebd-p106">指定した範囲のテキスト値。テキスト値は、セルの幅には依存しません。Excel UI で発生する # 記号による置換は、この API から返されるテキスト値には影響しません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="77ebd-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="77ebd-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="77ebd-155">valueTypes</span></span>|<span data-ttu-id="77ebd-156">Json</span><span class="sxs-lookup"><span data-stu-id="77ebd-156">Json</span></span>|<span data-ttu-id="77ebd-p107">各セルのデータの種類を表します。読み取り専用です。使用可能な値は次のとおりです。Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="77ebd-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="77ebd-160">values</span><span class="sxs-lookup"><span data-stu-id="77ebd-160">values</span></span>|<span data-ttu-id="77ebd-161">Json</span><span class="sxs-lookup"><span data-stu-id="77ebd-161">Json</span></span>|<span data-ttu-id="77ebd-p108">指定した範囲ビューの Raw 値を表します。返されるデータの型は、文字列、数値、ブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="77ebd-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="77ebd-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="77ebd-165">Relationships</span></span>
| <span data-ttu-id="77ebd-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="77ebd-166">Relationship</span></span> | <span data-ttu-id="77ebd-167">型</span><span class="sxs-lookup"><span data-stu-id="77ebd-167">Type</span></span>   |<span data-ttu-id="77ebd-168">説明</span><span class="sxs-lookup"><span data-stu-id="77ebd-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77ebd-169">rows</span><span class="sxs-lookup"><span data-stu-id="77ebd-169">rows</span></span>|<span data-ttu-id="77ebd-170">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="77ebd-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="77ebd-p109">範囲に関連付けられている範囲ビューのコレクションを表します。読み取り専用です。  読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="77ebd-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77ebd-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77ebd-174">JSON representation</span></span>
<span data-ttu-id="77ebd-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="77ebd-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```