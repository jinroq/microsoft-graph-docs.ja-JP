---
title: rangeView リソースの種類
description: RangeView は、親の範囲の表示されているセルのセットを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 745ed45b4e5b79c8d1764a86fac04cf7fcfdcc26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957803"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="de264-103">rangeView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de264-103">rangeView resource type</span></span>
<span data-ttu-id="de264-104">RangeView は、親の範囲の表示されているセルのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="de264-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="de264-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="de264-105">Methods</span></span>

| <span data-ttu-id="de264-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="de264-106">Method</span></span>           | <span data-ttu-id="de264-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="de264-107">Return Type</span></span>    |<span data-ttu-id="de264-108">説明</span><span class="sxs-lookup"><span data-stu-id="de264-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de264-109">行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="de264-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="de264-110">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="de264-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="de264-111">workbookRangeView オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="de264-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="de264-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="de264-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="de264-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="de264-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="de264-114">インデックスに基づいて範囲ビューの項目を取得します。</span><span class="sxs-lookup"><span data-stu-id="de264-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="de264-115">Range</span><span class="sxs-lookup"><span data-stu-id="de264-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="de264-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="de264-116">workbookRange</span></span>](range.md)|<span data-ttu-id="de264-117">範囲ビューに関連付けられた範囲オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="de264-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="de264-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de264-118">Properties</span></span>
| <span data-ttu-id="de264-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de264-119">Property</span></span>     | <span data-ttu-id="de264-120">型</span><span class="sxs-lookup"><span data-stu-id="de264-120">Type</span></span>   |<span data-ttu-id="de264-121">説明</span><span class="sxs-lookup"><span data-stu-id="de264-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de264-122">cellAddresses</span><span class="sxs-lookup"><span data-stu-id="de264-122">cellAddresses</span></span>|<span data-ttu-id="de264-123">Json</span><span class="sxs-lookup"><span data-stu-id="de264-123">Json</span></span>|<span data-ttu-id="de264-124">セルのアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="de264-124">Represents the cell addresses</span></span>
|<span data-ttu-id="de264-125">columnCount</span><span class="sxs-lookup"><span data-stu-id="de264-125">columnCount</span></span>|<span data-ttu-id="de264-126">Int32</span><span class="sxs-lookup"><span data-stu-id="de264-126">Int32</span></span>|<span data-ttu-id="de264-p101">表示されている列の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="de264-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="de264-129">formulas</span><span class="sxs-lookup"><span data-stu-id="de264-129">formulas</span></span>|<span data-ttu-id="de264-130">Json</span><span class="sxs-lookup"><span data-stu-id="de264-130">Json</span></span>|<span data-ttu-id="de264-131">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="de264-131">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="de264-132">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="de264-132">formulasLocal</span></span>|<span data-ttu-id="de264-133">Json</span><span class="sxs-lookup"><span data-stu-id="de264-133">Json</span></span>|<span data-ttu-id="de264-p102">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="de264-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="de264-136">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="de264-136">formulasR1C1</span></span>|<span data-ttu-id="de264-137">Json</span><span class="sxs-lookup"><span data-stu-id="de264-137">Json</span></span>|<span data-ttu-id="de264-138">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="de264-138">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="de264-139">index</span><span class="sxs-lookup"><span data-stu-id="de264-139">index</span></span>|<span data-ttu-id="de264-140">Int32</span><span class="sxs-lookup"><span data-stu-id="de264-140">Int32</span></span>|<span data-ttu-id="de264-141">範囲のインデックス。</span><span class="sxs-lookup"><span data-stu-id="de264-141">Index of the range.</span></span>|
|<span data-ttu-id="de264-142">numberFormat</span><span class="sxs-lookup"><span data-stu-id="de264-142">numberFormat</span></span>|<span data-ttu-id="de264-143">Json</span><span class="sxs-lookup"><span data-stu-id="de264-143">Json</span></span>|<span data-ttu-id="de264-p103">指定したセルの Excel の数値書式コードを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="de264-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="de264-146">rowCount</span><span class="sxs-lookup"><span data-stu-id="de264-146">rowCount</span></span>|<span data-ttu-id="de264-147">Int32</span><span class="sxs-lookup"><span data-stu-id="de264-147">Int32</span></span>|<span data-ttu-id="de264-p104">表示されている行の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="de264-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="de264-150">text</span><span class="sxs-lookup"><span data-stu-id="de264-150">text</span></span>|<span data-ttu-id="de264-151">Json</span><span class="sxs-lookup"><span data-stu-id="de264-151">Json</span></span>|<span data-ttu-id="de264-p105">指定した範囲のテキスト値。テキスト値は、セルの幅には依存しません。Excel UI で発生する # 記号による置換は、この API から返されるテキスト値には影響しません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="de264-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="de264-156">valueTypes</span><span class="sxs-lookup"><span data-stu-id="de264-156">valueTypes</span></span>|<span data-ttu-id="de264-157">Json</span><span class="sxs-lookup"><span data-stu-id="de264-157">Json</span></span>|<span data-ttu-id="de264-158">各セルのデータの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="de264-158">Represents the type of data of each cell.</span></span> <span data-ttu-id="de264-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="de264-159">Read-only.</span></span> <span data-ttu-id="de264-160">値を指定できます: 不明な空白、文字列、整数、ブール値、エラーでは 2 倍、です。</span><span class="sxs-lookup"><span data-stu-id="de264-160">The possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="de264-161">values</span><span class="sxs-lookup"><span data-stu-id="de264-161">values</span></span>|<span data-ttu-id="de264-162">Json</span><span class="sxs-lookup"><span data-stu-id="de264-162">Json</span></span>|<span data-ttu-id="de264-p107">指定した範囲ビューの Raw 値を表します。返されるデータの型は、文字列、数値、ブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="de264-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="de264-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de264-166">Relationships</span></span>
| <span data-ttu-id="de264-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de264-167">Relationship</span></span> | <span data-ttu-id="de264-168">型</span><span class="sxs-lookup"><span data-stu-id="de264-168">Type</span></span>   |<span data-ttu-id="de264-169">説明</span><span class="sxs-lookup"><span data-stu-id="de264-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de264-170">rows</span><span class="sxs-lookup"><span data-stu-id="de264-170">rows</span></span>|<span data-ttu-id="de264-171">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="de264-171">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="de264-p108">範囲に関連付けられている範囲ビューのコレクションを表します。読み取り専用です。  読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="de264-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de264-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de264-175">JSON representation</span></span>
<span data-ttu-id="de264-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de264-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
