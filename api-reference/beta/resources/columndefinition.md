---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 9b99abe78b009786d489ec7f0c0fdce1e2945b1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066611"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="3665c-102">columnDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3665c-102">columnDefinition resource type</span></span>

> <span data-ttu-id="3665c-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3665c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3665c-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3665c-104">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3665c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3665c-105">JSON representation</span></span>

<span data-ttu-id="3665c-106">ColumnDefinition リソースの JSON 表現は、ここで。</span><span class="sxs-lookup"><span data-stu-id="3665c-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3665c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3665c-107">Properties</span></span>

<span data-ttu-id="3665c-108">列には、さまざまな種類のデータを保持できます。</span><span class="sxs-lookup"><span data-stu-id="3665c-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="3665c-109">次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="3665c-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="3665c-110">タイプに関連するプロパティ (ブール値、計算された、選択、通貨、日時、検索、番号、personOrGroup、テキスト) は相互に排他的な--列のみが指定されているそれらの 1 つです。</span><span class="sxs-lookup"><span data-stu-id="3665c-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="3665c-111">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="3665c-111">Property name</span></span>           | <span data-ttu-id="3665c-112">型</span><span class="sxs-lookup"><span data-stu-id="3665c-112">Type</span></span>    | <span data-ttu-id="3665c-113">説明</span><span class="sxs-lookup"><span data-stu-id="3665c-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="3665c-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="3665c-114">**columnGroup**</span></span>         | <span data-ttu-id="3665c-115">文字列</span><span class="sxs-lookup"><span data-stu-id="3665c-115">string</span></span>  | <span data-ttu-id="3665c-116">サイト列の場合、この列が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="3665c-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="3665c-117">関連する列を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="3665c-117">Helps organize related columns.</span></span>
| <span data-ttu-id="3665c-118">**description**</span><span class="sxs-lookup"><span data-stu-id="3665c-118">**description**</span></span>         | <span data-ttu-id="3665c-119">文字列</span><span class="sxs-lookup"><span data-stu-id="3665c-119">string</span></span>  | <span data-ttu-id="3665c-120">列に関するユーザー向けの説明。</span><span class="sxs-lookup"><span data-stu-id="3665c-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="3665c-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="3665c-121">**displayName**</span></span>         | <span data-ttu-id="3665c-122">文字列</span><span class="sxs-lookup"><span data-stu-id="3665c-122">string</span></span>  | <span data-ttu-id="3665c-123">列を示すユーザー向けの名前。</span><span class="sxs-lookup"><span data-stu-id="3665c-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="3665c-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="3665c-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="3665c-125">boolean</span><span class="sxs-lookup"><span data-stu-id="3665c-125">boolean</span></span> | <span data-ttu-id="3665c-126">True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="3665c-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="3665c-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="3665c-127">**hidden**</span></span>              | <span data-ttu-id="3665c-128">boolean</span><span class="sxs-lookup"><span data-stu-id="3665c-128">boolean</span></span> | <span data-ttu-id="3665c-129">この列がユーザー インターフェイスに表示されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3665c-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="3665c-130">**id**</span><span class="sxs-lookup"><span data-stu-id="3665c-130">**id**</span></span>                  | <span data-ttu-id="3665c-131">string</span><span class="sxs-lookup"><span data-stu-id="3665c-131">string</span></span>  | <span data-ttu-id="3665c-132">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3665c-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="3665c-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="3665c-133">**indexed**</span></span>             | <span data-ttu-id="3665c-134">boolean</span><span class="sxs-lookup"><span data-stu-id="3665c-134">boolean</span></span> | <span data-ttu-id="3665c-135">列の値を、並べ替えと検索に使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3665c-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="3665c-136">**name**</span><span class="sxs-lookup"><span data-stu-id="3665c-136">**name**</span></span>                | <span data-ttu-id="3665c-137">文字列</span><span class="sxs-lookup"><span data-stu-id="3665c-137">string</span></span>  | <span data-ttu-id="3665c-138">[listItem][] の [fields][] に表示される、列を示す API 向けの名前。</span><span class="sxs-lookup"><span data-stu-id="3665c-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="3665c-139">ユーザー向けの名前については **displayName** をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3665c-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="3665c-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="3665c-140">**readOnly**</span></span>            | <span data-ttu-id="3665c-141">bool</span><span class="sxs-lookup"><span data-stu-id="3665c-141">bool</span></span>    | <span data-ttu-id="3665c-142">列の値を変更できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3665c-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="3665c-143">**required**</span><span class="sxs-lookup"><span data-stu-id="3665c-143">**required**</span></span>            | <span data-ttu-id="3665c-144">boolean</span><span class="sxs-lookup"><span data-stu-id="3665c-144">boolean</span></span> | <span data-ttu-id="3665c-145">列の値が省略不可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3665c-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="3665c-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="3665c-146">**boolean**</span></span>       | <span data-ttu-id="3665c-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-147">[booleanColumn][]</span></span>       | <span data-ttu-id="3665c-148">この列にはブール値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-148">This column stores boolean values.</span></span>
| <span data-ttu-id="3665c-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="3665c-149">**calculated**</span></span>    | <span data-ttu-id="3665c-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="3665c-151">この列のデータは、他の列に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="3665c-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="3665c-152">**choice**</span></span>        | <span data-ttu-id="3665c-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-153">[choiceColumn][]</span></span>        | <span data-ttu-id="3665c-154">この列には、選択肢リストからのデータが格納されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="3665c-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="3665c-155">**currency**</span></span>      | <span data-ttu-id="3665c-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-156">[currencyColumn][]</span></span>      | <span data-ttu-id="3665c-157">この列には通貨値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-157">This column stores currency values.</span></span>
| <span data-ttu-id="3665c-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="3665c-158">**dateTime**</span></span>      | <span data-ttu-id="3665c-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="3665c-160">この列には日時の値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="3665c-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="3665c-161">**defaultValue**</span></span>  | <span data-ttu-id="3665c-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="3665c-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="3665c-163">この列の既定値です。</span><span class="sxs-lookup"><span data-stu-id="3665c-163">The default value for this column.</span></span>
| <span data-ttu-id="3665c-164">**地理位置情報**</span><span class="sxs-lookup"><span data-stu-id="3665c-164">**geolocation**</span></span>   | <span data-ttu-id="3665c-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="3665c-166">この列は、地理位置情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="3665c-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="3665c-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="3665c-167">**lookup**</span></span>        | <span data-ttu-id="3665c-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-168">[lookupColumn][]</span></span>        | <span data-ttu-id="3665c-169">この列のデータは、サイト内の別のソースから検索されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="3665c-170">**number**</span><span class="sxs-lookup"><span data-stu-id="3665c-170">**number**</span></span>        | <span data-ttu-id="3665c-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-171">[numberColumn][]</span></span>        | <span data-ttu-id="3665c-172">この列には数値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-172">This column stores number values.</span></span>
| <span data-ttu-id="3665c-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="3665c-173">**personOrGroup**</span></span> | <span data-ttu-id="3665c-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="3665c-175">この列にはユーザーまたはグループの値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="3665c-176">**text**</span><span class="sxs-lookup"><span data-stu-id="3665c-176">**text**</span></span>          | <span data-ttu-id="3665c-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="3665c-177">[textColumn][]</span></span>          | <span data-ttu-id="3665c-178">この列にはテキスト値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="3665c-178">This column stores text values.</span></span>

><span data-ttu-id="3665c-179">**注:** これらのプロパティは、SharePoint の[SPFieldType][]の列挙体に対応しています。</span><span class="sxs-lookup"><span data-stu-id="3665c-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="3665c-180">最も一般的なフィールドの種類は上記の表に表示されるときにこのベータ版の API がまだないです。</span><span class="sxs-lookup"><span data-stu-id="3665c-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="3665c-181">そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。</span><span class="sxs-lookup"><span data-stu-id="3665c-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="3665c-182">備考</span><span class="sxs-lookup"><span data-stu-id="3665c-182">Remarks</span></span>

<span data-ttu-id="3665c-183">`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。</span><span class="sxs-lookup"><span data-stu-id="3665c-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="3665c-184">**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。</span><span class="sxs-lookup"><span data-stu-id="3665c-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="3665c-185">[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。</span><span class="sxs-lookup"><span data-stu-id="3665c-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
