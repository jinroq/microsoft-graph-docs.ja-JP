---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: 598a781c25dd9271be84eb3dfc16b1e5ff439298
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862882"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="0cd2e-102">ColumnDefinition リソース</span><span class="sxs-lookup"><span data-stu-id="0cd2e-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cd2e-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cd2e-103">JSON representation</span></span>

<span data-ttu-id="0cd2e-104">以下は、ColumnDefinition リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="0cd2e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cd2e-105">Properties</span></span>

<span data-ttu-id="0cd2e-106">**columnDefinition** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="0cd2e-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0cd2e-107">Property name</span></span>           | <span data-ttu-id="0cd2e-108">種類</span><span class="sxs-lookup"><span data-stu-id="0cd2e-108">Type</span></span>    | <span data-ttu-id="0cd2e-109">説明</span><span class="sxs-lookup"><span data-stu-id="0cd2e-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="0cd2e-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-110">**columnGroup**</span></span>         | <span data-ttu-id="0cd2e-111">string</span><span class="sxs-lookup"><span data-stu-id="0cd2e-111">string</span></span>  | <span data-ttu-id="0cd2e-112">サイト列の場合、この列が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="0cd2e-113">関連する列を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-113">Helps organize related columns.</span></span>
| <span data-ttu-id="0cd2e-114">**description**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-114">**description**</span></span>         | <span data-ttu-id="0cd2e-115">string</span><span class="sxs-lookup"><span data-stu-id="0cd2e-115">string</span></span>  | <span data-ttu-id="0cd2e-116">列に関するユーザー向けの説明。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="0cd2e-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-117">**displayName**</span></span>         | <span data-ttu-id="0cd2e-118">string</span><span class="sxs-lookup"><span data-stu-id="0cd2e-118">string</span></span>  | <span data-ttu-id="0cd2e-119">列を示すユーザー向けの名前。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="0cd2e-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="0cd2e-121">boolean</span><span class="sxs-lookup"><span data-stu-id="0cd2e-121">boolean</span></span> | <span data-ttu-id="0cd2e-122">True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="0cd2e-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-123">**hidden**</span></span>              | <span data-ttu-id="0cd2e-124">boolean</span><span class="sxs-lookup"><span data-stu-id="0cd2e-124">boolean</span></span> | <span data-ttu-id="0cd2e-125">この列がユーザー インターフェイスに表示されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="0cd2e-126">**id**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-126">**id**</span></span>                  | <span data-ttu-id="0cd2e-127">string</span><span class="sxs-lookup"><span data-stu-id="0cd2e-127">string</span></span>  | <span data-ttu-id="0cd2e-128">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="0cd2e-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-129">**indexed**</span></span>             | <span data-ttu-id="0cd2e-130">boolean</span><span class="sxs-lookup"><span data-stu-id="0cd2e-130">boolean</span></span> | <span data-ttu-id="0cd2e-131">列の値を、並べ替えと検索に使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="0cd2e-132">**name**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-132">**name**</span></span>                | <span data-ttu-id="0cd2e-133">string</span><span class="sxs-lookup"><span data-stu-id="0cd2e-133">string</span></span>  | <span data-ttu-id="0cd2e-134">[listItem][] の [fields][] に表示される、列を示す API 向けの名前。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="0cd2e-135">ユーザー向けの名前については **displayName** をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="0cd2e-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-136">**readOnly**</span></span>            | <span data-ttu-id="0cd2e-137">bool</span><span class="sxs-lookup"><span data-stu-id="0cd2e-137">bool</span></span>    | <span data-ttu-id="0cd2e-138">列の値を変更できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="0cd2e-139">**required**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-139">**required**</span></span>            | <span data-ttu-id="0cd2e-140">boolean</span><span class="sxs-lookup"><span data-stu-id="0cd2e-140">boolean</span></span> | <span data-ttu-id="0cd2e-141">列の値が省略不可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="0cd2e-142">列には、さまざまな種類のデータを保持できます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="0cd2e-143">次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="0cd2e-144">これらのプロパティは相互に排他的で、各列でいずれか 1 つだけを指定できます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="0cd2e-145">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0cd2e-145">Property name</span></span>     | <span data-ttu-id="0cd2e-146">種類</span><span class="sxs-lookup"><span data-stu-id="0cd2e-146">Type</span></span>                    | <span data-ttu-id="0cd2e-147">説明</span><span class="sxs-lookup"><span data-stu-id="0cd2e-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="0cd2e-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-148">**boolean**</span></span>       | <span data-ttu-id="0cd2e-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-149">[booleanColumn][]</span></span>       | <span data-ttu-id="0cd2e-150">この列にはブール値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-150">This column stores boolean values.</span></span>
| <span data-ttu-id="0cd2e-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-151">**calculated**</span></span>    | <span data-ttu-id="0cd2e-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="0cd2e-153">この列のデータは、他の列に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="0cd2e-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-154">**choice**</span></span>        | <span data-ttu-id="0cd2e-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-155">[choiceColumn][]</span></span>        | <span data-ttu-id="0cd2e-156">この列には、選択肢リストからのデータが格納されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="0cd2e-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-157">**currency**</span></span>      | <span data-ttu-id="0cd2e-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-158">[currencyColumn][]</span></span>      | <span data-ttu-id="0cd2e-159">この列には通貨値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-159">This column stores currency values.</span></span>
| <span data-ttu-id="0cd2e-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-160">**dateTime**</span></span>      | <span data-ttu-id="0cd2e-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="0cd2e-162">この列には日時の値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="0cd2e-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-163">**defaultValue**</span></span>  | <span data-ttu-id="0cd2e-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="0cd2e-165">この列の既定値です。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-165">The default value for this column.</span></span>
| <span data-ttu-id="0cd2e-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-166">**lookup**</span></span>        | <span data-ttu-id="0cd2e-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-167">[lookupColumn][]</span></span>        | <span data-ttu-id="0cd2e-168">この列のデータは、サイト内の別のソースから検索されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="0cd2e-169">**number**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-169">**number**</span></span>        | <span data-ttu-id="0cd2e-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-170">[numberColumn][]</span></span>        | <span data-ttu-id="0cd2e-171">この列には数値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-171">This column stores number values.</span></span>
| <span data-ttu-id="0cd2e-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-172">**personOrGroup**</span></span> | <span data-ttu-id="0cd2e-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="0cd2e-174">この列にはユーザーまたはグループの値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="0cd2e-175">**text**</span><span class="sxs-lookup"><span data-stu-id="0cd2e-175">**text**</span></span>          | <span data-ttu-id="0cd2e-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="0cd2e-176">[textColumn][]</span></span>          | <span data-ttu-id="0cd2e-177">この列にはテキスト値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-177">This column stores text values.</span></span>

<span data-ttu-id="0cd2e-178">注: これらのプロパティは SharePoint の [SPFieldType][] 列挙体に対応しています。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="0cd2e-179">中、最も一般的な種類のフィールドは、上は、この API がまだないです。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-179">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="0cd2e-180">そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="0cd2e-181">備考</span><span class="sxs-lookup"><span data-stu-id="0cd2e-181">Remarks</span></span>

<span data-ttu-id="0cd2e-182">`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="0cd2e-183">**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="0cd2e-184">[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。</span><span class="sxs-lookup"><span data-stu-id="0cd2e-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
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
