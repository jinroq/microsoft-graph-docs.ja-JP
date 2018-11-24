---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: a9c715983d83a448175c2c9d4110a92ff71edbbe
ms.sourcegitcommit: ebac77d2ca32438e552831de0258fe5e86fa225a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/17/2018
ms.locfileid: "26571666"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="446ce-102">ColumnDefinition リソース</span><span class="sxs-lookup"><span data-stu-id="446ce-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="446ce-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="446ce-103">JSON representation</span></span>

<span data-ttu-id="446ce-104">以下は、ColumnDefinition リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="446ce-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="446ce-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="446ce-105">Properties</span></span>

<span data-ttu-id="446ce-106">**columnDefinition** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="446ce-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="446ce-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="446ce-107">Property name</span></span>           | <span data-ttu-id="446ce-108">種類</span><span class="sxs-lookup"><span data-stu-id="446ce-108">Type</span></span>    | <span data-ttu-id="446ce-109">説明</span><span class="sxs-lookup"><span data-stu-id="446ce-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="446ce-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="446ce-110">**columnGroup**</span></span>         | <span data-ttu-id="446ce-111">string</span><span class="sxs-lookup"><span data-stu-id="446ce-111">string</span></span>  | <span data-ttu-id="446ce-112">サイト列の場合、この列が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="446ce-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="446ce-113">関連する列を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="446ce-113">Helps organize related columns.</span></span>
| <span data-ttu-id="446ce-114">**description**</span><span class="sxs-lookup"><span data-stu-id="446ce-114">**description**</span></span>         | <span data-ttu-id="446ce-115">string</span><span class="sxs-lookup"><span data-stu-id="446ce-115">string</span></span>  | <span data-ttu-id="446ce-116">列に関するユーザー向けの説明。</span><span class="sxs-lookup"><span data-stu-id="446ce-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="446ce-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="446ce-117">**displayName**</span></span>         | <span data-ttu-id="446ce-118">string</span><span class="sxs-lookup"><span data-stu-id="446ce-118">string</span></span>  | <span data-ttu-id="446ce-119">列を示すユーザー向けの名前。</span><span class="sxs-lookup"><span data-stu-id="446ce-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="446ce-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="446ce-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="446ce-121">boolean</span><span class="sxs-lookup"><span data-stu-id="446ce-121">boolean</span></span> | <span data-ttu-id="446ce-122">True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="446ce-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="446ce-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="446ce-123">**hidden**</span></span>              | <span data-ttu-id="446ce-124">boolean</span><span class="sxs-lookup"><span data-stu-id="446ce-124">boolean</span></span> | <span data-ttu-id="446ce-125">この列がユーザー インターフェイスに表示されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="446ce-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="446ce-126">**id**</span><span class="sxs-lookup"><span data-stu-id="446ce-126">**id**</span></span>                  | <span data-ttu-id="446ce-127">string</span><span class="sxs-lookup"><span data-stu-id="446ce-127">string</span></span>  | <span data-ttu-id="446ce-128">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="446ce-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="446ce-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="446ce-129">**indexed**</span></span>             | <span data-ttu-id="446ce-130">boolean</span><span class="sxs-lookup"><span data-stu-id="446ce-130">boolean</span></span> | <span data-ttu-id="446ce-131">列の値を、並べ替えと検索に使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="446ce-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="446ce-132">**name**</span><span class="sxs-lookup"><span data-stu-id="446ce-132">**name**</span></span>                | <span data-ttu-id="446ce-133">string</span><span class="sxs-lookup"><span data-stu-id="446ce-133">string</span></span>  | <span data-ttu-id="446ce-134">[listItem][] の [fields][] に表示される、列を示す API 向けの名前。</span><span class="sxs-lookup"><span data-stu-id="446ce-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="446ce-135">ユーザー向けの名前については **displayName** をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="446ce-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="446ce-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="446ce-136">**readOnly**</span></span>            | <span data-ttu-id="446ce-137">bool</span><span class="sxs-lookup"><span data-stu-id="446ce-137">bool</span></span>    | <span data-ttu-id="446ce-138">列の値を変更できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="446ce-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="446ce-139">**required**</span><span class="sxs-lookup"><span data-stu-id="446ce-139">**required**</span></span>            | <span data-ttu-id="446ce-140">boolean</span><span class="sxs-lookup"><span data-stu-id="446ce-140">boolean</span></span> | <span data-ttu-id="446ce-141">列の値が省略不可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="446ce-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="446ce-142">列には、さまざまな種類のデータを保持できます。</span><span class="sxs-lookup"><span data-stu-id="446ce-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="446ce-143">次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="446ce-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="446ce-144">これらのプロパティは相互に排他的で、各列でいずれか 1 つだけを指定できます。</span><span class="sxs-lookup"><span data-stu-id="446ce-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="446ce-145">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="446ce-145">Property name</span></span>     | <span data-ttu-id="446ce-146">種類</span><span class="sxs-lookup"><span data-stu-id="446ce-146">Type</span></span>                    | <span data-ttu-id="446ce-147">説明</span><span class="sxs-lookup"><span data-stu-id="446ce-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="446ce-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="446ce-148">**boolean**</span></span>       | <span data-ttu-id="446ce-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-149">[booleanColumn][]</span></span>       | <span data-ttu-id="446ce-150">この列にはブール値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-150">This column stores boolean values.</span></span>
| <span data-ttu-id="446ce-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="446ce-151">**calculated**</span></span>    | <span data-ttu-id="446ce-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="446ce-153">この列のデータは、他の列に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="446ce-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="446ce-154">**choice**</span></span>        | <span data-ttu-id="446ce-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-155">[choiceColumn][]</span></span>        | <span data-ttu-id="446ce-156">この列には、選択肢リストからのデータが格納されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="446ce-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="446ce-157">**currency**</span></span>      | <span data-ttu-id="446ce-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-158">[currencyColumn][]</span></span>      | <span data-ttu-id="446ce-159">この列には通貨値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-159">This column stores currency values.</span></span>
| <span data-ttu-id="446ce-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="446ce-160">**dateTime**</span></span>      | <span data-ttu-id="446ce-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="446ce-162">この列には日時の値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="446ce-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="446ce-163">**defaultValue**</span></span>  | <span data-ttu-id="446ce-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="446ce-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="446ce-165">この列の既定値です。</span><span class="sxs-lookup"><span data-stu-id="446ce-165">The default value for this column.</span></span>
| <span data-ttu-id="446ce-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="446ce-166">**lookup**</span></span>        | <span data-ttu-id="446ce-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-167">[lookupColumn][]</span></span>        | <span data-ttu-id="446ce-168">この列のデータは、サイト内の別のソースから検索されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="446ce-169">**number**</span><span class="sxs-lookup"><span data-stu-id="446ce-169">**number**</span></span>        | <span data-ttu-id="446ce-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-170">[numberColumn][]</span></span>        | <span data-ttu-id="446ce-171">この列には数値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-171">This column stores number values.</span></span>
| <span data-ttu-id="446ce-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="446ce-172">**personOrGroup**</span></span> | <span data-ttu-id="446ce-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="446ce-174">この列にはユーザーまたはグループの値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="446ce-175">**text**</span><span class="sxs-lookup"><span data-stu-id="446ce-175">**text**</span></span>          | <span data-ttu-id="446ce-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="446ce-176">[textColumn][]</span></span>          | <span data-ttu-id="446ce-177">この列にはテキスト値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="446ce-177">This column stores text values.</span></span>

