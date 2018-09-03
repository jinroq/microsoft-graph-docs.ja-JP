---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 2fd6c08e1cfc28a77019d174763b9d698519b6a2
ms.sourcegitcommit: 9e4dc7745eb1bbbe595afd8c7f3db4c19c6bb4ac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2018
ms.locfileid: "23271316"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="5b008-102">ColumnDefinition リソース</span><span class="sxs-lookup"><span data-stu-id="5b008-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b008-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b008-103">JSON representation</span></span>

<span data-ttu-id="5b008-104">以下は、ColumnDefinition リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b008-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5b008-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b008-105">Properties</span></span>

<span data-ttu-id="5b008-106">**columnDefinition** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="5b008-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="5b008-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="5b008-107">Property name</span></span>           | <span data-ttu-id="5b008-108">型</span><span class="sxs-lookup"><span data-stu-id="5b008-108">Type</span></span>    | <span data-ttu-id="5b008-109">説明</span><span class="sxs-lookup"><span data-stu-id="5b008-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="5b008-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="5b008-110">**columnGroup**</span></span>         | <span data-ttu-id="5b008-111">文字列</span><span class="sxs-lookup"><span data-stu-id="5b008-111">string</span></span>  | <span data-ttu-id="5b008-112">サイト列の場合、この列が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="5b008-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="5b008-113">関連する列を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5b008-113">Helps organize related columns.</span></span>
| <span data-ttu-id="5b008-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5b008-114">**description**</span></span>         | <span data-ttu-id="5b008-115">文字列</span><span class="sxs-lookup"><span data-stu-id="5b008-115">string</span></span>  | <span data-ttu-id="5b008-116">列に関するユーザー向けの説明。</span><span class="sxs-lookup"><span data-stu-id="5b008-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="5b008-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="5b008-117">**displayName**</span></span>         | <span data-ttu-id="5b008-118">文字列</span><span class="sxs-lookup"><span data-stu-id="5b008-118">string</span></span>  | <span data-ttu-id="5b008-119">列を示すユーザー向けの名前。</span><span class="sxs-lookup"><span data-stu-id="5b008-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="5b008-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="5b008-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="5b008-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="5b008-121">boolean</span></span> | <span data-ttu-id="5b008-122">True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="5b008-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="5b008-123">**隠し**</span><span class="sxs-lookup"><span data-stu-id="5b008-123">**hidden**</span></span>              | <span data-ttu-id="5b008-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="5b008-124">boolean</span></span> | <span data-ttu-id="5b008-125">この列がユーザー インターフェイスに表示されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5b008-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="5b008-126">**ID**</span><span class="sxs-lookup"><span data-stu-id="5b008-126">**id**</span></span>                  | <span data-ttu-id="5b008-127">文字列</span><span class="sxs-lookup"><span data-stu-id="5b008-127">string</span></span>  | <span data-ttu-id="5b008-128">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5b008-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="5b008-129">**インデックス済**</span><span class="sxs-lookup"><span data-stu-id="5b008-129">**indexed**</span></span>             | <span data-ttu-id="5b008-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="5b008-130">boolean</span></span> | <span data-ttu-id="5b008-131">列の値を、並べ替えと検索に使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5b008-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="5b008-132">**名前**</span><span class="sxs-lookup"><span data-stu-id="5b008-132">**name**</span></span>                | <span data-ttu-id="5b008-133">文字列</span><span class="sxs-lookup"><span data-stu-id="5b008-133">string</span></span>  | <span data-ttu-id="5b008-134">[listItem][] の [fields][] に表示される、列を示す API 向けの名前。</span><span class="sxs-lookup"><span data-stu-id="5b008-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="5b008-135">ユーザー向けの名前については **displayName** をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5b008-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="5b008-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="5b008-136">**readOnly**</span></span>            | <span data-ttu-id="5b008-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="5b008-137">bool</span></span>    | <span data-ttu-id="5b008-138">列の値を変更できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5b008-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="5b008-139">**必須です**</span><span class="sxs-lookup"><span data-stu-id="5b008-139">**required**</span></span>            | <span data-ttu-id="5b008-140">ブール値</span><span class="sxs-lookup"><span data-stu-id="5b008-140">boolean</span></span> | <span data-ttu-id="5b008-141">列の値が省略不可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5b008-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="5b008-142">列には、さまざまな種類のデータを保持できます。</span><span class="sxs-lookup"><span data-stu-id="5b008-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="5b008-143">次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="5b008-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="5b008-144">これらのプロパティは相互に排他的で、各列でいずれか 1 つだけを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5b008-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="5b008-145">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="5b008-145">Property name</span></span>     | <span data-ttu-id="5b008-146">型</span><span class="sxs-lookup"><span data-stu-id="5b008-146">Type</span></span>                    | <span data-ttu-id="5b008-147">説明</span><span class="sxs-lookup"><span data-stu-id="5b008-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="5b008-148">**ブール値**</span><span class="sxs-lookup"><span data-stu-id="5b008-148">**boolean**</span></span>       | <span data-ttu-id="5b008-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-149">[booleanColumn][]</span></span>       | <span data-ttu-id="5b008-150">この列にはブール値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-150">This column stores boolean values.</span></span>
| <span data-ttu-id="5b008-151">**計算済み**</span><span class="sxs-lookup"><span data-stu-id="5b008-151">**calculated**</span></span>    | <span data-ttu-id="5b008-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="5b008-153">この列のデータは、他の列に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="5b008-154">**選択**</span><span class="sxs-lookup"><span data-stu-id="5b008-154">**choice**</span></span>        | <span data-ttu-id="5b008-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-155">[choiceColumn][]</span></span>        | <span data-ttu-id="5b008-156">この列には、選択肢リストからのデータが格納されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="5b008-157">**通貨**</span><span class="sxs-lookup"><span data-stu-id="5b008-157">**currency**</span></span>      | <span data-ttu-id="5b008-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-158">[currencyColumn][]</span></span>      | <span data-ttu-id="5b008-159">この列には通貨値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-159">This column stores currency values.</span></span>
| <span data-ttu-id="5b008-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="5b008-160">**dateTime**</span></span>      | <span data-ttu-id="5b008-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="5b008-162">この列には日時の値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="5b008-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="5b008-163">**defaultValue**</span></span>  | <span data-ttu-id="5b008-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="5b008-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="5b008-165">この列の既定値です。</span><span class="sxs-lookup"><span data-stu-id="5b008-165">The default value for this column.</span></span>
| <span data-ttu-id="5b008-166">**参照**</span><span class="sxs-lookup"><span data-stu-id="5b008-166">**lookup**</span></span>        | <span data-ttu-id="5b008-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-167">[lookupColumn][]</span></span>        | <span data-ttu-id="5b008-168">この列のデータは、サイト内の別のソースから検索されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="5b008-169">**数**</span><span class="sxs-lookup"><span data-stu-id="5b008-169">**number**</span></span>        | <span data-ttu-id="5b008-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-170">[numberColumn][]</span></span>        | <span data-ttu-id="5b008-171">この列には数値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-171">This column stores number values.</span></span>
| <span data-ttu-id="5b008-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="5b008-172">**personOrGroup**</span></span> | <span data-ttu-id="5b008-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="5b008-174">この列にはユーザーまたはグループの値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="5b008-175">**テキスト**</span><span class="sxs-lookup"><span data-stu-id="5b008-175">**text**</span></span>          | <span data-ttu-id="5b008-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="5b008-176">[textColumn][]</span></span>          | <span data-ttu-id="5b008-177">この列にはテキスト値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="5b008-177">This column stores text values.</span></span>

<span data-ttu-id="5b008-178">注: これらのプロパティは SharePoint の [SPFieldType][] 列挙体に対応しています。</span><span class="sxs-lookup"><span data-stu-id="5b008-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="5b008-179">ほとんどの一般的なフィールドの種類を上記に示しましたが、この API には含まれないものもあります。</span><span class="sxs-lookup"><span data-stu-id="5b008-179">While the most common field types are represented above, this beta API is still missing some.</span></span>
<span data-ttu-id="5b008-180">そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。</span><span class="sxs-lookup"><span data-stu-id="5b008-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="5b008-181">備考</span><span class="sxs-lookup"><span data-stu-id="5b008-181">Remarks</span></span>

<span data-ttu-id="5b008-182">列の ColumnDefinitions とフィールドの値は、既定では表示されません。`hidden`</span><span class="sxs-lookup"><span data-stu-id="5b008-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="5b008-183">**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。</span><span class="sxs-lookup"><span data-stu-id="5b008-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="5b008-184">[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。</span><span class="sxs-lookup"><span data-stu-id="5b008-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
