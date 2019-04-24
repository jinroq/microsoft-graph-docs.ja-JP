---
title: rangeView リソースの種類
description: RangeView は、親の範囲の表示されているセルのセットを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ace424d12e38e4bb907923ea542ebd7330130d06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453508"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="ecb3b-103">rangeView リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecb3b-103">rangeView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecb3b-104">RangeView は、親の範囲の表示されているセルのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="ecb3b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ecb3b-105">Methods</span></span>

| <span data-ttu-id="ecb3b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ecb3b-106">Method</span></span>           | <span data-ttu-id="ecb3b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ecb3b-107">Return Type</span></span>    |<span data-ttu-id="ecb3b-108">説明</span><span class="sxs-lookup"><span data-stu-id="ecb3b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ecb3b-109">行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ecb3b-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="ecb3b-110">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ecb3b-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="ecb3b-111">workbookRangeView オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="ecb3b-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="ecb3b-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="ecb3b-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="ecb3b-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="ecb3b-114">インデックスに基づいて範囲ビューの項目を取得します。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="ecb3b-115">Range</span><span class="sxs-lookup"><span data-stu-id="ecb3b-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="ecb3b-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="ecb3b-116">workbookRange</span></span>](range.md)|<span data-ttu-id="ecb3b-117">範囲ビューに関連付けられた範囲オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="ecb3b-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecb3b-118">Properties</span></span>
| <span data-ttu-id="ecb3b-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecb3b-119">Property</span></span>     | <span data-ttu-id="ecb3b-120">型</span><span class="sxs-lookup"><span data-stu-id="ecb3b-120">Type</span></span>   |<span data-ttu-id="ecb3b-121">説明</span><span class="sxs-lookup"><span data-stu-id="ecb3b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb3b-122">columnCount</span><span class="sxs-lookup"><span data-stu-id="ecb3b-122">columnCount</span></span>|<span data-ttu-id="ecb3b-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ecb3b-123">Int32</span></span>|<span data-ttu-id="ecb3b-p101">表示されている列の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="ecb3b-126">formulas</span><span class="sxs-lookup"><span data-stu-id="ecb3b-126">formulas</span></span>|<span data-ttu-id="ecb3b-127">Json</span><span class="sxs-lookup"><span data-stu-id="ecb3b-127">Json</span></span>|<span data-ttu-id="ecb3b-128">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-128">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="ecb3b-129">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="ecb3b-129">formulasLocal</span></span>|<span data-ttu-id="ecb3b-130">Json</span><span class="sxs-lookup"><span data-stu-id="ecb3b-130">Json</span></span>|<span data-ttu-id="ecb3b-p102">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="ecb3b-133">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="ecb3b-133">formulasR1C1</span></span>|<span data-ttu-id="ecb3b-134">Json</span><span class="sxs-lookup"><span data-stu-id="ecb3b-134">Json</span></span>|<span data-ttu-id="ecb3b-135">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-135">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="ecb3b-136">index</span><span class="sxs-lookup"><span data-stu-id="ecb3b-136">index</span></span>|<span data-ttu-id="ecb3b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ecb3b-137">Int32</span></span>|<span data-ttu-id="ecb3b-138">範囲のインデックス。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-138">Index of the range.</span></span>|
|<span data-ttu-id="ecb3b-139">numberFormat</span><span class="sxs-lookup"><span data-stu-id="ecb3b-139">numberFormat</span></span>|<span data-ttu-id="ecb3b-140">Json</span><span class="sxs-lookup"><span data-stu-id="ecb3b-140">Json</span></span>|<span data-ttu-id="ecb3b-p103">指定したセルの Excel の数値書式コードを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="ecb3b-143">rowCount</span><span class="sxs-lookup"><span data-stu-id="ecb3b-143">rowCount</span></span>|<span data-ttu-id="ecb3b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ecb3b-144">Int32</span></span>|<span data-ttu-id="ecb3b-p104">表示されている行の数を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="ecb3b-147">text</span><span class="sxs-lookup"><span data-stu-id="ecb3b-147">text</span></span>|<span data-ttu-id="ecb3b-148">Json</span><span class="sxs-lookup"><span data-stu-id="ecb3b-148">Json</span></span>|<span data-ttu-id="ecb3b-p105">指定した範囲のテキスト値。テキスト値は、セルの幅には依存しません。Excel UI で発生する # 記号による置換は、この API から返されるテキスト値には影響しません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="ecb3b-153">valueTypes</span><span class="sxs-lookup"><span data-stu-id="ecb3b-153">valueTypes</span></span>|<span data-ttu-id="ecb3b-154">Json</span><span class="sxs-lookup"><span data-stu-id="ecb3b-154">Json</span></span>|<span data-ttu-id="ecb3b-p106">各セルのデータの種類を表します。読み取り専用です。使用可能な値は次のとおりです。Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="ecb3b-158">values</span><span class="sxs-lookup"><span data-stu-id="ecb3b-158">values</span></span>|<span data-ttu-id="ecb3b-159">Json</span><span class="sxs-lookup"><span data-stu-id="ecb3b-159">Json</span></span>|<span data-ttu-id="ecb3b-p107">指定した範囲ビューの Raw 値を表します。返されるデータの型は、文字列、数値、ブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="ecb3b-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ecb3b-163">Relationships</span></span>
| <span data-ttu-id="ecb3b-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ecb3b-164">Relationship</span></span> | <span data-ttu-id="ecb3b-165">型</span><span class="sxs-lookup"><span data-stu-id="ecb3b-165">Type</span></span>   |<span data-ttu-id="ecb3b-166">説明</span><span class="sxs-lookup"><span data-stu-id="ecb3b-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb3b-167">rows</span><span class="sxs-lookup"><span data-stu-id="ecb3b-167">rows</span></span>|<span data-ttu-id="ecb3b-168">[workbookRangeView](workbookrangeview.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ecb3b-168">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="ecb3b-p108">範囲に関連付けられている範囲ビューのコレクションを表します。読み取り専用です。  読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ecb3b-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecb3b-172">JSON representation</span></span>
<span data-ttu-id="ecb3b-173">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ecb3b-173">Here is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookrangeview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
