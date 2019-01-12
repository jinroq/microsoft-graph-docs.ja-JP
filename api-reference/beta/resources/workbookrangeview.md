---
title: rangeView リソースの種類
description: RangeView は、親の範囲の表示されているセルのセットを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9476b3f4a085f70be51d81a9da667c07db3b9232
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983717"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="a32b3-103">rangeView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a32b3-103">rangeView resource type</span></span>

> <span data-ttu-id="a32b3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a32b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a32b3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a32b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a32b3-106">RangeView は、親の範囲の表示されているセルのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="a32b3-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="a32b3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a32b3-107">Methods</span></span>

| <span data-ttu-id="a32b3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a32b3-108">Method</span></span>           | <span data-ttu-id="a32b3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a32b3-109">Return Type</span></span>    |<span data-ttu-id="a32b3-110">説明</span><span class="sxs-lookup"><span data-stu-id="a32b3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a32b3-111">行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a32b3-111">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="a32b3-112">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a32b3-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="a32b3-113">workbookRangeView オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a32b3-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="a32b3-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="a32b3-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="a32b3-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="a32b3-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="a32b3-116">インデックスに基づいて範囲ビューの項目を取得します。</span><span class="sxs-lookup"><span data-stu-id="a32b3-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="a32b3-117">Range</span><span class="sxs-lookup"><span data-stu-id="a32b3-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="a32b3-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="a32b3-118">workbookRange</span></span>](range.md)|<span data-ttu-id="a32b3-119">範囲ビューに関連付けられた範囲オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a32b3-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="a32b3-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a32b3-120">Properties</span></span>
| <span data-ttu-id="a32b3-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a32b3-121">Property</span></span>     | <span data-ttu-id="a32b3-122">種類</span><span class="sxs-lookup"><span data-stu-id="a32b3-122">Type</span></span>   |<span data-ttu-id="a32b3-123">説明</span><span class="sxs-lookup"><span data-stu-id="a32b3-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a32b3-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="a32b3-124">columnCount</span></span>|<span data-ttu-id="a32b3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a32b3-125">Int32</span></span>|<span data-ttu-id="a32b3-p102">表示されている列の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a32b3-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="a32b3-128">formulas</span><span class="sxs-lookup"><span data-stu-id="a32b3-128">formulas</span></span>|<span data-ttu-id="a32b3-129">Json</span><span class="sxs-lookup"><span data-stu-id="a32b3-129">Json</span></span>|<span data-ttu-id="a32b3-130">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="a32b3-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="a32b3-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="a32b3-131">formulasLocal</span></span>|<span data-ttu-id="a32b3-132">Json</span><span class="sxs-lookup"><span data-stu-id="a32b3-132">Json</span></span>|<span data-ttu-id="a32b3-p103">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="a32b3-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="a32b3-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="a32b3-135">formulasR1C1</span></span>|<span data-ttu-id="a32b3-136">Json</span><span class="sxs-lookup"><span data-stu-id="a32b3-136">Json</span></span>|<span data-ttu-id="a32b3-137">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="a32b3-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="a32b3-138">index</span><span class="sxs-lookup"><span data-stu-id="a32b3-138">index</span></span>|<span data-ttu-id="a32b3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a32b3-139">Int32</span></span>|<span data-ttu-id="a32b3-140">範囲のインデックス。</span><span class="sxs-lookup"><span data-stu-id="a32b3-140">Index of the range.</span></span>|
|<span data-ttu-id="a32b3-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="a32b3-141">numberFormat</span></span>|<span data-ttu-id="a32b3-142">Json</span><span class="sxs-lookup"><span data-stu-id="a32b3-142">Json</span></span>|<span data-ttu-id="a32b3-p104">指定したセルの Excel の数値書式コードを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a32b3-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="a32b3-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="a32b3-145">rowCount</span></span>|<span data-ttu-id="a32b3-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a32b3-146">Int32</span></span>|<span data-ttu-id="a32b3-p105">表示されている行の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a32b3-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="a32b3-149">text</span><span class="sxs-lookup"><span data-stu-id="a32b3-149">text</span></span>|<span data-ttu-id="a32b3-150">Json</span><span class="sxs-lookup"><span data-stu-id="a32b3-150">Json</span></span>|<span data-ttu-id="a32b3-p106">指定した範囲のテキスト値。テキスト値は、セルの幅には依存しません。Excel UI で発生する # 記号による置換は、この API から返されるテキスト値には影響しません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a32b3-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="a32b3-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="a32b3-155">valueTypes</span></span>|<span data-ttu-id="a32b3-156">Json</span><span class="sxs-lookup"><span data-stu-id="a32b3-156">Json</span></span>|<span data-ttu-id="a32b3-p107">各セルのデータの種類を表します。読み取り専用です。使用可能な値は次のとおりです。Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="a32b3-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="a32b3-160">values</span><span class="sxs-lookup"><span data-stu-id="a32b3-160">values</span></span>|<span data-ttu-id="a32b3-161">Json</span><span class="sxs-lookup"><span data-stu-id="a32b3-161">Json</span></span>|<span data-ttu-id="a32b3-p108">指定した範囲ビューの Raw 値を表します。返されるデータの型は、文字列、数値、ブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="a32b3-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="a32b3-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a32b3-165">Relationships</span></span>
| <span data-ttu-id="a32b3-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a32b3-166">Relationship</span></span> | <span data-ttu-id="a32b3-167">型</span><span class="sxs-lookup"><span data-stu-id="a32b3-167">Type</span></span>   |<span data-ttu-id="a32b3-168">説明</span><span class="sxs-lookup"><span data-stu-id="a32b3-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a32b3-169">rows</span><span class="sxs-lookup"><span data-stu-id="a32b3-169">rows</span></span>|<span data-ttu-id="a32b3-170">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a32b3-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="a32b3-p109">範囲に関連付けられている範囲ビューのコレクションを表します。読み取り専用です。  読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a32b3-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a32b3-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a32b3-174">JSON representation</span></span>
<span data-ttu-id="a32b3-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a32b3-175">Here is a JSON representation of the resource.</span></span>
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
