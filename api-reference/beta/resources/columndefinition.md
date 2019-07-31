---
author: JeremyKelley
description: 以下は、columnDefinition リソースの JSON 表記です。
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7f60d33f8fbfe76c9dfd0ca02c98df96ca6ab380
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973301"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="b16dd-103">columnDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b16dd-103">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="b16dd-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b16dd-104">JSON representation</span></span>

<span data-ttu-id="b16dd-105">以下は、columnDefinition リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b16dd-105">Here is a JSON representation of a columnDefinition resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": "true",
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="b16dd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b16dd-106">Properties</span></span>

<span data-ttu-id="b16dd-107">列には、さまざまな種類のデータを保持できます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-107">Columns can hold data of various types.</span></span>
<span data-ttu-id="b16dd-108">次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="b16dd-108">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="b16dd-109">型に関連するプロパティ (boolean、演算、choice、currency、dateTime、lookup、number、個人、グループ、テキスト) は相互に排他的です。1つの列に指定できるのは1つだけです。</span><span class="sxs-lookup"><span data-stu-id="b16dd-109">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="b16dd-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b16dd-110">Property name</span></span>           | <span data-ttu-id="b16dd-111">種類</span><span class="sxs-lookup"><span data-stu-id="b16dd-111">Type</span></span>    | <span data-ttu-id="b16dd-112">説明</span><span class="sxs-lookup"><span data-stu-id="b16dd-112">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="b16dd-113">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="b16dd-113">**columnGroup**</span></span>         | <span data-ttu-id="b16dd-114">string</span><span class="sxs-lookup"><span data-stu-id="b16dd-114">string</span></span>  | <span data-ttu-id="b16dd-115">サイト列の場合、この列が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="b16dd-115">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="b16dd-116">関連する列を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-116">Helps organize related columns.</span></span>
| <span data-ttu-id="b16dd-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b16dd-117">**description**</span></span>         | <span data-ttu-id="b16dd-118">string</span><span class="sxs-lookup"><span data-stu-id="b16dd-118">string</span></span>  | <span data-ttu-id="b16dd-119">列に関するユーザー向けの説明。</span><span class="sxs-lookup"><span data-stu-id="b16dd-119">The user-facing description of the column.</span></span>
| <span data-ttu-id="b16dd-120">**displayName**</span><span class="sxs-lookup"><span data-stu-id="b16dd-120">**displayName**</span></span>         | <span data-ttu-id="b16dd-121">string</span><span class="sxs-lookup"><span data-stu-id="b16dd-121">string</span></span>  | <span data-ttu-id="b16dd-122">列を示すユーザー向けの名前。</span><span class="sxs-lookup"><span data-stu-id="b16dd-122">The user-facing name of the column.</span></span>
| <span data-ttu-id="b16dd-123">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="b16dd-123">**enforceUniqueValues**</span></span> | <span data-ttu-id="b16dd-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="b16dd-124">boolean</span></span> | <span data-ttu-id="b16dd-125">True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b16dd-125">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="b16dd-126">**hidden**</span><span class="sxs-lookup"><span data-stu-id="b16dd-126">**hidden**</span></span>              | <span data-ttu-id="b16dd-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="b16dd-127">boolean</span></span> | <span data-ttu-id="b16dd-128">この列がユーザー インターフェイスに表示されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b16dd-128">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="b16dd-129">**id**</span><span class="sxs-lookup"><span data-stu-id="b16dd-129">**id**</span></span>                  | <span data-ttu-id="b16dd-130">string</span><span class="sxs-lookup"><span data-stu-id="b16dd-130">string</span></span>  | <span data-ttu-id="b16dd-131">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b16dd-131">The unique identifier for the column.</span></span>
| <span data-ttu-id="b16dd-132">**indexed**</span><span class="sxs-lookup"><span data-stu-id="b16dd-132">**indexed**</span></span>             | <span data-ttu-id="b16dd-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="b16dd-133">boolean</span></span> | <span data-ttu-id="b16dd-134">列の値を、並べ替えと検索に使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b16dd-134">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="b16dd-135">**name**</span><span class="sxs-lookup"><span data-stu-id="b16dd-135">**name**</span></span>                | <span data-ttu-id="b16dd-136">string</span><span class="sxs-lookup"><span data-stu-id="b16dd-136">string</span></span>  | <span data-ttu-id="b16dd-137">[listItem][] の [fields][] に表示される、列を示す API 向けの名前。</span><span class="sxs-lookup"><span data-stu-id="b16dd-137">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="b16dd-138">ユーザー向けの名前については **displayName** をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b16dd-138">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="b16dd-139">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="b16dd-139">**readOnly**</span></span>            | <span data-ttu-id="b16dd-140">bool</span><span class="sxs-lookup"><span data-stu-id="b16dd-140">bool</span></span>    | <span data-ttu-id="b16dd-141">列の値を変更できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b16dd-141">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="b16dd-142">**required**</span><span class="sxs-lookup"><span data-stu-id="b16dd-142">**required**</span></span>            | <span data-ttu-id="b16dd-143">boolean</span><span class="sxs-lookup"><span data-stu-id="b16dd-143">boolean</span></span> | <span data-ttu-id="b16dd-144">列の値が省略不可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b16dd-144">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="b16dd-145">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b16dd-145">**boolean**</span></span>       | <span data-ttu-id="b16dd-146">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-146">[booleanColumn][]</span></span>       | <span data-ttu-id="b16dd-147">この列にはブール値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-147">This column stores boolean values.</span></span>
| <span data-ttu-id="b16dd-148">**calculated**</span><span class="sxs-lookup"><span data-stu-id="b16dd-148">**calculated**</span></span>    | <span data-ttu-id="b16dd-149">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-149">[calculatedColumn][]</span></span>    | <span data-ttu-id="b16dd-150">この列のデータは、他の列に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-150">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="b16dd-151">**choice**</span><span class="sxs-lookup"><span data-stu-id="b16dd-151">**choice**</span></span>        | <span data-ttu-id="b16dd-152">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-152">[choiceColumn][]</span></span>        | <span data-ttu-id="b16dd-153">この列には、選択肢リストからのデータが格納されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-153">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="b16dd-154">**currency**</span><span class="sxs-lookup"><span data-stu-id="b16dd-154">**currency**</span></span>      | <span data-ttu-id="b16dd-155">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-155">[currencyColumn][]</span></span>      | <span data-ttu-id="b16dd-156">この列には通貨値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-156">This column stores currency values.</span></span>
| <span data-ttu-id="b16dd-157">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b16dd-157">**dateTime**</span></span>      | <span data-ttu-id="b16dd-158">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-158">[dateTimeColumn][]</span></span>      | <span data-ttu-id="b16dd-159">この列には日時の値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-159">This column stores DateTime values.</span></span>
| <span data-ttu-id="b16dd-160">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="b16dd-160">**defaultValue**</span></span>  | <span data-ttu-id="b16dd-161">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-161">[defaultColumnValue][]</span></span>  | <span data-ttu-id="b16dd-162">この列の既定値です。</span><span class="sxs-lookup"><span data-stu-id="b16dd-162">The default value for this column.</span></span>
| <span data-ttu-id="b16dd-163">**地理位置情報**</span><span class="sxs-lookup"><span data-stu-id="b16dd-163">**geolocation**</span></span>   | <span data-ttu-id="b16dd-164">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-164">[geolocationColumn][]</span></span>   | <span data-ttu-id="b16dd-165">この列には、地理位置情報が格納されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-165">This column stores a geolocation.</span></span>
| <span data-ttu-id="b16dd-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="b16dd-166">**lookup**</span></span>        | <span data-ttu-id="b16dd-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-167">[lookupColumn][]</span></span>        | <span data-ttu-id="b16dd-168">この列のデータは、サイト内の別のソースから検索されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="b16dd-169">**number**</span><span class="sxs-lookup"><span data-stu-id="b16dd-169">**number**</span></span>        | <span data-ttu-id="b16dd-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-170">[numberColumn][]</span></span>        | <span data-ttu-id="b16dd-171">この列には数値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-171">This column stores number values.</span></span>
| <span data-ttu-id="b16dd-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="b16dd-172">**personOrGroup**</span></span> | <span data-ttu-id="b16dd-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="b16dd-174">この列にはユーザーまたはグループの値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="b16dd-175">**text**</span><span class="sxs-lookup"><span data-stu-id="b16dd-175">**text**</span></span>          | <span data-ttu-id="b16dd-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="b16dd-176">[textColumn][]</span></span>          | <span data-ttu-id="b16dd-177">この列にはテキスト値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-177">This column stores text values.</span></span>

><span data-ttu-id="b16dd-178">**注:** これらのプロパティは、SharePoint の[SPFieldType][]列挙に対応しています。</span><span class="sxs-lookup"><span data-stu-id="b16dd-178">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="b16dd-179">最も一般的なフィールドの種類は上記の表で表されていますが、このベータ版 API にはまだ不足しています。</span><span class="sxs-lookup"><span data-stu-id="b16dd-179">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="b16dd-180">そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="b16dd-181">備考</span><span class="sxs-lookup"><span data-stu-id="b16dd-181">Remarks</span></span>

<span data-ttu-id="b16dd-182">`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。</span><span class="sxs-lookup"><span data-stu-id="b16dd-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="b16dd-183">**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="b16dd-184">[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。</span><span class="sxs-lookup"><span data-stu-id="b16dd-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->