<span data-ttu-id="446ce-178">注: これらのプロパティは SharePoint の [SPFieldType][] 列挙体に対応しています。</span><span class="sxs-lookup"><span data-stu-id="446ce-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="446ce-179">中、最も一般的な種類のフィールドは、上は、この API がまだないです。</span><span class="sxs-lookup"><span data-stu-id="446ce-179">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="446ce-180">そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。</span><span class="sxs-lookup"><span data-stu-id="446ce-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="446ce-181">備考</span><span class="sxs-lookup"><span data-stu-id="446ce-181">Remarks</span></span>

<span data-ttu-id="446ce-182">`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。</span><span class="sxs-lookup"><span data-stu-id="446ce-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="446ce-183">**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。</span><span class="sxs-lookup"><span data-stu-id="446ce-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="446ce-184">[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。</span><span class="sxs-lookup"><span data-stu-id="446ce-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleanColumn.md
[calculatedColumn]: calculatedColumn.md
[choiceColumn]: choiceColumn.md
[currencyColumn]: currencyColumn.md
[dateTimeColumn]: dateTimeColumn.md
[defaultColumnValue]: defaultColumnValue.md
[lookupColumn]: lookupColumn.md
[numberColumn]: numberColumn.md
[personOrGroupColumn]: personOrGroupColumn.md
[textColumn]: textColumn.md
[fieldValueSet]: fieldValueSet.md
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
