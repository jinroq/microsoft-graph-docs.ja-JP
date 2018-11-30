---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 96587cc1b3badf2d5fcc90bc7c1d2b1cfb710f6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021079"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="f3208-102">ColumnDefinition リソース</span><span class="sxs-lookup"><span data-stu-id="f3208-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3208-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3208-103">JSON representation</span></span>

<span data-ttu-id="f3208-104">以下は、ColumnDefinition リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3208-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f3208-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3208-105">Properties</span></span>

<span data-ttu-id="f3208-106">**columnDefinition** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="f3208-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="f3208-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f3208-107">Property name</span></span>           | <span data-ttu-id="f3208-108">種類</span><span class="sxs-lookup"><span data-stu-id="f3208-108">Type</span></span>    | <span data-ttu-id="f3208-109">説明</span><span class="sxs-lookup"><span data-stu-id="f3208-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="f3208-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="f3208-110">**columnGroup**</span></span>         | <span data-ttu-id="f3208-111">string</span><span class="sxs-lookup"><span data-stu-id="f3208-111">string</span></span>  | <span data-ttu-id="f3208-112">サイト列の場合、この列が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="f3208-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="f3208-113">関連する列を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="f3208-113">Helps organize related columns.</span></span>
| <span data-ttu-id="f3208-114">**description**</span><span class="sxs-lookup"><span data-stu-id="f3208-114">**description**</span></span>         | <span data-ttu-id="f3208-115">string</span><span class="sxs-lookup"><span data-stu-id="f3208-115">string</span></span>  | <span data-ttu-id="f3208-116">列に関するユーザー向けの説明。</span><span class="sxs-lookup"><span data-stu-id="f3208-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="f3208-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f3208-117">**displayName**</span></span>         | <span data-ttu-id="f3208-118">string</span><span class="sxs-lookup"><span data-stu-id="f3208-118">string</span></span>  | <span data-ttu-id="f3208-119">列を示すユーザー向けの名前。</span><span class="sxs-lookup"><span data-stu-id="f3208-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="f3208-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="f3208-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="f3208-121">boolean</span><span class="sxs-lookup"><span data-stu-id="f3208-121">boolean</span></span> | <span data-ttu-id="f3208-122">True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="f3208-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="f3208-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="f3208-123">**hidden**</span></span>              | <span data-ttu-id="f3208-124">boolean</span><span class="sxs-lookup"><span data-stu-id="f3208-124">boolean</span></span> | <span data-ttu-id="f3208-125">この列がユーザー インターフェイスに表示されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3208-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="f3208-126">**id**</span><span class="sxs-lookup"><span data-stu-id="f3208-126">**id**</span></span>                  | <span data-ttu-id="f3208-127">string</span><span class="sxs-lookup"><span data-stu-id="f3208-127">string</span></span>  | <span data-ttu-id="f3208-128">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f3208-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="f3208-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="f3208-129">**indexed**</span></span>             | <span data-ttu-id="f3208-130">boolean</span><span class="sxs-lookup"><span data-stu-id="f3208-130">boolean</span></span> | <span data-ttu-id="f3208-131">列の値を、並べ替えと検索に使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3208-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="f3208-132">**name**</span><span class="sxs-lookup"><span data-stu-id="f3208-132">**name**</span></span>                | <span data-ttu-id="f3208-133">string</span><span class="sxs-lookup"><span data-stu-id="f3208-133">string</span></span>  | <span data-ttu-id="f3208-134">[listItem][] の [fields][] に表示される、列を示す API 向けの名前。</span><span class="sxs-lookup"><span data-stu-id="f3208-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="f3208-135">ユーザー向けの名前については **displayName** をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f3208-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="f3208-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="f3208-136">**readOnly**</span></span>            | <span data-ttu-id="f3208-137">bool</span><span class="sxs-lookup"><span data-stu-id="f3208-137">bool</span></span>    | <span data-ttu-id="f3208-138">列の値を変更できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3208-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="f3208-139">**required**</span><span class="sxs-lookup"><span data-stu-id="f3208-139">**required**</span></span>            | <span data-ttu-id="f3208-140">boolean</span><span class="sxs-lookup"><span data-stu-id="f3208-140">boolean</span></span> | <span data-ttu-id="f3208-141">列の値が省略不可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3208-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="f3208-142">列には、さまざまな種類のデータを保持できます。</span><span class="sxs-lookup"><span data-stu-id="f3208-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="f3208-143">次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="f3208-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="f3208-144">これらのプロパティは相互に排他的で、各列でいずれか 1 つだけを指定できます。</span><span class="sxs-lookup"><span data-stu-id="f3208-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="f3208-145">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f3208-145">Property name</span></span>     | <span data-ttu-id="f3208-146">種類</span><span class="sxs-lookup"><span data-stu-id="f3208-146">Type</span></span>                    | <span data-ttu-id="f3208-147">説明</span><span class="sxs-lookup"><span data-stu-id="f3208-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="f3208-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="f3208-148">**boolean**</span></span>       | <span data-ttu-id="f3208-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-149">[booleanColumn][]</span></span>       | <span data-ttu-id="f3208-150">この列にはブール値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-150">This column stores boolean values.</span></span>
| <span data-ttu-id="f3208-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="f3208-151">**calculated**</span></span>    | <span data-ttu-id="f3208-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="f3208-153">この列のデータは、他の列に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="f3208-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="f3208-154">**choice**</span></span>        | <span data-ttu-id="f3208-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-155">[choiceColumn][]</span></span>        | <span data-ttu-id="f3208-156">この列には、選択肢リストからのデータが格納されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="f3208-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="f3208-157">**currency**</span></span>      | <span data-ttu-id="f3208-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-158">[currencyColumn][]</span></span>      | <span data-ttu-id="f3208-159">この列には通貨値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-159">This column stores currency values.</span></span>
| <span data-ttu-id="f3208-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="f3208-160">**dateTime**</span></span>      | <span data-ttu-id="f3208-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="f3208-162">この列には日時の値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="f3208-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="f3208-163">**defaultValue**</span></span>  | <span data-ttu-id="f3208-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="f3208-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="f3208-165">この列の既定値です。</span><span class="sxs-lookup"><span data-stu-id="f3208-165">The default value for this column.</span></span>
| <span data-ttu-id="f3208-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="f3208-166">**lookup**</span></span>        | <span data-ttu-id="f3208-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-167">[lookupColumn][]</span></span>        | <span data-ttu-id="f3208-168">この列のデータは、サイト内の別のソースから検索されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="f3208-169">**number**</span><span class="sxs-lookup"><span data-stu-id="f3208-169">**number**</span></span>        | <span data-ttu-id="f3208-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-170">[numberColumn][]</span></span>        | <span data-ttu-id="f3208-171">この列には数値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-171">This column stores number values.</span></span>
| <span data-ttu-id="f3208-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="f3208-172">**personOrGroup**</span></span> | <span data-ttu-id="f3208-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="f3208-174">この列にはユーザーまたはグループの値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="f3208-175">**text**</span><span class="sxs-lookup"><span data-stu-id="f3208-175">**text**</span></span>          | <span data-ttu-id="f3208-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="f3208-176">[textColumn][]</span></span>          | <span data-ttu-id="f3208-177">この列にはテキスト値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="f3208-177">This column stores text values.</span></span>

<span data-ttu-id="f3208-178">注: これらのプロパティは SharePoint の [SPFieldType][] 列挙体に対応しています。</span><span class="sxs-lookup"><span data-stu-id="f3208-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="f3208-179">中、最も一般的な種類のフィールドは、上は、この API がまだないです。</span><span class="sxs-lookup"><span data-stu-id="f3208-179">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="f3208-180">そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。</span><span class="sxs-lookup"><span data-stu-id="f3208-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="f3208-181">備考</span><span class="sxs-lookup"><span data-stu-id="f3208-181">Remarks</span></span>

<span data-ttu-id="f3208-182">`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。</span><span class="sxs-lookup"><span data-stu-id="f3208-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="f3208-183">**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。</span><span class="sxs-lookup"><span data-stu-id="f3208-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="f3208-184">[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。</span><span class="sxs-lookup"><span data-stu-id="f3208-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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
